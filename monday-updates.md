# Week 9 (2020-11-02)

**What did we do last week?**
- Building Prototype 3 with lot's of polishing: horizontal level layout,
- More graphics: Symbols on the playing cards, an "avatar" in the form of a small monster instead of "HEAD"
- Restructured the high-level layout of the screen a bit
- new levels with the time travel topic
- 2 Playtests on Friday:
  - People generally seemed to like the "time travel" theme :D
  - People were a bit confused by file explorers for the working directory *and* on the commits. We might just unify them?
  - Some early feedback on how to improve accessibility - our fonts are probably way to small.
- Wrote a short [Twitter thread](https://twitter.com/blinry/status/1322544265629782018) with a gameplay video and links to all the resources

**What do we plan to do this week?**

- We have a strange bug that occasionally crashes the game - without any clear error messages. We need to find and fix it! :D
- Visualizing Card Targets
- How could we extend the level format to allow hints during the level?

**What's blocking us?**

- Nothing factual, just some virus and election anxiety?

**What's motivating us?**

- We seem to be on a good path, according to feedback from our beta testers!
- We are happy to have quiate a clear view what our next steps will be. Feels good :)


# Week 8 (2020-10-26)

**What did we do last week?**

- A lot of debugging on Widows :D Had a very stubborn bug, but we found it in the end. The game *almost* runs on Windows again, just need to solve another problem related to command execution.
- Visual File Explorer for a nice graphical representation of different commit states, of the index, and of the working directory. This should be much more beginner-friendly!
- Wrote a short sequence of levels where the player is a time travel agent and can help solve temporal paradoxes. We thing this approach is promising: it very quickly makes you focus on the *content* of commits, which, in the end, seems quite important.
- Failed to find people for playtesting this week, but we found at least one for this week.

**What do we plan to do this week?**

- Playtest on Friday
- Polish Timetravel Levels, maybe add a few advanced ones
- Improve the playing card system, to more closely integrate it with the level sequence

**What's blocking us?**

- Some University deadlines, but they are over at the end of October :)

**What's motivating us?**

- Playtests \o/

# Week 7 (2020-10-19)

**What did we do last week?**

- Implemented a "playing card" interface, inspired by games like Hearthstone: each card contains a command, like "git push" or "git checkout", and if you drag it into the game (or on a commit), it is executed. Definitely fun for ourselves to play with! We are not sure yet whether this is an interface we'll really use, but it could be neat to be able to give new cards to players as a reward - "here's your git push -f card" :3
- Recorded [Dev-Log #2](https://youtu.be/w3oEKqKMQOc)
- Wrote as good as a [README](https://github.com/git-learning-game/git-hydra/blob/main/README.md) as we could, which describes installation instructions, and how to contribute!
- Added the [Contributor Covenant](https://www.contributor-covenant.org/) and the [Blue Oak Model License](https://blueoakcouncil.org/license/1.0.0).
- Made our first payment request.

**What do we plan to do this week?**

- Building new levels in the "time travel" theme
- Test whether the game still runs on Windows, probably make slight tweaks, have our CI produce Windows builds
- Plan and do a new round of playtesting!

**What's blocking us?**

- Virus-related anxiety :(

**What's motivating us?**

- The prospect of having people playtest is always motivating to get the game into a more polished state! :)


# Week 6 (2020-10-12)

**What did we do last week?**

- Tested the game on macOS, and made some tiny changes that allow it to run there!
- Automatically compile executables and deploy them to github pages
- Add some missing shortcuts for convenience, like Ctrl+S for saving a file, and Ctrl+W for deleting the last word.
- We had our first coaching session with John from Zero360 \o/ Main takeaway: He motivated us to try more graphical interface systems for interacting with Git repos, like something block-based, which would be friendlier to people who are really new to the command line. Maybe we can then gradually transition to a "pure" command line UI?

**What do we plan to do this week?**

- Experimenting with graphical UIs
- Decide on a license :) We tend towards something pretty permissive?
- Finish up some documentation.
- Record a new dev (v)log, and invite people to try to build their own levels

**What's blocking us?**

- Nothing in sight ^_^

**What's motivating us?**

- Getting the game to run on macOS was surprisingly straightforward! :)
- looking forward to play with fancy GUI stuff


# Week 5 (2020-10-05)

**What did we do last week?**

- Thought a bit about possible other game modes, like a "deck building" game, where you play cards that say "git reset --hard HEAD", for example. :P
- Added the possibility to split levels into "chapters".
- Implemented a new level format, which should make it easier to write new levels - for ourselves, and for people who want to contribute!
- Clever node positioning to get better graph layouts.
- Command line switch to start sandbox mode in one of your own projects (git-hydra --sandbox=.)
- A lot of code refactoring, to make it more maintainable.

**What do we plan to do this week?**

- Documentation! Add a README, a license, and a CoC to the project, and explain how to contribute code and levels.
- Probably fix a lot of bugs along the way. ;P
- We plan to be able to invite community-contributed levels by the end of the week.
- Check out how to bundle git with our godot game on Linux to ship it with a current git version.

**What's blocking us?**

- How to balance learning and fun? The coaching this month might help get us more insights.
- We didn't make progress on allowing interactive commands (like `git add -p`). It's lingering in the backs of our heads a bit.

**What's motivating us?**

- Looking forward to a next gameplay session and user generated levels :D
- We're excited about giving the game better visuals – might go in the direction of a solarpunk aesthetic?
- The realization that interactive rebasing... just... works already!


# Week 4 (2020-09-28)

**What did we do last week?**

- We built a file explorer, so players can better understand how their repository folder changes
- Started building a simple autocompletion mechanism, which should help players remember Git subcommands
- Learned more about how Godot's UI system works, polished the appearance a lot and started building a simple "theme"
- We recorded a first Dev-Log video where we show and talk a bit about our progress: [Dev-Log #1](https://youtu.be/bXERJIZnaXg)
- Built a "sandbox mode" with just a terminal and a visualization, which is optimized to record simple explainer videos. In a first example, we talk about what [git replace](https://www.youtube.com/watch?v=gHFnEylQP4k) does.

**What do we plan to do this week?**

- Plan which features we want to include in the second prototype.
- Sketch some new ideas for how puzzles and levels could work.
- Continue improving the autocomplete feature.

**What's blocking us?**

- Interactive commands are tricky to implement in our terminal. We tried different approaches and have a somewhat working version, but are not yet completely satisfied with the result.

**What's motivating us?**

- Seeing interest in the dev-log video was nice! We got a few new people interested in doing playtesting, as well as our first (very valid) [issue](https://github.com/git-learning-game/git-hydra/issues/1).
- We're generally really interested in learning about all the obscure features of Git ourselves! :)


# Week 3 (2020-09-12)

**What did we do last week?**

- Some polishing of the UI
- A lot of polishing of the level sequence. At this point, we have levels that explain almost all Git internals, with the exception of annotated tags \o/
- First playtesting with two experienced Git users!! Main takeaways:
  - The game seemed to work on their Linux machines, which is good. We found a small problem that seems fixable.
  - They didn't seem too annoyed with the UI or our terminal, which is good ;)
  - We definitely need a built-in documentation, because people will forget the commands we teach them quickly: a cheat sheet? A man page browser?
  - What is the motivation of people who are new to Git to play the game? Should we explain things top-down for them, starting with the commands they will actually use?

**What do we plan to do this week?**

- Implementing a first prototype of a "cheat-sheet" so that users can write down important commands or information
- Learn more about Godot's GUI system works in detail
- Try writing a series of high-level introduction levels?

**What's blocking us?**

- Not really blocking, but after this prototype, there are a lot of directions we could proceed in, and it's unclear which is best.

**What's motivating us?**

- The Playtests and showing first prototypes to others :)
- Working together on this project is really fun and works well. We're basically pair-programming all the time. :)


# Week 2 (2020-09-14)

**What did we do last week?**

- Getting the game to run on Windows! This was something that seemed difficult, and which we wanted to get out of the way. Fortunately, just plugging in the portable version of the Git Bash instead of /bin/bash seemed to work pretty immediately. :)
- Implementing "win conditions" for levels. They are simply bash scripts that are run on a repo and either exit with code 0 or 1. This mechanism allows us to have a [playable level sequence](https://twitter.com/blinry/status/1304685656405409792).
- When considering which dependencies which we can build on, we found that because Git depends on Perl anyway, we will always have Perl. This will be useful for writing little helper scripts, and we switched our "fake editor" to Perl.
- Wrote [one of the prettiest lines of code](https://github.com/git-learning-game/git-hydra/blob/master/shell.gd#L49) of our lives... This is a workaround for an unfortunate quoting behaviour on Godot's side, but should fix the problem.

**What do we plan to do this week?**

- How can we communicate with Git processes that take input while they are running? (For example `git add -i`.)
- Polish level texts and appearance a bit, so that we can show it to the very first alpha testers! :O

**What's blocking us?**

- Working with a Windows VM is *not pleasant*, and really slow. blinry might want to install Windows on a real machine.

**What's motivating us?**

- Getting uncertain technical problems out of the way first feels good and the project overall feels more doable :)
- We're looking forward to the very first test runs! Curious what people might say, and whether the game will work for them!


# Week 1 (2020-09-07)

**What did we do last week?**

- We're starting out by building on top of a [horizontal prototype](https://github.com/git-learning-game/git-hydra) for the game we had built when writing the application.
- Investigated a technical risk: how can we trigger commit message editing from within the game? We settled on using the `EDITOR` environment variable to communicate to the game from Git via TCP...
- Implemented a simple structure for levels, with a description, and shell scripts which create a goal state and an initial state.
- Refactored out the logic that visualizes the individual repositories, so that we can draw multiple of them next to each other.
- Built a simple game view that displays the goal repository and the current repository, as well as a terminal that takes commands.

**What do we plan to do this week?**

- Look at another technical risk: can we bundle the game with Git binaries for multiple platforms, to make it standalone – especially for Windows?
- And another one: how can we communicate with Git processes that take input while they are running? (For example `git add -i`.)

**What's blocking us?**

- Nothing in sight ;)

**What's motivating us?**

- Seeing that hard (and maybe a bit frightening) problems can be solvend and we found technical solutions for them.
- Many people filled out our [pre-project survey](https://docs.google.com/forms/d/e/1FAIpQLScUG41naRSm_l1tg08eblze0qtNw2foMDQJP3aGqCZES6gfZw/viewform) and gave super helpful input! :)
- General excitement for finally starting with this project!
- We're planning to participate in a tradition in the indie gamedev world, where you post about your game on Saturdays, with the hashtag #screenshotsaturday. Here's our [first post with a video](https://twitter.com/blinry/status/1302175196284096512)!


# Week (2020-)

**What did we do last week?**

- 

**What do we plan to do this week?**

- 

**What's blocking us?**

- 

**What's motivating us?**

- 