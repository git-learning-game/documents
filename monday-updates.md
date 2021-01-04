# Week 18 (2020-01-04)

**What did we do in week 16?**

- Made a big master plan of everything we still want to do, and assigned the things to weeks. Seems like quite a lot of work, but doable, and we have two unplanned buffer weeks :)
- Implemented a general "hint" system
- Extended the level format so that goals can have multiple components, which are displayed
- Built a general "trigger-action" system, so that we can build more interactive levels – a "friend" who reacts when you push to their repository, for example
- Built a simple title screen and level picker. It's still ugly, but it works!
- Sent out a talk submission to FOSDEM

**What do we plan to do this week?**

- Cover all the things we want to teach in the game with simple test levels
- Optimize the screen layout
- Remember which levels are solved in a "savegame", and mark them green or something
- Different levels: cards vs terminal
- Sandbox mode with all cards
- Organize playtests for next week

**What's blocking us?**

- We can't think of anything :P

**What's motivating us?**

- The master plan makes it easy to know what to work on when
- Looking forward to the next playtest!



# Week 16 (2020-12-21)

**What did we do last week?**

- Call with y'all! :)
- Looked at [PuzzleGraph](https://runevision.itch.io/puzzlegraph) for inspiration of which mechanisms we could use
- Had a long brainstorming about all different variations our 2D world could have, and sketched some levels in ASCII style. It's hard to find a balance between an exciting world and not straying too far away from Git.
- In particular, because we still want the player to be able to use the command line to solve the puzzles, we'd have to prevent certain types of "cheating", where the player can just edit or copy files.
- Having a "2D world" seems promising because it would often allow us to have very clear goals for the levels - "get to the exit", for example. In the current version, the goals are a bit more fuzzy - "make a merge that results in a file which has these specific properties". But for some concepts we want to teach, we didn't really find good rules/levels that enforce that the player uses Git in a specific way.

**What do we plan to do this week?**

- We'll take some time today to build a roadmap for the last two months!
- What we'll do today will depend on that. :D

**What's blocking us?**

- We've been doing some conceptual work in the last weeks - because we're thinking about what the next steps are, we can't work efficiently on implementing them, but we think that's okay. :)

**What's motivating us?**

- Having some cozy days around Christmas :D


# Week 15 (2020-12-14)

**What did we do last week?**

- Vacation \o/

**What do we plan to do this week?**

- Think of a few 2D puzzle mechanisms, implement them, play around with them to see what's fun
- Submit a lightning talk to FOSDEM, which has finally opened submissions :)

**What's blocking us?**

- Nothing in sight :)

**What's motivating us?**

- Curious what we'll think of the current status when we look at it with fresh eyes :)
- Requested the first payout today :D

# Week 14 (2020-12-07)

**What did we do last week?**

- We played [5D Chess With Multiverse Time Travel](https://store.steampowered.com/app/1349230/5D_Chess_With_Multiverse_Time_Travel/) to see how they solved some GUI problems that are similar to our cases.
- Thought some more about what the rules in the 2D world should be like. Looking for a balance between making it simple and interesting.

**What do we plan to do this week?**

- We're on "vacation" this week, except for the call! :)

**What's blocking us?**

- Still not super clear where to go next. We have some ideas, but might schedule another coaching?

**What's motivating us?**

- blinry notices that a planned vacation is really nice! Hasn't done that in a while.

# Week 13 (2020-11-30)

**What did we do last week?**

- Brainstormed on a high level about how a "2D world" would work and what you could do in it. There might be levels about unlocking a chest with a key, and the key is actually a GPG key?! :D
- Thought about which incentives we could have for moving from the visual playing card interface to the command line. Commands like "rm *" might be well-suited, because they demonstrate the power of the command line?
- Thought about high-level game structure: there might be two alternating styles of levels: the ones in which you learn new Git stuff in an "official" setting from your teachers, and can use the playing cards. And then, you get levels where you need to apply your new knowledge in a different, more personal setting - maybe playing pranks on people, being sneaky and tricky - and this is where you can use the command line to "trick" the game.
- Created an inventory to take files through time \o/

**What do we plan to do this week?**

- Drag & Drop item combination
- Try building a few levels with what we have, see what already works and what's missing
- Look for inspiration on how the 2D world can work or look like

**What's blocking us?**

- Godot's GUI nodes still feel cumbersome to use. We need a lot of time to wrangle with them, which is time we'd rather spend on making actual content for the game...

**What's motivating us?**

- We saw [this tweet](https://twitter.com/round/status/1331693653740322816) about a 5-dimensional chess game, and someone mentioned that there should be a Git UI like this. That was a really good moment to plug our game, and people seemed interested!


# Week 12 (2020-11-23)

**What did we do last week?**

- Fixed MacOS crash caused by a non-existent option for 'sed'
- Creating a 2D scene for more fun interaction with files. The player can walk around and create/delete/manipulate objects that represent files.
- Show a combined view of the working directory, of the index, and of the last commit, with halos: the current files are white objects, the index versions are blue halos, the last commit is a faint shadow. Seems like a promising way to build more intuition of how these three interact.
- Had an enjoyable chat with Marie, thanks for that!

**What do we plan to do this week?**

- Try adding more properties to the 2D objects (something like "what is the character saying right now?")
- Creating test-levels for the new 2D file scenes
- We're considering putting the finalized game on Steam in the end. Might look into how all of that works :)

**What's blocking us?**

- Nothing in sight ^_^

**What's motivating us?**

- bleeptrack's job at university runs out, so there's more free time and more energy :)
- Trying a new direction of having 2D objects in the game is exciting! :D


# Week 11 (2020-11-16)

**What did we do last week?**

- Playing cards can now have string parameters, which enables a number of new cool actions, like `git branch [string]` or `touch [string]`.
- Wrote some new levels, which explain how to create/delete branches, and how to work with files (create, delete, and rename them)
- Making all fonts 15% larger – this was based on feedback regarding accessibility we got.
- A friendly person opened a number of small issues in the GitHub project, we fixed them.
- Adding shader to target halos so players can better see where they can drop their card.

**What do we plan to do this week?**

- Fix MacOS crash (see github issue [#9](https://github.com/git-learning-game/git-hydra/issues/9))
- Write more levels, which explain concepts we haven't covered yet.

**What's blocking us?**

- Nothing this week :)

**What's motivating us?**

- Talk submissions to FOSDEM might open this week, we're thinking of doing a lightning talk or something. :)


# Week 10 (2020-11-09)

**What did we do last week?**

- Started working on the bug that randomly crashes the game: we removed a possible error source, but the bug is still there. :O
- The file explorer can now also show the index and indicates the current file status (new, modified, conflicted) via symbols
- We noticed that our playtesters sometimes didn't know where to drag the playing cards to run commands. We added a functionality that highlights the "valid" drag targets (commits, refs, or files), which should help with this problem.
- Current builds of the game are now automatically deployed to [itch.io](https://blinry.itch.io/git-hydra)!

**What do we plan to do this week?**

- Look some more into the random crashes. This is high priority! :D
- Write more levels that teach how to use the index. We're curious how well the playing card interface scales up when you have more cards.
- Some fancy glow effect for the drop areas.

**What's blocking us?**

- Nothing in sight :)

**What's motivating us?**

- Results of the US elections! We're pretty relieved!
- It's pretty neat that building this game helps us get a deep, intuitive understanding of Git ourselves! :)


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
- We are happy to have quite a clear view what our next steps will be. Feels good :)


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