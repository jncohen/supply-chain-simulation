# Supply Chain Simulator

A free classroom simulation of the bullwhip effect: an independent implementation of the Beer Distribution Game exercise, built from published system-dynamics research. Not affiliated with or endorsed by MIT.

- **Play it live:** https://jncohen.github.io/supply-chain-simulation/
- **Instructor page:** https://jncohen.commons.gc.cuny.edu/supply-chain-simulator/
- **Version:** 1.0.0

## Simulation Explained

In this simulation, participants assume one of four roles: Retailer, Wholesaler, Distributor, and Factory. Together, they form a linear supply chain of a hypothetical product. 

Each round, each person sees only their own inventory, backlog, and the order that just arrived from downstream. Your goal is to manage inventory and purchases so as to minimize your inventories while also satisfying demand.  Each person purchases products from someone earlier in the chain and sells to someone downstream.  You will make your estimates of consumer demand from the orders you receive from your downstream customer.  There is a time delay, such that (i) orders take two rounds to reach a supplier and (ii) shipments take two more rounds to arrive back. 

Built for classroom use: one shared device per group of four (a laptop, phone, or iPad in fullscreen, passed role to role), with a privacy screen between turns, a seeded-scenario setup step, and an end-of-game chart, cost table, and debrief prompts.

## How to run it

The game is hosted on the web. Open the link above in any browser. No install, no account, no server; once the page has loaded it runs without an internet connection.

1. **Before class.** Pick a scenario number (1–20) for each group. Give every group the same number to compare results, or different numbers to vary the shock.
2. **Set up.** One laptop, phone, or iPad per group, in fullscreen. Choose the scenario and the number of rounds (16 by default).
3. **Play.** Four students, four roles, one each. Pass the device role to role; the privacy screen hides each player's numbers from the next. A group of five pairs up on one role and decides together. The game tells players that customer demand changes once; do not tell them when or by how much.
4. **Debrief.** The end screen shows all four order lines against customer demand, a cost table, and four debrief prompts. Export the results as CSV or the chart as PNG.

## How it works

- 4-tier chain, 2-round order delay, 2-round shipping delay
- $0.50/unit/round holding cost, $1.00/unit/round backorder cost (standard Sterman parameters)
- Customer demand of 4 units per round, then one permanent step up between rounds 4 and 7; size and timing are set by the scenario and not shown to players
- 20 preset scenarios, each distinct in shock timing and size, plus a custom seed; the same scenario number always plays the same game

## Origin and attribution

The underlying exercise — a four-tier supply chain, ordering and shipping delays, and a demand shock that induces the bullwhip effect — was developed by J. W. Forrester and MIT's System Dynamics Group in the late 1950s, out of Forrester's industrial dynamics research. J. D. Sterman named it the "Beer Distribution Game" in 1984 and ran the canonical behavioral study this implementation's demand-shock design follows:

> Sterman, J. D. (1989). Modeling Managerial Behavior: Misperceptions of Feedback in a Dynamic Decision Making Experiment. *Management Science*, 35(3), 321–339.

This repository is an independent implementation built from the published academic record. The delay structure, cost parameters, and demand-shock design reproduced here are documented methodology in a peer-reviewed paper. No code, text, or materials from any licensed version of the game were used. Not affiliated with or endorsed by MIT.

## License

[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) — public domain dedication; see [LICENSE](LICENSE). Copy, adapt, host, or sell it, with no permission needed. A citation is appreciated but not required.

The dedication covers this implementation only: the code, interface, and debrief text. The underlying exercise design is published academic methodology (Forrester; Sterman) and was never this repository's to license.

## Citation

Cohen, J. N. (2026). *Supply Chain Simulator* (Version 1.0.0) [Web application]. https://jncohen.commons.gc.cuny.edu/supply-chain-simulator/

Source code: https://github.com/jncohen/supply-chain-simulation. GitHub's "Cite this repository" button reads [CITATION.cff](CITATION.cff).

## Using it in a course?

Tell me: the course, the number of students, and the date. Write to me through [jncohen.commons.gc.cuny.edu](https://jncohen.commons.gc.cuny.edu).

## AI acknowledgement

The game and this documentation were built with Claude, Anthropic's AI assistant, under the author's direction. The author chose the design, tested the game, and is responsible for its content.

## Author

Joseph N. Cohen — [jncohen.commons.gc.cuny.edu](https://jncohen.commons.gc.cuny.edu)
