# Codecamp Agent Competition

This is our: "build your own bomberman agent" competion!

For [docs](https://www.gocoder.one/docs)

Requirements:

- Docker(docker desktop will be fine)
- docker-compose(for your test runs)
- Your preferred programming language
- ghrc.io login

To login to ghrc.io:

- get a token on [your github profile](https://github.com/settings/tokens) and create one
- login by using `echo '{token}' | docker login ghcr.io -u {github username} --password-stdin`

## How to run

To get started to see what you are developing you can run the following in the terminal: `docker-compose -f docker-compose.yml up --force-recreate --build`

Then your terminal will be filled with a lot of text and will finish with the text: `game over, winner is [x]` or something similar.

Congrats, you have a running agent!

## How to develop

This is a Golang agent, see [this](https://github.com/CoderOneHQ/bomberland) for available agents.
Choose your agent of preference, BUT:

- Never delete the `Dockerfile`, this is being used for distribution of the image, you can change this to the language you need
- Never delete the `replay.json` file, this is being used by the engine

See the `docker-compose.yml` file to change the opponnent your agent is facing.
Depending on how many teams, you can change the image name to `codecamp-2022-team-xx` by replacing the xx with a number(01 to 12)

Good luck on winning the winning price and/or special price!

## Leaderboard

Check [the leaderboard](https://dataworkz-nl.github.io/codecamp-2022-ranking/) for the current ranking!
