<div style="text-align:center"><img width="643" alt="referential" src="https://user-images.githubusercontent.com/4453806/89699745-901f2e00-d8ee-11ea-94f3-a70f79825923.png"></div>

REPLs and Browsers and Friends, oh my!

## Problem we're starting from

Terminals are fast and powerful. But it's too hard and time-consuming to get data into and out of them, and too hard to share results and sessions in them.

What happens if we totally eliminate the barriers between terminals, browsers, and social communication and sharing?

## Background

Terminals and terminal emulators, unlike the shells that run inside them and the operating systems they interact with, are a relatively unchanged and untouched part of the modern development stack. As with character encodings before the standardization and adoption of Unicode, when you configure or debug a terminal, layers of old protocols and accreted, outdated hacks peek through, like ancient geological strata on a cliff face. They are incredibly powerful and fast in the hands of a knowledgable user, but they are also hard to learn and configure because of this history. Most importantly for the purposes of this project, they are increasingly hard to use in conjunction with other more modern data sources and tools, and on fast-moving teams in constant communication.

Terminals were invented when computers were room-sized, rare, and batch-oriented. They allowed users to access this resource in parallel and remotely, with keyboards instead of punch cards and switches: a major advance in the economics of computing. Since terminals where invented, though, computing and its applications have gone through several massive revolutions: personal computers, the internet, social networks, mobile computing, and cloud. Computers are cheap, small, everywhere, and we interact with them all the time to access information and communicate with other people. Terminals remain the most powerful and fastest tool for one-player "power user" operation of commands over files and bytes on a single computer, but the distance between that experience and the interactive apps and data on the web, the distributed and cloud systems we build to run them, and the social networks we leverage to develop and distribute those apps, makes the impedance between these systems and the terminal quite high!

**referential** is a project that explores what happens when you eliminate as many barriers to interoperation between the terminal, the browser, and team/social interaction as is feasible. It does so by simply putting these three interfaces together into a single app. The interaction model of each constituent app remains the same: power user text UI in the terminal, exploration by search and navigation in the browser, and status updates and quick video/text communication in the social pane. **referential** borrows the fundamental interaction paradigm from modern graphical user interfaces to facilitate far easier and more useful sharing _between_ these interfaces: select and drag. When you drag a selection from any of these interfaces into another, **referential** reflects the data, computation, or social interaction into the other interface in an immediately useful way.

**referential** brings people (social), computers (terminal), and problems/data (browser) together with a single interaction model to enable fast, cloud and internet-connected, team-first computing.

### Translations

As we select and drag data, computational expressions, and even people between these different paradigms, we have to interpret them in the new context to be most immediately useful. **referential** calls these adaptations **translations**, and there are `3!` = `6` of them:

- **Browser ➡️ Terminal**: turn the content into data structures in the currently running language environment, or into a local file if in top level shell.
- **Browser ➡️ Friends**: share the page, the currently highlighted content, and optional comments with your friend(s).
- **Terminal ➡️ Browser**: deploy the current session, file, or codebase to a shareable repl.it, Gist, or deployment
- **Terminal ➡️ Friends**: fork and share the session with your friend(s)
- **Friends ➡️ Browser**: invite your friend(s) to a shared browser session (plutoview?)
- **Friends ➡️ Terminal**: invite your friend(s) to a shared terminal/editing session (repl.it or Live Share?)

**TODO**: Think about other interaction sets that may be best:
- do fewer translations make sense (maybe terminal is always bound to a webpage and sharing/inviting is over both of those in tandem)?
- do more make sense (⊆ of the directed _hyper_graph, including self-edges to fork or record entire **referential** sessions)?

### Mockup

Behold!

<div style="text-align:center"><img width="643" alt="referential" src="https://user-images.githubusercontent.com/4453806/89699787-eb512080-d8ee-11ea-9e1b-ac07f9e8be51.png"></div>

Project theme song: https://www.youtube.com/watch?v=4JkIs37a2JE
