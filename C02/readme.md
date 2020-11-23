# Web-hook to trigger rebuild

> Pre-requisites, the application created in *[Exercise 2](/exercises/A02/index.html)*

In this exercise we will set up a web to trigger an automatic build when the code in Github is changed.

* From the Builds configuration page, find the Github Web-hook URL and copy it down.

![Triggers](/img/triggerURL.png)

* Go to your forked repository in Github, in the `Settings > Web-hooks`, add a new one. Use the URL you copied, change the content type to `application/json` and save it.

* Push any change to the repository and see what happens.
