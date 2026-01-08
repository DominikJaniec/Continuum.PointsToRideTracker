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

I'm rather surprised with the results, and I'm glad that I've checked more tool than first one, as my initial and expected disappointment after using this extended "prompt" for first try, was satisfied in at least one tool.

I know about vibecoding tools like:

* https://replit.com/
* https://emergent.sh/
* https://lovable.dev/

### best results so far /12026-01-09/

1. https://points-to-ride-tracker.lovable.app/

* looks great, and that tool suggested that "undo" button itself
* but no good way to get source without accessing with github...
