# Debugging Challenges

Debugging, curiosity, and critical thinking are incredibly hard skills to coach and refine without practice. Debugging challenges are designed to give an environment that fosters critical thinking and a curious mind.

The following challenges represent common problems encountered in cloud and containerized applications. Some challenges run locally with [Docker Desktop](https://www.docker.com/products/docker-desktop/) and some will require deploying to running cloud environment. These challenges will have scripts that deploy the necessary resources to your cloud of choice. To ensure you don't get an insane bill from Amazon, it's recommended to spin up the environments for only as long as someone will be working on them and then run the included destroy scripts to spin down the resources.

## Challenges

### One

Challenge one is comprised of a server application (using ASP.NET Core) and a client application (using Next.js 14) that are unable to talk to one another. The server application has a single endpoint, `/code`, that returns an object with a single property, cleverly named `code` (can be found in `server/src/Program.cs` line 19).