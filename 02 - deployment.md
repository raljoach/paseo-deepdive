# Deployment
We're going to keep deployment simple. In the past I've used Hugging Face Spaces to deploy my front-end and I've used Render.com to deploy the backend. This worked when i was creating a simple iterative REPL version of Paseo to gain feedback from test users using Gradio as a quick rapid frontend prototype and then have a backend service for the business logic which I hosted on render.com which gave the benefits of checking on health status. For scrappy hacking it worked fine and at this moment I'm inclined to continue to use this approach if it works. I also used Gemini free api models for any agent development but haven't tried deploying them as a backend on render.com. That's to be explored.

Of course over time this will have to turn into a more sophisticated CI/CD pipeline, maybe run on Google Cloud or AWS.
For now, we'll build that as we go with scripts and as much small scale automation that we can without overburdening ourselves.

1 script start platform would also generally be nice or just a nice set of instructions in a README.

Containers? Docker? Not sure that's necessary unless the platform that hosts the app requires it.