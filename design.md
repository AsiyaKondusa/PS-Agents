# PS-Agents
**Question 1**:Design the agent using the PEAS framework and further define its environment 
using the 5 definitions of agent environments,

PEAS FRAMEWORK
1.Performance measure – Fuel efficiency, least travel time, best route, safety of the cargo, condition of the cargo on arrival, accuracy of getting to the right destination. 
2.Environment: road types, traffic, pedestrians, weather, signposts, other vehicles like bikes, cars
3.Actuators: steering wheel, accelerator, brake, horn, signals 
4.Sensors: GPS, speedometer, sonar/radar, cameras

5 DEFINITIONS OF AGENT ENVIRONMENT
1. Partially observable - Information about the environment is not fully available to the agent.It must make informed guesses about world. A trailer cannot see behind other trucks or around bends due to sensor limitations.
2. Stochastic - Environment has variety of aspects beyond the control of the agent. Other people driving and weather suddenly changing from sunny to rainy which is beyond the control of the self driving trailer
3. Dynamic - Dynamic means the world changes while the agent is deciding - While the trailer decides to take a turn, a pedestrian suddenly crosses the road, or a bike appears from nowhere which would require the trailer to brake suddenly.
4. Multiagent - The agent is operating with other agents in the environment. Other bikes and cars each move differently and are heading to their destinations at different speeds
5.Sequential - Choice of action by agent is dependent on previous actions- To get to Nyahururu, one can choose different routes like A014 to B5 or A3 to B7 to B6 then B5. The route it chooses will determine which roads and junctions it encounters next, influencing its previous actions until it reaches its destination. 

   
