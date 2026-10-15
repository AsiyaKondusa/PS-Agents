# PS-Agents
**Question 1**:Design the agent using the PEAS framework and further define its environment 
using the 5 definitions of agent environments,

PEAS FRAMEWORK
1. Performance measure – Fuel efficiency, least travel time, best route, safety of the cargo, condition of the cargo on arrival, accuracy of getting to the right destination.
2. Environment: road types, traffic, pedestrians, weather, signposts, other vehicles like bikes, cars.
3.  Actuators: steering wheel, accelerator, brake, horn, signals
4.  Sensors: GPS, speedometer, sonar/radar, cameras

5 DEFINITIONS OF AGENT ENVIRONMENT
1. Partially observable - Information about the environment is not fully available to the agent.It must make informed guesses about world. A trailer cannot see behind other trucks or around bends due to sensor limitations.
2. Stochastic - Environment has variety of aspects beyond the control of the agent. Other people driving and weather suddenly changing from sunny to rainy which is beyond the control of the self driving trailer
3. Dynamic - Dynamic means the world changes while the agent is deciding - While the trailer decides to take a turn, a pedestrian suddenly crosses the road, or a bike appears from nowhere which would require the trailer to brake suddenly.
4. Multiagent - The agent is operating with other agents in the environment. Other bikes and cars each move differently and are heading to their destinations at different speeds
5. Sequential - Choice of action by agent is dependent on previous actions- To get to Nyahururu, one can choose different routes like A014 to B5 or A3 to B7 to B6 then B5. The route it chooses will determine which roads and junctions it encounters next, influencing its previous actions until it reaches its destination. 

   
# Question 2:
## Developing a suitable directed graph and search tree
# Nairobi to Kisumu Distances

## Route 1

Nairobi → Naivasha → Nakuru → Kericho → Kisumu

| From     | To       | Distance |
|----------|----------|----------|
| Nairobi  | Naivasha | 91 km    |
| Naivasha | Nakuru   | 71.0 km  |
| Nakuru   | Kericho  | 107.0 km |
| Kericho  | Kisumu   | 84.0 km  |

## Route 2

Nairobi → Naivasha → Nakuru → Eldoret → Kisumu

| From     | To       | Distance |
|----------|----------|----------|
| Nairobi  | Naivasha | 91.0 km  |
| Naivasha | Nakuru   | 71.0 km  |
| Nakuru   | Eldoret  | 156.0 km |
| Eldoret  | Kisumu   | 138.0 km |

## Route 3

Nairobi → Narok → Bomet → Kisii → HomaBay → Kisumu

| From    | To      | Distance |
|---------|---------|----------|
| Nairobi | Narok   | 143.0 km |
| Narok   | Bomet   | 81.0 km  |
| Bomet   | Kisii   | 82.4 km  |
| Kisii   | HomaBay | 52.0 km  |
| HomaBay | Kisumu  | 108.0 km |

## Route 4

Nairobi → Narok → Bomet → Litein → Kericho → Kisumu

| From    | To      | Distance |
|---------|---------|----------|
| Nairobi | Narok   | 143.0 km |
| Narok   | Bomet   | 81.0 km  |
| Bomet   | Litein  | 44.1 km  |
| Litein  | Kericho | 32.0 km  |
| Kericho | Kisumu  | 84 km    |


Directed Graph:
<img width="958" height="1097" alt="Directed_Graph_Nairobi-Kisumu" src="https://github.com/user-attachments/assets/85dd4143-ab9d-4082-ae42-1f685840b683" />


# Question 3:
## Determine the optimal path the trailer can take from Nairobi to Kisumu & Calculate the distance between towns

### Route 1: Nairobi → Naivasha → Nakuru → Kericho → Kisumu
path cost function = 91 + 71.0 + 107.0 + 84.0 = 353.0km

### Route 2: Nairobi → Naivasha → Nakuru → Eldoret → Kisumu
path cost function = 91.0 + 71.0 + 156.0 + 138.0 = 456.0km

### Route 3: Nairobi → Narok → Bomet → Kisii → HomaBay → Kisumu
path cost function = 143.0 + 81.0 + 82.4 + 52.0 +108.0 = 466.4km

### Route 4: Nairobi → Narok → Bomet → Litein → Kericho → Kisumu
path cost function = 143.0 + 81.0 + 44.1 + 32.0 + 84.0 = 384.1km

## optimal path conclusion:
In conclusion after comparing all possible routes, route 1 yields the lowest path cost at 353.0km. Therefore, the optimal path selected by the self-driving trailer agent is:
Nairobi → Naivasha → Nakuru → Kericho → Kisumu

## Group Photo
![Group Photo](https://github.com/AsiyaKondusa/PS-Agents/blob/cadd85c368a9e91b1861798cccb7214a913babce/WhatsApp%20Image%202026-10-15%20at%203.21.57%20PM.jpeg)
