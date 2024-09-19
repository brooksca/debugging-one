# Debugging Challenge: One

This is the first in a set of challenges designed to improve debugging skills in cloud and containerized applications. Debugging, curiosity, and critical thinking are incredibly hard skills to coach and refine without practice. Debugging challenges are designed to give an environment that fosters critical thinking and a curious mind.

This challenge is comprised of a server application (using ASP.NET Core) and a client application (using Next.js 14) that are unable to talk to one another. The server application has a single endpoint, `/code`, that returns an object with a single property, cleverly named `code` (can be found in `server/src/Program.cs` line 19).

When the applications are communicating properly, the value of the `code` property will be displayed as a third item in the next.js home page at [http://localhost:3000](http://localhost:3000), just below `2. Save and see your changes instantly`.

The objective is to ensure the client application can successfully retrieve data from the server and in doing so, adding a third item to the main page.

## Running the project

To run the project, all that's required is opening your terminal and `cd`ing into the root directory of the project and executing `docker compose up`. This will start both the API and the UI on ports `5001` and `3000`, respectively.

Both the server and client applications have hot reload enabled (although the .NET application is finicky).

## Requirements

1. [Docker Desktop](https://docs.docker.com/engine/install/)
