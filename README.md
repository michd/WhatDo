# What Do
This will be my take on, to put it simply, a TODO app. I figured I'll develop it in the open from the very beginning.

So at this point there is nothing to see. (Watch me forget to update the README as there start being things to see...).

## Thinking

The user interaction in general use I want to see from this app is:

1. Have some spare time in which you'd like to get _something_ done
2. Open up the app
3. App asks "how much time you got?"
4. Press some preset timeframe button
5. App presents a task that's due that has an approximate duration that's close to / within the amount of time you gave.
6. Do the thing, tell it you've done the thing

This relies on the idea of recurring tasks that aren't really on a rigid schedule, but which you probably be done with some regularity. 
I often find myself noticing a thing and being like "I should really get around to doing X again" (like cleaning tasks). Then I end up having free time to fit in some task, but can never remember those.

So this app would keep track of tasks, how often you want them to be done, and approximately how long they take, in order to provide a very low friction way to select a task to do and mark it as done.

I have further ideas but that's the minimal core of it.

### Technically

I've never made a "progressive web app". So my goal is to build this as an installable web app that can work purely clientside, using indexedDb for storage of all the task data etc. So essentially a fully functional app out of purely html/css/js.

However, that locks you to a single device to use it on, which isn't great. So I also wish to build an _optional_ server side where you can create an account, to sync this all to. The client will keep in sync with the server when it can but should be fully functional offline.

Beyond that, the ability to share collections of tasks with another registered user, for collaboration (such as in a household).

Such a server side for it I envision as being written in rust, with an SQL database (probably mysql/mariadb as it's what I'm used to), and deployable with docker-compose, so it's relatively simple to self-host the thing, so you don't have to give up your privacy for convenience / rely on me to keep hosting the thing.

---

Anyway, better get to building it. :)
