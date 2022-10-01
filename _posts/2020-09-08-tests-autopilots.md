## Testing the autopilots

Our **Goose** prototype has been out for a year now (2kg for 500g of payload). Although this doesn't look like much, the stucture has held up despite numerous falls (let's take a moment to remember the countless times it rolled over 10+ times, or this wall it collided into at 20km/h... without a scratch!:sunglasses:).

<div style="text-align: center;"><img src="/images/2020-09-08_launching-goose.jpg" alt="" width="60%"/></div>


But today is about our new guidance and navigation systems! These are built on top of our home-made control algorithms for different flying modes, namely *Altitude-Hold* and *Heading-Hold* ensuring constant altitude or heading using barometer or gyrometer data respectively. Due to the low reliability of our GPS sensor, a navigation filter is being developed (we went for an Unscented Kalman Filter), thanks to the dynamics equations derived when designing our simulator.

<div style="text-align: center;"><img src="/images/2020-09-08_goose-in-auto-pilot.jpg" alt="" width="60%"/></div>


A First guidance algorithm consists in a *Return-To-Home* (RTH) feature. Indeed, should we lose the communication between the pilot's remote and the drone, our mechatronic friend should come back to its take-off location on its own - or at least until the communication is restored. Therefore, dynamic waypoints are computed, taking into account the large radius of curvature of the paramotor. Another algorithm was designed so as to come near each waypoint and counteract external disturbances (wind gusts in particular), using the motor as little as possible (this allows to return safely, should the battery run low). Eventually, the drone hovers in circles over its take-off location.


<div style="text-align: center;"><img src="/images/2020-09-08_goose-flying.jpg" alt="" width="60%"/></div>

The second guidance algorithms uses the same principles to achieve a desired trajectory (carefully adding extra waypoints so as to smoothen and successfully accomplish the trajectory). Unfortunately, due to legal restrictions in Europe at the time of writing, Beyond-Visual-Line-Of-Sight (BVLOS) flights are prohibited, and missions (including the drone's expected trajectories) often need to be established in advance. For this reason, we decided to focus on accurate path following, which, let's face it, is no easy thing to do with an autonomous paraglider!

<div style="text-align: center;"><img src="/images/2020-09-08_collapse.gif" alt="" width="50%"/></div>
