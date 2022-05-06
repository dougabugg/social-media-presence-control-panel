# social-media-presence-control-panel
An applicaiton for managing social media presence on multiple platforms

# Project Viability

It is not uncommon for me to start a project, but run into a roadblock, and lose interest in working on the project for a time. This project is no different. I guess the roadblock that hit me the hardest was how "viable" this project would be. The current path I was heading down, I was effectively trying to reimplement [selenium](https://en.wikipedia.org/wiki/Selenium_(software)) using a webview and some hacky javascript. I might still be able to make a working prototype this way, but I'm not convinced it will be a good path forward for the project in the long term.

Another idea I had was to build a framework to allow the user to "record" their interactions with any website, and then "play back" and customize certain aspects of the interaction in an automated fashion later. I think this is a lot more viable and useful; if a website changes their layout and breaks the automation, users don't need to wait for an update or patch to be released by a developer, they simply need to "re-record" any interactions that "broke".

So the scope of this "super project" is much larger than this project; my goal now is to build a tool for automating arbitrary interactions on websites for sending and collecting data. Such a project might not benefit from a simple webview, but a full fledged user agent, like [servo](https://en.wikipedia.org/wiki/Servo_(software))

# (previous musings)

## What's the roadmap?

The high level roadmap is first to design/document and then build web scrapers to grab data from various social media websites, and present all that data in various forms for further processing and inspection.

Web scrapers can break if the website starts outputting new HTML that doesn't match the form we built the scaper to parse, so we might want to fall back on an API or something. API set up could be partially supported from within the UI.

Next, we can to build tools for inspecting and organizing the data, and finally an interface that allows the user to customize this pipeline and see the results quickly (latency hopefully minimized).

## What are some potential road blocks?

For starters, I was looking at twitter. They have an official API, but it's geared more towards enterprise.

see links
- https://developer.twitter.com/en/docs/twitter-api/migrate/twitter-api-endpoint-map
- https://developer.twitter.com/en/docs/twitter-api/getting-started/about-twitter-api

I'm tempted to build a web scraper that operates by hitting the same API endpoints the twitter web app uses. That way, we can access "Tweet Analytics" for impressions and such.

Also, I should reconfirm the goal of the project with the client.

After reading the initial pitch that got me interested in working on this, it looks like the main goals I should be focusing on are automation of the scheduling and posting of content, supporting multiple social media platforms, and also grabbing notificaitons and direct messages from each platform.

## Update on backend

I plan on developing on my current OS/Desktop Env, which is win10 currently.
Right now, I'm reviewing documentation https://docs.microsoft.com/en-us/microsoft-edge/webview2/reference/win32/icorewebview2

## Aside

I realized after I made this repo, I had another repo named `social-media-detective-toolkit`, but I never made any progress. If I'm remember correctly what I meant for that project to be, this project is actually larger in scope, and implementing the detective toolkit on top of this presence control panel would be trivial once this project is operational.
