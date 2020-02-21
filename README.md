# Welcome to Project Yolo

It's going to be bold. It's going to be daring. It might even be a little bit sexy. This is the kind of project you make when you-only-live-once. Buckle up.

## Collaborating

The toughest part about this jam (I think) is going to be collaborating across distance and time. I've tried to get the whole back-end set up, so that we can all just jump in and start working. We're going to be using two tools to collaborate:

* GitHub: It's the website you're on right now (and we'll be using the page you're on now). It runs on a program called '[git](https://git-scm.com/)' that is basically just advanced version control. *All of our game files (code, art, levels, etc.) will live here*, and it will serve as a central place to push updates you make and to pull updates that other people make. More on that later.
* Discord: All of our communication should go through here. No need to F* with text, Whatsapp, or anything else. [Go to the server.](https://discord.gg/U2nmZJV)

Note: If anyone has suggestions about how to organize better, make them. That's part of collaborating, too.

## Getting Started

1. Install Unreal Engine 4

This is the engine we're going to be using. You can install it [here](https://www.unrealengine.com/en-US/?sessionInvalidated=true). Make sure to install version **4.24**. *Tip:* It will run faster if you install it on a solid state drive, if you have one, but it will take up a huge chunk of that drive (~40-50GB).

2. Install GitHub for Desktop

This is a desktop client for GitHub that will make it easier for you to pull/push game changes. You can install it [here](https://desktop.github.com/).

3. Clone the project repository to your local computer

Near the top of this page, there's a green button that says 'Clone or download.' Click that and then click 'Open in Desktop.' It should clone the project to your local computer. *Test:* By this point, you should have everything you need to start developing. Confirm by double-clicking the *ProjectYolo.uproject* file in your project folder (or open from the Epic Games Launcher->Unreal Engine tab). Your Editor should open up to a level with two chairs.

4. *Bonus*: Install Steam and keep it running in the background

In case we want to add online multiplayer functionality (not necessarily needed), Steam is the best platform to facilitate that. In particular, Steam's servers let you play cross-platform, so we could test games between PC's and Mac's at the same time.

## Using GitHub to stay up-to-date

Installing GitHub and downloading the project for the first time is only the first step. Next, you have to learn how to keep the project synced with your changes and everyone else's. You'll run into two basic scenarios:

* *Someone else changed the project*: Press the 'Fetch Origin' button to *pull* down changes that other people made into your local copy. It's a good idea to do this at the start of a dev session, or whenever someone makes a major change that your current task depends on.
  * *Note on conflicts*: If you try to pull down changes that conflict with your local copy (maybe you changed a level, and someone else did too), the fetch will spit out a conflict. You should be given an option to resolve the conflict, i.e. pick whose version wins out. If in doubt, check with the person who made the conflicting commit to see whose version should win out.
* *You changed the project*:  Changes are noted when you save a tracked file (for our purposes, most commonly a Blueprint with a *.uasset* extension). You then have to *commit* those changes, adding an appropriate description of what changed. Finally, you have to *push* those changes upstream to our central repository (this site) so that everyone can access them, using a somewhat confusingly named *pull request*. (It's called a request because the changes won't get pushed to the central repository automatically - instead we get to see them, comment on them, and handle any conflicts that might exist before confirming. You can read more [here](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests).)

## Development Standards (will add as I think of them)

Here's a few standards that we should try to stick by:

### Folder Structure

1. All game levels should be in the folder *ProjectYolo/Content/ProjectYolo/Maps*.