# social-media-presence-control-panel
An applicaiton for managing social media presence on multiple platforms

## What's the roadmap?

The high level roadmap is first to design/document and then build web scrapers to grab data from various social media websites, and present all that data in various forms for further processing and inspection.

Web scrapers can break if the website starts outputting new HTML that doesn't match the form we built the scaper to parse, so we might want to fall back on an API or something. API set up could be partially supported from within the UI.

Next, we can to build tools for inspecting and organizing the data, and finally an interface that allows the user to customize this pipeline and see the results quickly (latency hopefully minimized).

# Aside

I realized after I made this repo, I had another repo named `social-media-detective-toolkit`, but I never made any progress. If I'm remember correctly what I meant for that project to be, this project is actually larger in scope, and implementing the detective toolkit on top of this presence control panel would be trivial once this project is operational.