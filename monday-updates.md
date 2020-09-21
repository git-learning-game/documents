
# Week 3 (2020-09-12)

What did we do last week?

- Some polishing of the UI
- A lot of polishing of the level sequence. At this point, we have levels that explain almost all Git internals, with the exception of annotated tags \o/
- First playtesting with two experienced Git users!! Main takeaways:
  - The game seemed to work on their Linux machines, which is good. We found a small problem that seems fixable.
  - They didn't seem too annoyed with the UI or our terminal, which is good ;)
  - We definitely need a built-in documentation, because people will forget the commands we teach them quickly: a cheat sheet? A man page browser?
  - What is the motivation of people who are new to Git to play the game? Should we explain things top-down for them, starting with the commands they will actually use?

What do we plan to do this week?

- Implementing a first prototype of a "cheat-sheet" so that users can write down important commands or information
- Learn more about Godot's GUI system works in detail
- Try writing a series of high-level introduction levels?

What's blocking us?

- Not really blocking, but after this prototype, there are a lot of directions we could proceed in, and it's unclear which is best.

What's motivating us?

- The Playtests and showing first prototypes to others :)
- Working together on this project is really fun and works well. We're basically pair-programming all the time. :)


# Week 2 (2020-09-14)

What did we do last week?

- Getting the game to run on Windows! This was something that seemed difficult, and which we wanted to get out of the way. Fortunately, just plugging in the portable version of the Git Bash instead of /bin/bash seemed to work pretty immediately. :)
- Implementing "win conditions" for levels. They are simply bash scripts that are run on a repo and either exit with code 0 or 1. This mechanism allows us to have a [playable level sequence](https://twitter.com/blinry/status/1304685656405409792).
- When considering which dependencies which we can build on, we found that because Git depends on Perl anyway, we will always have Perl. This will be useful for writing little helper scripts, and we switched our "fake editor" to Perl.
- Wrote [one of the prettiest lines of code](https://github.com/git-learning-game/git-hydra/blob/master/shell.gd#L49) of our lives... This is a workaround for an unfortunate quoting behaviour on Godot's side, but should fix the problem.

What do we plan to do this week?

- How can we communicate with Git processes that take input while they are running? (For example `git add -i`.)
- Polish level texts and appearance a bit, so that we can show it to the very first alpha testers! :O

What's blocking us?

- Working with a Windows VM is *not pleasant*, and really slow. blinry might want to install Windows on a real machine.

What's motivating us?

- Getting uncertain technical problems out of the way first feels good and the project overall feels more doable :)
- We're looking forward to the very first test runs! Curious what people might say, and whether the game will work for them!


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


# Week (2020-)

What did we do last week?

What do we plan to do this week?

What's blocking us?

What's motivating us?