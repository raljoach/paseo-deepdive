# Folder Structure
To keep things very simple I'd like to think of Paseo first in terms of folder structure.  
```
paseo/  
│    
├── backend/    
│   ├── flights   
│   └── stays
│
├── frontend/
│   └── chat
│
└── README.md
```

I'm keeping it minimal for now, but in the future this folder structure probably will expand.    


# FAST
The best way I would like think of the Paseo architecture is it's **FAST**

F - flights  
A - activities  
S - stays   
T - transportation  

I know in the above ***folder structure*** I kept it simply flights and stays but for a true complete 
*trip planner* (and this is the realm we're getting into)   
we're going to need to add activities and transportation to the itineraries we're going to generate   
such that users have a complete picture of getting from home to their destination and also    
have things to do while on vacation or travel rather.    

What actually goes under flights, stays, activities, and transportation folders will change over time.   
For now you can think of each subfolder containing a service that supports a chat interface.

I kept the front-end simply a chat for many reasons, one being that it's the way most modern agentic   
platforms start and also it can be incorporated or integrated into any existing UI surface and it's    
easily testable.
