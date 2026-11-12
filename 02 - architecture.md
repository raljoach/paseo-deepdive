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
│   ├── pages/
│       └── chat
│   └── main.tsx
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

# Front-End
Inspirted by how I attempted to build Paseo using a coding ai agent (ie Claude Code Pro)   
https://github.com/raljoach/paseo-agent/blob/main/frontend/AGENTS.md   
https://github.com/raljoach/paseo-agent/blob/main/frontend/src/main.tsx
https://github.com/raljoach/paseo-agent/blob/main/frontend/src/App.tsx#L6    
https://github.com/raljoach/paseo-agent/blob/main/frontend/src/pages/chat/ChatPage.tsx#L172        

The cleanest front-end development of Paseo I've done so far in my past iterations used React as a front-end.       
If you read the AGENTS.md above, you'll see the breakdown of that front-end architecture is quite extensive,   
but it basically boils down to a main.tsx that loads an App component which for all intensive purposes      
loads a ChatPage component.


The layout for the chat page is similar to ChatGPT in that on the left side it will show Trips (represented by TripList component)     
and on the right side it will have the conversation history for the trip which is encapsulated by the Card component.
It's a very intuitive interface and follows the same pattern as most ai chat platforms.     


Starting out brand new, a user would click on New trip and they would be shown a message box on the right where they can    
enter a query to begin their trip planning.