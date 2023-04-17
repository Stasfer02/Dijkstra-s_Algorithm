The algorithm uses the following network:

<img width="248" alt="Screenshot 2023-04-17 at 14 20 38" src="https://user-images.githubusercontent.com/96784667/232482302-d70a4971-54ce-4551-80a7-a347acb519d9.png">

The cities are connected by train lines that have a certain length. Our algorithm has to find the fastest way between two given points and the route it took. 

There's one extra hurdle: there could be disruptions in the train network (Duh, it's holland). 

These can be specified by the user.

An example input would look like this:


2           -> meaning, two disruptions 

Utrecht     -> disruption 1, city 1

Zwolle      -> disruption 1, city 2

Enschede    -> disruption 2, city 1

Zwolle      -> disruption 2, city 2

Amsterdam   -> route 1, city 1

Groningen   -> route 1, city 2

Enschede    -> route 2, city 1

Eindhoven   -> route 2, city 2

Leeuwarden  -> route 3, city 1

Eindhoven   -> route 3, city 2

!


the corresponding output would be:


Amsterdam   -> route 1

Utrecht     ..

Eindhoven   ..

Nijmegen    ..

Zwolle      ..

Meppel      ..

Groningen   -> end route 1

269         -> #minutes round 1 took

UNREACHABLE -> the second route is not reachable due to disruptions

Leeuwarden  -> route 3 

Meppel      ..

Zwolle      ..

Nijmegen    ..

Eindhoven   -> end route 3

187         -> #minutes route 3 took



