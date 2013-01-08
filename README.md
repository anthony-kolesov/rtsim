RTSim
=====

RTSim stands for Road traffic simulator (I haven't spent much time thinking
about name). It employes a microsimulation model.
That means that each car is simulated on its own. Compare this with
macrosimulation models that simulate traffic as a whole streams. This models
uses a discreet time which means that simulation is run in sequantial steps
with constant time offset between these steps. At each step behavior for each
simulated object is evaluated. My model uses a shanpshot approach here - each
car is simulated using model state at the beginning of step, changes in cars
state won't be visible until next step. That solves the probelm of defining
the order of car simulation - obviously if all cars use he same model state the
order is irrelevant. 

This project is based on my diploma work, however I start this from the scratch
without code reuse but using already gained experience.
