# WHAT IS IT? #

This project simulates the activity patterns of students of University of Central Florida. The agents in this model behave based on the survey data that was gathered from more than 1000 students in the university. An agent (student) arrives at the school on certain times, goes to some locations like a department or restaurant and finally departs the campus.

Each agent has these set of defining parameters: entrance, dormitory, department, class building, arrive, depart, lunch, dinner, beverage, recreation and wellness, parking, shuttle, and miscellaneous. The first four parameters designate the single (most common) value of the agents’ entry point to the campus, housing situation, home department, and main class building. The remaining parameters are lists of locations for the agent’s dining, recreation, and commuting. Additionally, each parameter that includes a location has another matching parameter that shows the time or frequency of visiting that location. These frequencies are calculated by using statistical distributions that are fitted to the answers of designed survey questions. Statistical sampling is used in order to create the initial values for the parameters.

When the simulation commences, all the agents are initialized with parameters that remain constant over the lifetime of the agent and are used to create daily activity profiles. In our model, one tick represents one hour of activity in the real world. When the model starts, each agent runs within a loop. The loop continues until the simulation is stopped.

# HOW TO USE IT #

Like most of Netlogo projects, “Setup” and “Go” are the main buttons of the interface. Setup initializes the model and sets the value of the agents’ parameters.

Three other buttons named “link,” “junc” and “place” exist below the introduced buttons. These buttons might be used after stopping the model in order to graphically show the extent of passing roads (and walkways), junctions and the different buildings of the campus (departments, parking …). In the produced outputs bigger circles or thicker lines correspond to the roads or locations that more agents used. The five monitors on the right side of these two buttons indicate the current time of simulation or the amount of time passed after the model started. The slider on the top left side sets the number of agents/students. The number that was used for our experiments was 47000.

The remaining buttons, switches and toolboxes at the button the interface page are used for debugging purposes.

# THINGS TO NOTICE #
Since each step of running the model might require too much computation for each agent, like other complex Netlogo models, it is strongly recommended to disable graphical updates while the model is running.

Please note that the image file that is downloadable from the _Downloads_ tab, should be in the same folder (root) as the Netlogo code.

The initial procedures that exist in the code implement the set-up tasks like the way that Netlogo models work. After that, there are the procedures implanting agent’s behavior. The final procedures set the location of different buildings and roads through the imaginary graph on the map’s background. The nodes of this graph are the locations in the campus including departments, parking, dorms etc. The edges of this graph correspond to the map’s roads and walkways.

# THINGS TO TRY #

Try changing the number of agents/students and see the results.
Try running the model for different duration (the original one was 3 months), and see how the final results vary.

# CREDITS AND REFERENCES #
This research was supported in part by DARPA award N10AP20027. This project was part of a research project for building a simulator of students transportation activates performed in IAL lab of the University of Central Florida by Rahmatollah Beheshti and Dr. Gita Sukthankar.
