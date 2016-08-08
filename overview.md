## Class #1 ##

### General expectations ###
* Welcome to college.
* Today: we talk about a few details; then we build stuff, then we talk about how to talk about building stuff.
* For next class: make an account at http://onshape.com and model a cube with a hole through it, or something more complicated if you like.
* Turn off cellphones and computers in class.
* br.st@tufts.edu, I check email in the morning.
* Your fellow students are a valuable resource because they're new to the material, like you, so they share your reference frame.

### Let's build ###

Build a track for a golf ball out of popsicle sticks.

### The role of failure in learning ###

On average, you will learn faster if you take big, risky steps, fail, and then recover, than if you take small, safe steps and never fail. 

### Being open to critique ###

* *Criticize the design, not the person.* When you feel criticized, check whether the target might be the design rather than you.
  * :heart: "I'm worried this part won't be strong enough." :heart:
  * :warning: "You're out of your mind! This will never work!" :warning:
* *Be specific in your criticism.* Try to anticipate failures and describe failure modes.
  * :heart: "I'm worried the wood will slide under the tape, and then the upper deck will collapse." :heart:
  * :warning: "This design is bad. So bad. It just is." :warning:

## Class #2 ##

* Last time: Popsicle sticks and how we talk about building stuff.
* This time: Drawing, CAD modeling, tolerances, and iterative design.

### Technical drawing on paper ###

* You might think that, "I'm just not good at drawing." Note that almost everyone thinks that, even the people who are really skilled. It's scary to make a drawing and then show it to lots of people.
* Learning technical drawing makes you a faster, clearer, more efficient communicator. 

### The naive approach ###

In software, we call this "the waterfall method."

Here are the steps:

    1. Figure out what the thing needs to do, AKA "generating requirements"
    2. Design something with specifications that meet those requirements.
    3. Manufacture the thing.
    4. Test the thing.
    5. Manufacture a large quantity of the thing.
    6. Ship the thing.

Generally, this approach seems like it should work. Surprisingly, it usually does not.

### A more savvy approach ###

You could call this iterative design.

Here are the steps:

    1. Start with at least one basic requirement.
    2. Build a prototype quickly.
    3. Show the prototype to users.
    4. Add more requirements and return to step 2, (build a prototype).
    
Each iteration through the loop improves the quality of the prototype. After a few iterations, you can start making batches of prototypes ("alpha units" and then "beta units"). As you move from rough prototypes to detailed designs, the rate of iteration decreases.

If you take the approach of iterative design, tools that allow you to prototype quickly become extremely alluring. This is why people get so excited about lasercutters and 3D printers.

### 3D CAD with Onshape ###

* Chrome or Chromium will run a little faster than Firefox. Internet Explorer won't work right, as usual.
* Parametric modeling; explanation of how you can get into trouble
* Parts, part studios, assemblies, drawings
* Underdefined, overdefined, reference dimensions

There are a few different approaches you can take to CAD modeling.

* Example: modeling a sledgehammer as a filleted box on a cylindrical handle or a drafted extrusion on a swept handle
* Example: tracing a photo of a finial to create a profile for a swept solid

It might seem like a CAD model could define a part completely, but it omits data about tolerances. In real life, parts you make aren't perfectly formed, and it costs more money to make parts more perfect.

### Some mechanical tolerances for parts the size of your hand ###

* Woodworking tools, hand tools used by a skilled person: good to within 30 mil (~ 1/32")
* Machine tools, like a milling machine amateurs get to touch: 5 mil (0.005")
* Machine tools so expensive we aren't allowed to touch them: 1 mil (0.001")
* Wire EDM: 0.1 mil (0.0001", 100 microinches)
* Polishing machine used to make gyroscope rotors for Gravity Probe B: 0.0003 mil (0.0000003", 0.3 microinches)

## Class #3 ##

* Last time: Drawing, CAD modeling, tolerances, and iterative design.
* This time: Requirements vs. specifications, safety.

### Requirements vs. specifications ###

Specifications describe the characteristics of a something, usually with numbers.

*Tesla Roadster specifications*

* Length: 93"
* Width: 74"
* Weight: 2877 lbs
* Battery capacity: 53 kWh
* Battery energy density: 117 Wh/kg
* Battery volumetric energy density: 370 Wh/L
* 0-60 mph time: 3.9 s for standard model, 3.7 s for Sport model
* Range on EPA combined cycle test: 244 miles

Requirements describe targets that must be met or exceeded. Requirements are usually collected in a "requirements document."

For example, for the original Tesla Roadster, the requirement was that the car go 0-60 in under 4 seconds, because this what its high-performance competitors could do. When trying to hit this requirement, Tesla found that the best 2-speed transmission they could build couldn't survive the torque required to get under 4 seconds. They shipped the first 100 or so cars with a single-speed transmission that could handle the torque and offered to replace the transmissions once a two-speed transmission was developed.

Sometimes, requirements can lead you toward obsession with quantification. "Must be painted bright pink" is a legitimate requirement.
