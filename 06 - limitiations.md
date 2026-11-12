# Limitations
A lot of the limitations of the current implementation of the project are listed as addressable items either in the Implementation plan or in the Backlog, but namely some that come to mind they may or may not be on there are

- The use of specific hard-coded travel sites for search. Ideally would love this to be configurable
- The turn by turn logic is heavily coded deterministically instead of relying on the LLM to handle the conversation flow.   
  Right now LLM usage is just restricted to trip goal extraction based solely on what the user has typed in the chat message history.  
  That's fine for now, but there's a lot of deterministic code in run_turn that should really be handled by the LLM itself
- Having a complete workflow of finding flights, then stays, then activities and transportation is the ultimate goal, but we're not there yet
- Nuances on query requests like by the beach or near a point of interest aren't really handled
- There is some stored preferences in the app somewhere that can be manually altered, but there at some point should be some the ability to learn the tastes of the user so that the app becomes more personalized
- Ultimately the goal of this project was to make the user have to make less clicks or provide less information so little things like alreadying knowing the user's origin - i think the app hard defaults to orlando right now, and also probably defaulting the search to the next 30 days if no date is specified would be a little bit delightful
- Lastly having at least the booking links in a clean fashion some where the user can access them to book the trip all at once would be a gold feature if that's even possible. I'm not saying for the app to handle the booking for the user because that would be sort of a diamond feature, but at least getting all the links in one place and allowing the user to one by one handle the manual booking process on their own would be a nice next bridge step