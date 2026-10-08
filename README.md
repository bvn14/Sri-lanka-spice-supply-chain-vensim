# Sri Lanka Spice Supply Chain: System Dynamics Model

A stock and flow model of the Sri Lankan spice supply chain, built in Vensim PLE. The model follows spices from farm harvest to domestic sales and export.

Course project for DA3411 Business Valuation and Analysis, Department of Decision Science, University of Moratuwa.

## What I did

- Mapped the spice supply chain from farm to export market
- Built a stock and flow diagram in Vensim
- Ran a 60-month simulation and analysed the results for each stage of the chain
- Documented the model, equations, assumptions and results in a report

## Model structure

<img width="1390" height="550" alt="stock_flow_diagram" src="https://github.com/user-attachments/assets/0b197734-393c-4928-a86b-4fef1c6ec8c6" />


**Stocks:** Farm Inventory, Processor WIP, Finished Goods Inventory, Export Pipeline

**Flows:** harvest, farm dispatch to processing, processing completion, domestic sales, export shipments, export deliveries, and spoilage at the farm, processing and warehouse stages

**Main variables:** base harvest, processing capacity, handling time, processing lead time, dispatch capacity, dispatch time, shipping lead time, spoilage fractions, domestic demand, export demand

**Shipment logic:** shipments are the minimum of total demand, dispatch capacity and available finished goods. They are split between domestic and export markets based on each market's share of total demand.

**Simulation settings:** 60 months, time step 0.125 month

## Repository contents

```
.
├── model/
│   └── Spice_supply_chain.mdl
├── report/
│   └── Spice_Supply_Chain_Report.pdf
├── images/
│   └── stock_flow_diagram.png
└── README.md
```

## How to run

1. Install [Vensim PLE](https://vensim.com/vensim-personal-learning-edition/) (free for education).
2. Open `model/Spice_supply_chain.mdl`.
3. Click Simulate and view the graphs for each stock and flow.

## Tools

Vensim PLE, system dynamics modelling

## Author

Bavindu Gunasinghe
