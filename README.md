# Standardization-Project
The resources for the plan recognition standardization project

#Domains
These domains are based on the domains from the following publications:

- 1-5-2-3-4-full: *Kabanza et al. Controlling the hypothesis space in probabilistic plan recognition. IJCAI. 2013.*
A simulated domain based on and/or trees. The values in the name represent the characretirsics of the domain - 1 plan execution, 5 possible goals, or-branching of 2, and-branching of 3, depth of 4, fully ordered. This domain has no parameters.

- Monroe: *Blaylock. Towards tractable agent-based dialogue. Diss. University of Rochester, 2005.*
A domain based on plan executions of disaster response teams. Parameterized domain, partial order.

- Soccer: *Avrahami-Zilberbrand, and Kaminka. Incorporating observer biases in keyhole plan recognition (efficiently!). AAAI. Vol. 7. 2007.*
A domain based on the robo-cup planning competition. This is a very simple domain,  no parameters and fully ordered.

- TinkerPlots: *Oriel Uzan, Reuth Dekel, Or Seri, Ya'akov Gal.  Plan Recognition for Exploratory Learning*
A domain based on student's traces in a statistics educational software. This domain has parameters, exogenous actions and partial ordering.

- VirtualLabs: *Reuth Mirsky, Ya'akov  Gal, Stuart Shieber. CRADLE: An Online Plan Recognition Algorithm for Exploratory Domains. ACM Transactions on Intelligent Systems and Technology*
A domain based on student's traces in a Chemistry educational software. This domain has parameters, partial ordering and recursive rules. It does not have exogenous actions.

#Algorithms
The following algorithms support the use of this XML format:

- SBR: *Dorit Avrahami-Zilberbrand and Gal A. Kaminka. Fast and Complete Symbolic Plan Recognition. In Proceedings of the International Joint Conference on Artificial Intelligence (IJCAI-05), pp. 653–658, 2005.*
A complete algorithm for plan recognition. Does not handle exogenous actions and partial ordering. It contains tree parts in a pipeline - FDT,CSQ and HSQ. Their code is available online, soon will be able to handle parameters.

- PHATT and CRADLE: *Geib and Goldman. A probabilistic plan recognition algorithm based on plan tree grammars. Artificial Intelligence173.11. 2009. 1101-1132.* and *Reuth Mirsky, Ya'akov  Gal, Stuart Shieber. CRADLE: An Online Plan Recognition Algorithm for Exploratory Domains. ACM Transactions on Intelligent Systems and Technology*
CRADLE is a heuristic algorithm, based on PHATT. Can handle parameter-binding, exogenous actions, partial ordering and filters. When turning these modules off, you can work with PHATT. The code of the PHATT and CRADLE algorithms with this format is found here: https://github.com/ReuthMirsky/CRADLE

- IPR: *Mirsky, Stern, Gal, Kalech. Sequential Plan Recognition. IJCAI. 2016.*
An interactive algorithm which facilitates queries during the plan recognition process. The code of the IPR algorithm with this format is found here: https://github.com/ReuthMirsky/SPR

- SLIM: *Mirsky, Gal. SLIM: Semi-Lazy Inference Mechanism for Plan Recognition. IJCAI. 2016.*
A complete algorithm, combined bottom-up and top-down explanation generation. Does not handle parameters and exogenous actions, but can handle partial ordering. The code of the SLIM algorithm with this format is found here: https://github.com/ReuthMirsky/SLIM
