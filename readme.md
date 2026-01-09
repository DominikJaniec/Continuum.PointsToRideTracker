# Continuum :: Points To Ride Tracker

a simple web application to track victory points while playing the Ticket to Ride board game with my family or friends.

this web page should not need any active backend, nor external databases. every state should be kept in user's browser memory.

app should keep track of victory points per player, and having a history of those receiving events within one game.

main focus of this app, should be helping with tracking points during a single paly-through with useful UI and workflow, as steps below:

1. the setup -- create a set of players, or load them from memory.
    * every player should be unique in that play set.
    * a player should have at least a name and one of 7 basic colors.
    * arrange those players in some "circular fashion", to represent the game order.
    * user should be able to rearrange and edit them easily on UI during this setup phase.

2. the game -- following the game order, register one or more events representing receiving victory points.
    * while starting, the first player has to become starting one, and everyone have 0 points without history.

3. the receiving points UI -- for current player, user should be able to choose:
    * a track victory points value from preset:
        * "one car": 1 point
        * "two cars": 2 points
        * "3 cars": 4 points
        * "4 cars": 7 points
        * "6 cars": 15 points
        * "8 cars": 21 points
    * a ticket route victory points as:
        * free positive number value
        * with optional two names for both ends
        * with a toggle representing if that route was finished
        * and when unfinished, those points should be treated as negative
    * a custom bonus victory points as:
        * free positive number value
        * with optional name
    * to see scoreboard with leader on top
    * to see history of points for that player
    * to navigate to previous and next players
    * to reset the game with a prompt, going to the setup step

----

## it was vibecoded 😕

I've used basically the first part of this file as a prompt for some "vibecoding tools" for software developers.

I'm rather surprised with the results, and I'm glad that I've checked more tool than first one, as my initial and expected disappointment after using this extended "prompt" for first try, was satisfied in at least one tool right out of the box.

likewise, I know about vibecoding tools like:

* https://replit.com/
* https://emergent.sh/
* https://bolt.new/ (StackBlitz)
* https://lovable.dev/

on _replit.com_ I've started with a more simple prompt:

> I need a simple web application to track victory points while playing the Ticket to Ride board game with my family.

but apparently _"a simple web app"_ means a full stack template, with `36MB` of DB and whole CRUD backend. thus, with that disappointment, I've developed that more precise prompt on top of this file. unfortunately, I was already over half of my free tokens, thus agent is still working. but, whatever was done already, agent still used DB and backend, which even they said that those components should not be there at the beginning.

then, I've tried that long prompt with all three other tools simultaneously - in order above.

on _emergent.sh_ theirs agent start with asking questions about visual style - rather some not important thing for me, but I've assumed that this is a good sing. progress looks good on provided screenshots, unfortunately given free tokens run out before I've got any access to results.

on _bolt.new_ (StackBlitz) the project structure looked promising, however after two tries for fixing a "blank page", I've again run out of tokens again... fortunately, I can easily access sources and download them as single zip file.

on _lovable.dev_ I've got very good results very fast. it's agent also proposed an `Undo` button after the first iteration. and UI looks very nice and useful. there is access to every source file, however, even agent couldn't provide a way to get code without joining with GitHub.

finally, with another set of free trials tokens, I've gone back to _replit.com_ with its full stack project. after a few requests to remove DB code, it reimplemented storage to within JS runtime, but deployments somehow still required database. fortunately, access to code is very easy, and I got my sources as a single zip file.

also, with _bolt.new_ and after more request for fixing blank page, agent suggested browser's memory clean up, which I've solved loading that project in MS Edge instead of Firefox, and with some patience, app finally loaded. UI is not that bad and I could easily download sources.

### best results so far

> as on 12026-01-09

1. https://points-to-ride-tracker.lovable.app/ (no sources)
2. https://ticket-tally--dominjaniec.replit.app (js-storage)
3. https://ticket-to-ride-victo-69jm.bolt.host (local-storage)
