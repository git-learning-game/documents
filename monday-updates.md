# Week 1 (2020-09-07)

What did we do last week?

- We're starting out by building on top of a [horizontal prototype](https://github.com/git-learning-game/git-hydra) for the game we had built when writing the application.
- Investigated a technical risk: how can we trigger commit message editing from within the game? We settled on using the `EDITOR` environment variable to communicate to the game from Git via TCP...
- Implemented a simple structure for levels, with a description, and shell scripts which create a goal state and an initial state.
- Refactored out the logic that visualizes the individual repositories, so that we can draw multiple of them next to each other.
- Built a simple game view that displays the goal repository and the current repository, as well as a terminal that takes commands.

What do we plan to do this week?

- Look at another technical risk: can we bundle the game with Git binaries for multiple platforms, to make it standalone – especially for Windows?
- And another one: how can we communicate with Git processes that take input while they are running? (For example `git add -i`.)

What's blocking us?

- Nothing in sight ;)

What's motivating us?

- Seeing that hard (and maybe a bit frightening) problems can be solvend and we found technical solutions for them.
- Many people filled out our [pre-project survey](https://docs.google.com/forms/d/e/1FAIpQLScUG41naRSm_l1tg08eblze0qtNw2foMDQJP3aGqCZES6gfZw/viewform) and gave super helpful input! :)
- General excitement for finally starting with this project!
- We're planning to participate in a tradition in the indie gamedev world, where you post about your game on Saturdays, with the hashtag #screenshotsaturday. Here's our [first post with a video](https://twitter.com/blinry/status/1302175196284096512)!
