Authors
J. M. PEARSON1, S. N. IQBAL1, C. B. DRUCKER2, M. L. PLATT3;
1Duke Inst. for Brain Sci., 2Neurobio., Duke Univ., Durham, NC; 3Neurosci., Univ. of Pennsylvania, Philadelphia, PA
Disclosures
 J.M. Pearson: None. S.N. Iqbal: None. C.B. Drucker: None. M.L. Platt: None.
Abstract
The ecological niches occupied by most organisms, including humans, are both dynamic and uncertain, requiring that actions be taken in real time and modified in response to changing circumstances. However, most studies of dynamic decision-making to date have explored either repeated trials of the same task under slowly changing circumstances (e.g., bandit problems) or interactions between agents that take place in a restricted action space (e.g., prisoner’s dilemma). Here, we examine data from repeated trials of a real-time strategic interaction with continuous freedom of movement. We trained monkeys to play a competitive task in which the goal of one (the “shooter”) was to move a colored dot (the “ball”) from the left to right side of a computer monitor using joystick input. The goal of the second monkey (the “goalie”) was to block the dot by moving a vertical line along the right-hand side of the screen to intercept the it. Thus, each player controlled an avatar with at least one continuous degree of freedom, in principle allowing for dynamic coupling between the two in real time.
We analyzed these data using time series methods borrowed from the machine learning and optimal control literatures. We modeled each player’s avatar as a state space model with control input dependent on the dynamics of both players’ behavior. That is, the kicker’s control action was modeled as a filtered sum of his own and the goalie’s past trajectories (and vice-versa for the goalie). The model produces a set of filters and time series that can be used for subsequent analysis of neural data in terms of dynamic control signals derived from behavior.

# Main take-aways

- Real-world social decisions take place in dynamic environments
  - not just constrained sets of actions
- Real decisions take place in physical context
  - brains are for movementi!
  - taking advantage of decisions' piggybacking on movement signals
- by careful modeling, we can ameliorate the complexity penalty of less constrained tasks in a
  way that makes neural analysis possible and reveals interesting behavior
  - modularity is a key
  - principled modeling to be preferred over totally black box

# Slides
1. title
1. acknowledgments
1. social decisions are biologically important
  - but how to study in lab?
1. economic games
  - big literature, normative solution
  - but can be unrealistic, misaligned with brain structure
  - not dynamic in the way we might want
1. example: a penalty shot
  - social decision
  - repeatable, but lots of dynamic variation
  - decisions tightly coupled to motor actions
1. penalty shot task (video; autoplay and loop):
  - two monkeys, shooter and goalie (shooter recorded)
  - controlled by joysticks
  - roles rotated, animals know each other
  - repeated sessions
  - rapidly learned, rich dynamics
1. but there's a complexity tax
  - no clear way to average trials together
    - different length of time
    - different dynamics
    - no obvious events (save trial end) to align to
  - would like to find a set of quantities that can
    predict (or be predicted by) neural signals
1. our approach:
  1. borrow from control theory, time series analysis
  1. make use of neural networks to fit data
  1. break down black box models into pieces that make sense
1. modeling (slides from MLP lab meeting)
  - three slides
1. fitting the model (idea)
  - NNs, Evan's model
1. fitting the model (details)
1. fitted trials
1. generated trials
1. trial distributions compared
1. systematic and innovation terms visualized
1. conclusions and future directions
