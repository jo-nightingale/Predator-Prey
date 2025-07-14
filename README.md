# Predator-Prey
An agent based simulation for the predator-prey model, using zebras and lions. 

Features included: \
1. An animal class with basic features for all animals. It can move, see and detect enemies and allies. \
   a. Animals have a visibility range. If they can see enemies, they choose one of them as their current enemy. \
   b. Animals track collisions to determine whether they collide with enemies (and eat or are eaten) or collide with allies (and reproduce if they haven't done so recently). 
   
2. Subclasses for zebras and lions. \
   a. Lions choose a direction movement based on the zebra they are chasing. \
   b. Zebras choose a direction movement based on the lion they want to avoid. \
   c. If no visible enemies are around, animals will try and reproduce with animals of the same species. \
   d. Lions can also smell their prey. If they haven't eaten in a while they become "hungry" and their smelling range becomes bigger. If they can see no zebras but can smell one, they will only be informed of one of the zebra's coordinates and follow it semi-blindly. 
   
3. The main simulation loop. Each round consists of the following phases: \
   a. Animals see their visible enemies and allies and choose a goal and target (avoid/chase a certain animal or mate with a certain animal) if they don't already have one. \
   b. Animals move in the direction of their target. \
   c. Collisions are tracked. 


https://github.com/user-attachments/assets/d307d28a-603c-42fe-9e33-c378d4df573b



Limitations and potential features: \
  a. Introduce deaths by old age or hunger. \
  b. Add a third element or agent to stabilize populations. \
  c. Introduce mutations.
