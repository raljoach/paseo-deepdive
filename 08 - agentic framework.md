# Agentic Foundations
Tools, Algorithms, Roles, Pipelines/Workflows/Chat
Multi-Agent: A2A, Supervisor vs Swarm

# Agentic Design: Swarm
Flight Agent - 1st node
Stay Agent - 2nd node

create_react_agent:LangGraph
add_edges, add_nodes
start -> flight_agent_node
compile
query

# Agentic Design: Supervisor
Planner Agent - Your a travel planner and [you're connected these tools] and you're job is create the best itinerary   
based on the follow user trip creation request. You should extract the trip goal into structured json containing 
key information such as origin, destination, start date, end date, number of travelers/guests, etc etc so on and so forth
An itinerary consists of flights, stays, activities, and transportation and the best itinerary meets the user's trip
request goal which may include constraints (ie budget, availability dates for travel) and preferences (ie proximity, point of interest, travel distance, time of day for travel, location, types of things to do, vibe, etc etc so on and so forth)

Flight Agent - Your job is to search for flights based on specific parameters such as   
origin, destination, start date, end date, flight type: 1 way vs round-trip, etc etc so on and so forth
and rank flight results according to [tool, algorithm] and you have at your disposal numerous flight providers to compare
flight prices and choose the best one meeting the user trip goal request goal which may include constraints (ie budget, availability dates for travel) and preferences given to you


crew=[planner_agent, flight_agent, stay_agent]
crew.invoke(query | prompt | llm)