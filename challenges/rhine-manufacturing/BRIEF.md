# From a Rhine Signal to Action — Manufacturing in the BioValley

> Use real Rhine-region data to keep critical biopharma materials moving.

**Domain:** high-tech-manufacturing

## Original challenge wording

Build a smart manufacturing cell that turns real public data about Rhine conditions, Basel traffic and weather into physical decisions on the factory floor: prioritize, buffer, reroute or quarantine critical material.

Basel is one of Europe's major life-sciences manufacturing regions. Modern pharmaceutical and biotech production depends not only on what happens inside a factory, but also on what is happening around it.

A change in Rhine conditions can affect logistics. Heavy road traffic can delay deliveries. Extreme weather can increase transportation and cold-chain risk.

What if a factory could see these disruptions developing and change its material-flow decisions before production is affected?

Your challenge is to build a manufacturing control system that turns real-world open data into actionable factory decisions.

## The manufacturing scenario

Imagine a Basel-area biopharmaceutical manufacturing facility.

The factory depends on a critical refrigerated biopharma reagent or intermediate used during production.

For the purpose of this challenge, assume that the material:

- requires refrigerated handling at 2–8°C;
- is critical to an upcoming manufacturing step;
- should spend as little unnecessary time as possible outside controlled storage;
- may require quality review if its handling conditions are uncertain;
- cannot simply be replaced instantly if the next delivery is disrupted.

The factory therefore needs to continuously decide what should happen to critical material already in its network.

## Possible actions

- **EXPEDITE** — Prioritize the material and move it toward the required production step.
- **BUFFER** — Keep the material safely in controlled storage until it is required.
- **REROUTE** — Recommend another logistics route, receiving point or manufacturing path because the expected route is at risk.
- **QUARANTINE** — Flag the material for quality review when conditions indicate that its handling may have been compromised.

Your system should explain why it made its decision.

## Your mission

Build a working application that combines at least two real open-data sources and converts them into a manufacturing risk or priority decision.

Basic pipeline:

```
Open Data → Disturbance Detection → Risk Assessment → Manufacturing Decision → Factory Dashboard
```

Teams may use current data or replay a real historical period.

## Disturbance sources described in the challenge

### Rhine conditions

Use real measurements of Rhine water level and discharge around Basel.

Potential signals:

- rapidly rising water levels;
- high-water conditions;
- unusually low water conditions;
- significant changes in discharge;
- trends indicating deteriorating conditions.

Translate the signal into the manufacturing question:

> Could replenishment of a critical production material become less reliable?

### Basel road traffic

Use real traffic-counting data to identify congestion or unusually high traffic around important logistics corridors.

Potential signals:

- increased vehicle counts;
- increased heavy-vehicle traffic;
- unusual congestion periods;
- differences between normal and abnormal traffic patterns.

Potential action sequence:

`NORMAL → BUFFER → EXPEDITE → REROUTE`

### Weather

Use MeteoSwiss measurements such as:

- temperature;
- precipitation;
- wind;
- humidity;
- radiation.

Weather can affect transport reliability and refrigerated-material handling risk.

## What should you build?

1. **Open-data integration** — connect or import at least two provided open datasets.
2. **Disturbance detection** — determine when conditions become unusual or operationally important.
3. **Manufacturing risk score** — convert conditions into an operator-readable state.
4. **Factory decision** — recommend at least one of EXPEDITE, BUFFER, REROUTE or QUARANTINE and explain why.
5. **Visual interface** — show the decision so a manufacturing operator can understand it quickly.

## Resources named by the challenge

- Basel Rhine Water Level & Discharge
- Basel Motor Traffic Counts
- MeteoSwiss Weather Data API
- Port of Switzerland — Rhine Navigation Conditions
- WHO — Temperature-Sensitive Pharmaceutical Storage & Transport
