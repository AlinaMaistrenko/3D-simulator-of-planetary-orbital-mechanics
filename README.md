# 3D-simulator-of-planetary-orbital-mechanics
An orbit simulator for the solar system in real scale with Newtonian dynamics and Kepler laws, which can be manipulated.

## Screenshots

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/screenshot1.jpg)

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/screenshot2.jpg)

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/screenshot3.jpg)

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/screenshot4.jpg)

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/screenshot5.jpg)


## Controls

* '+' key increases simulation speed of time
* '-' key decreases simulation speed of time
* 'W' key rotates the vehicle upward
* 'S' key rotates the vehicle downward
* 'A' key rotates the vehicle left
* 'D' key rotates the vehicle right
* 'Q' key rotates the vehicle counterclockwise
* 'E' key rotates the vehicle clockwise
* 'Z' key sets the throttle to maximum
* 'X' key sets the throttle to zero (halts the engine)
* Shift key gradually increases throttle
* Ctrl key gradually decreases throttle
* 'H' key toggles camera chase mode
* 'G' key toggles grids


## Autosave feature

The simulation state is automatically saved to your browser's localStorage.
When you exit the application and load it again, you will continue from where
you left off.
If you want to reset state, choose "Earth orbit" from the scenarios.



## User Interface


### Overlays

#### Periapsis

![Periapsis](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/periapsis.png)

This icon is shown on the periapsis of current orbit.

#### Apoapsis

![Apoapsis](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/apoapsis.png)

This icon is shown on the apoapsis of current orbit.

### Navigation ball/Throttle bar

On the bottom of the screen is the navigation ball and throttle bar.

![navball](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/navball.jpg)

#### Throttle bar

* Clicking and dragging on the throttle bar on the left will control the throttle.
* Clicking on the max button will make the throttle maximum (maximum acceleration).
* Clicking on the stop button will halt the engine (zero acceleration).

#### Navigation ball

The navigation ball on the right indicates the orientation of the vehicle
in relation to currently orbiting body.

Pointing mouse cursor or holding touch on the navigation ball shows a set of
arrows indicating rotation directions.

![navball rotation](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/navballRotation.jpg)

Pressing keyboard keys corresponding to the rotation direction or pressing the arrows by the mouse or finger on touch screen will rotate the rocket in
the designated direction.
Note that the rotation has inertia; the longer you hold pressing, the faster
the spin will be and takes longer time to stop.


#### Prograde/retrograde icon

![prograde](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/prograde.png)
![retrograde](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/retrograde.png)

These icons on the navigation ball indicates which direction the rocket is
going, in relation to the vehicle's orientation.

The left icon is called prograde, meaning the direction the vehicle is going.
Accelerating in this direction will put more energy on the orbit and push it wider.

The right icon is retrograde, meaning the direction opposite to the vehicle is going.
Accelerating in this direction will reduce the energy from the orbit and make it narrower.


#### Watermark

![watermark](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/watermark.png)

This icon indicates horizontal line in the vehicle's orientation.
The navigation ball is oriented in a way that the watermark is fixed.

It is common to see this kind of instrument in actual aerospace vehicle.
I guess this is useful for aerial vehicles, but not so much in space.


### Simulation Speed Control

On top left corner of the screen is a widget for controlling the speed of the simulation, from real-time to a million times faster than reality.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/timescale.png)

Clicking on one of the green triangles sets the speed to that scale.
Leftmost is slowest and it gets faster as you go right.
Each triangle means 10 times faster than the previous one.
You can also change the speed by '+' and '-' keys.

Note that you cannot turn or accelerate the vehicle unless you're in real-time scale.

You'll need it to travel distances between planets.


### Scenarios

On top right corner of the screen is a little icon.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/menuIcon.png)

Clicking it will show a list of predefined scenarios.

![Scenario selector](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/scenarioSelector.jpg)

Clicking one of these items will teleport the rocket to specific location in the solar system.


### Save State

On the 2nd from right top corner is an icon for saving simulation state.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/saveIcon.png)

Clicking it will show a list of saved states.

Saved states are like scenarios but you can create whenever and as many as you would like to.

You can either type a new save name or overwrite existing one by clicking on its name.
You can delete a saved state by clicking on the trash can icon ![trashcan](src/images/trashcan.png).

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/saveData.jpg)


### Load State

On the 3rd from right top corner is an icon for loading simulation state.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/loadIcon.png)

Clicking on it will show a list of saved states.

You can click on one of the items to load it.
You can delete a saved state by clicking on the trash can icon ![trashcan](src/images/trashcan.png).

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/loadData.jpg)


### Orbital Elements

Just below the Speed control is a little icon for toggling orbital elements display.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/orbitIcon.png)

If you click on it,  a little table shows up like below.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/orbital-elements.png)

These are parameters that uniquely define the orbit, given an orbital plane as a reference frame.
In this application, reference frame is ecliptic plane.
If you're not familiar with orbital mechanics, [Wikipedia](https://en.wikipedia.org/wiki/Orbital_elements) is a good place to start learning.

* e - Eccentricity.
* a - Semi-major axis.
* i - Inclination.
* Omega - Longitude of Ascending Node.
* w - Longitude of Periapsis.
* Periapsis - The distance of Periapsis from the center of celestial body.
* Apoapsis - The distance of Apoapsis from the center of celestial body.
* head - Whether the vehicle is heading towards apoapsis. This is not really an orbital element, mainly used for debugging.


### Celestial Bodies

Below the Orbital Elements control is Celestial Bodies button.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/bodiesIcon.png)

If you click on it,  a little table shows up like below.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/celestialBodies.jpg)

Currently focused celestial body is highlighted.
Clicking on a name of a body will make the focus move to that body.


### Statistics

On the 4th from right top corner is an icon for statistics.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/statsIcon.png)

Clicking on it will toggle the display of statistics of the whole mission.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/statistics.jpg)

* Mission time

  Quite obvious, but it's the (in-simulation) elapsed time since the simulation has started.

* Delta-V

  The total Delta-V exerted by burning the rocket engine. Basically all rockets have limited Delta-V, which is determined by amount of fuel and weight of the rocket, among other factors.
  However, in this simulation, our rocket has infinite Delta-V.

* Ignition Count

  If you throttle up from zero, it's counted as an ignition. The number of ignition matters because re-igniting liquid fuel engine in zero-g is not a trivial work.

### Settings

Just below the Statistics icon is an icon for toggling setting display.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/src/images/settingsIcon.png)

Clicking on it will toggle the display of a panel for settings.
Characters in parentheses indicate shortcut keys.

![](https://github.com/AlinaMaistrenko/3D-simulator-of-planetary-orbital-mechanics/blob/main/WebGL-Orbiter-master/screenshots/settings.jpg)

* Show grid - Toggles display of a grid in space.
* Chase camera - If it's turned on, the camera will automatically face the directon of vehicle's acceleration.
* Nonlinear scale - Renders objects in a fake scale so that they appear even if they would be smaller than a pixel in real scale. Don't worry - the simulation will always be performed in real scale.
* Units in KM - Shows distances in Orbital Elements panel in Kilometers instead of AUs.


## How to build

Use npm to build or debug the project.

1. Install Node.js
2. Run `npm i`
3. Serve the page with `npm run start` and open `http://localhost:8080` with a browser
4. or `npm run build` to make a static website.


## Libraries

This project uses:

* three.js
* Node.js
* webpack
