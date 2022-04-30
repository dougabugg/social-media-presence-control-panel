# social-media-presence-control-panel
An applicaiton for managing social media presence on multiple platforms

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


# Aside

I realized after I made this repo, I had another repo named `social-media-detective-toolkit`, but I never made any progress. If I'm remember correctly what I meant for that project to be, this project is actually larger in scope, and implementing the detective toolkit on top of this presence control panel would be trivial once this project is operational.