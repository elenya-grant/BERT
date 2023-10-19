# Baseline Electrolyzer Reference-design Tool (BERT)

This tool serves as an electrolyzer reference design, performance, and analysis tool and contains a library of various electrolyzer reference designs. This tool is intended to compliment existing tools by providing a large-scope of custom capabilities related to electrolysis. At the base-level, BERT will have electrolyzer reference designs for current and forecasted technology, highlight sensitivities to cell-level design variables, include multi-timescale and multi-forecast control strategies, include power-to-hydrogen and hydrogen-to-power calculations, provide a life-cycle-assessment of performance, and include baseline financial values.

## The goal of BERT:
- no hard-coded design variables that allows for easy-to-test sensitivity studies
- easy to modify and modular code design so that its developer-friendly 
- detailed documentation of resources, units, default-assumptions, and valid regions for design variables
- provide models of reference designs and validation studies
- assist with cell-level and stack-level design to use with other tools
- upfront documentation of ignored dynamics or assumptions

## BERT: Electrolyzer Design:
- user-customized electrolyzer cell-level design
    * custom degradation rates, efficiency, losses, etc
    * custom end-of-life definition
    * sensitivity studies to different design variables
- user-customized electrolyzer stack-level design
    * cold-start vs warm-start dynamics
    * operation range
    * ramp-rates
- library of reference designs 
    * documented or well-known current technology designs
    * documentation of design constraints
    * forecasted technology designs
- test best IV curve equation
    * test error for different equation fits
- (dream)
    * include how design changes impact dynamcis, degradation, cost, etc

## BERT: characterization & analysis
- characterization/visualization/trade-offs
    * efficiency curve (BOL vs EOL)
- LCOH calculation
- performance per year over entire plant life
- linear model

## herBERT: Hybrid ElectrolyzeR
- pem + alkaline optimal combination
- hydrogen set-back requirements
- electrolyzer footprint
- area-constrained electrolyzer capacity

## Electrolyzer+ Operation Capabilities:
### power-to-hydrogen
1. coordination with storage
    - upstream battery storage
    - downstream hydrogen storage
2. given an energy profile, optimize:
    - total electrolyzer capacity
    - stack size
    - energy dispatch

### hydrogen-to-power 
1. estimate energy required profile from an input hydrogen demand
    - constant hydrogen demand
    - peaker-plant style hydrogen demand
    - completely variable
    - constrained constant (72 hour constant production, then off for x hours)

2. include constraints/optimizations for
    - stack size/electrolyzer capacity
    - grid interconnection limit
    - optimize for lowest LCOH considering
        * grid price profile
        * hydrogen storage
        * meeting load demand (is shortfall allowed)
        * water usage/season
        * stack degradation
### hydrogen-to-x
1. compare how hydrogen demand profile changes sizing, operation, degradation, etc
2. make hydrogen demand profile given h2-to-x conversation ratio and other constraints

## BOS
- BOS constraints/considerations
    - ancillary equipment power usage
    - Hydrogen losses
    - BOS system design specs
        * transmission pipeline sizing
        * compressor sizing
- Scheduled maintenance?

### Electrolyzer Operation Constraints
- power-to-hydrogen
- hydrogen-to-power
- hydrogen-to-x


- coordination with storage
    - upstream battery storage
    - downstream hydrogen storage

- BOS constraints/considerations
    - ancillary equipment power usage
    - Hydrogen losses
    - BOS system design specs
        * transmission pipeline sizing
        * compressor sizing

### 
 various use-cases for electrolyzer design and performance analysis.

1. 