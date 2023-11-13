# Welcome

Here you will find a couple of exercises to help us get to know your experience
with Web development. We want this to be fun and solved in the same way you'd
tackle a real project at work.

Choose your favorite web framework that can run entirely in the browser.
Meaning don't use any framework that requires server-side rendering as at
TripShot our web apps are all SPAs. Feel free to use online documentation and
incorporate your favorite libraries into the project. Take a few days and if
you need more time just let us know.

## Using an actual TripShot endpoint

You'll build a simple web application based on a TripShot api. TripShot has
many customers with public-facing routes and timetables so we'll use one here.

Look at the output of this endpoint : https://mtma.tripshot.com/v1/p/route

```
curl 'https://mtma.tripshot.com/v1/p/route' | jq '.[]'
```

That produces a JSON array of JSON objects, each corresponding to a route available to riders on the MTMA service.

Create a small web application using this endpoint that does the following:

1. Retrieves the list of routes returned by this endpoint.
2. For each route show:
    a. The route name taken from the 'publicName' key, displayed with a background color taken from the 'color' key.
    b. When clicked, the route name takes the user to the url taken from the 'routeUrl' key.
3. Add a button or other UI element that allows sorting the route list by ascending or descending route name.
4. Automatically refresh the list every 10 seconds, preserving the current sort criterion. (Note that the endpoint contents rarely changes.)

## Making a fun game

Construct a web-based tic-tac-toe game. This need not be fancy but should do the following:

1. Allow two players to take turns (no need to implement an NPC).
2. Show the grid using DOM and CSS, no SVG or Canvas.
3. When either player wins or all squares are filled resulting in a tie game, indicate the game is over and indicate the outcome.

## Wrapping up

When you are done, put your code into a zip or tarball. Include anything needed
to build on a Linux/Mac OS machine and a short description of how to build and
test. Email that file back to us.

We are always interested in improving our hiring processes, so feedback about
the exercises is welcome.

Congratulations, you are done. Thanks for your interest in TripShot!

