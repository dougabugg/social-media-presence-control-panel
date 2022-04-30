# Architecture

The main app will run and display a webview window with a custom page when invoked. The custom page will enable setting up various data sources, like twitter, instagram, youtube, twitch, facebook, etc. it will be handled by the main app injecting a probe into the page, which enables the main app to pass messages and commands between the primary page (that initial custom view).
