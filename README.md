# Microchallenge-3

As the world faces increasing challenges related to water scarcity and environmental sustainability, innovative solutions are needed to promote efficient use of water resources.
One such solution is the implementation of grey water filtering systems, which allow for the reuse of wastewater from household and commercial activities.

This project was designed and developed as part of the third challenge in the IAAC's Master in Design for Emergent Futures course as part of the "Digital Prototyping for Design" seminar. 

The project is an exploration of the aesthetic and practical possibilities of reusing greywater in an urban environment.

Team: Çağsun, Korbinian, Ramiro as [Flowing Futures Collective](https://www.instagram.com/flowingfutures/)

![image](https://github.com/ramiroarga/Microchallenge-3/assets/115219057/7086dcc6-99ff-49da-aa6e-9ebbc167feb0)

## The Context

In the previous [design challenge II](https://https://cagsunacemoglu.github.io/MDEF/term2/MicroChallenge%20II/), we had developed a first prototype of bio/filter which we aimed to test in the upcoming months. It was a first trial for a two stage filter (lipid extraction & biofilter) that was not yet fully integrated as a system.

![](https://hackmd.io/_uploads/SJXriyzDn.jpg)

On the same day that we presented this prototype, [Space10  published a blueprint](https://space10.com/project/the-biofilter-lab/) for a very similar project. It was based on the same needs and they came up with a DIY proposal, along with an open documentation of its blueprint.
The SlowLab collective approached us with their intention to develop a copy this blueprint and we teamed up to build it together. 

While there were some good ideas in Space10's blueprint that we adapted, there were also a lot of bad design decisions from our view that we looked for ways to improve in this challenge.

**Here's a summary of our adaptation of the blueprint:**

What we kept:
- We liked and applied the idea of combining the biofilter with gravel-sand-carbon type mechanical filter in the same container
- We kept the idea of integrating the whole system in a sink structured

What we improved:
- We reduced the number of pumps from 4 to 2, by utilising gravity where possible
- We added a lipid extraction filter as the first stage to seperate greases from the water that enters the 2nd filter stage
- We were conscious about the materials we used: we used less containers, pipes, removed a lot of unneccary pieces, and used recycled/refurbished materials (old wood, broken clay pieces for the filter, etc.) where possible. We also sourced all our purchases from local providers making sure that everything we use is accessible by anyone who whats to duplicate this prototype.
- We looked for opportunities to depend less on technology and converted one of the pumps to a manual feet pump to run the sink - this makes the system less dependent on external energy sources, easier to maintain and involves the user in a different way than just asking them to use a black box.
- We rethought and redesigned the whole user workflow: Now users don't need to turn on/off electric pumps to operate the system.
- Part of the maintenance is now done by a microcontroller which we included that senses the water level in the lipid section and moves it to the 2nd stage filter automatically.
- The only electric pump we used is a 5V pump which can be run from a standard USB mobile batteries, which makes the unit a fully mobile & autonomous system, making it possible to use it out of the water grid.
    - For that purpose, we added more robust wheels than the original design what could be used on more diverse surfaces 
- We made the containers and overall design as transparent as possible for the users to easily understand how the system works so that they can intervene when necessary.

## The System

Having made these changes, we ended up with a grey water filtering system integrated into a sink. 
It's a point-of-use system, which is designed to treat water that is sourced from simple usage purposes such as washing hands, vegetables or dishes.

### The system map

> Schematics of the System
> The upper level horizantal filter is not yet utilised.
![](https://hackmd.io/_uploads/rJZtMlGwn.jpg)


### Explanation of the system flow

1- When a user uses the sink, the water goes through a mesh that filters large solids and water moves into the lipid extraction unit. The water remains there for some time, while the greases flow to the surface of the water and smaller solids sink to the bottom of the container. 

2- When the lipid container fills up, there's a water level sensor that detects the level of the water, and to avoid overfill, moves excess water into the upper filter unit where water free from greases gets filtrated slowly to remove other substances.

* The pump speed is adjusted to the speed at which the filter can process water. This part of the process is fully automated, users don't need to keep track of overfill of lipid section or pour water into the biofilter unit manually at a certain speed: It's all taken care off.

3- As the water is processed in the bio-mechanical filter section, it refills the main tank we're using for clean water. 

From there, when a user needs to use the sink, they pump the water by using the feet pump into the faucet and the circle starts again. 
<br>

<iframe src="https://player.vimeo.com/video/830141929?h=699de9916d" width="640" height="638" frameborder="0" allow="autoplay; fullscreen; picture-in-picture" allowfullscreen></iframe>
<p><a href="https://vimeo.com/830141929">Prototype v3 on Vimeo </a></p>

## Components of the System

### The Sink & the carrying wooded structure

Our friends at [SlowLab](https://www.instagram.com/slowlab.bcn/) bought a second hand sink in Wallapop and it became the starting point for building the prototype. We made some feet for it from refurbished wood at [Akasha Hub](https://akasha.barcelona/en/) to construct the main structure that would carry all components. We made a level near the floor to add our water tanks. 

We also cut out a hole on the unused area of the sink to place the filter unit there.

![](https://hackmd.io/_uploads/B1NmLxGvn.jpg)


## Lipid Extraction Stage

We previously had an acrylic lipid extraction filter we made using expensive acryllic material and laser-cutter. It was also not easy to fix it and make it leak-free using silicon - a material we wanted to avoid as much as possible due to environmental effect, difficulty of use, and additional costs. 

To make the project more accessible, we bought a cheap plastic container and a PVC roll for kitchen use and integrated them together using tape for an easier to build lipid filter. The idea to drill holes on the PVC to allow water flow from the center of the lipid section so that the lipids on the top do not flow to the right hand side section.

Users need to remove the greases on the top of the container manually with a certain frequency.

*Before*
![](https://hackmd.io/_uploads/rJxhPxMv2.jpg)


*After*
![](https://hackmd.io/_uploads/H1mZKxfPn.jpg)


## The bio-mechanical filter

This is the core of the system and took a while to build. We sourced materials from different places, the sand was from a friend at Iaac. Instead of gravel, we used broken 3d printed clay pieces we found in Iaac's trash. The plant was purchased by our friends at SlowLab. We bought the containers and the activated carbon in local small shops.

![](https://hackmd.io/_uploads/HykJBlGD2.jpg)

The process was tedious in the sense that we had to wash the sand around 10 rounds to get to clear water. Washing the clay pieces was much easier. This made us reflect on energy and resources used in our production process, the already baked clay pieces came to us from the trash but they were much cleaner. We discussed that next time it may be prudent to use pre-washed sand. 

We used a modular approach to build the filter, where we have kept all the materials in separate containers for easier maintenance later on. Each material container has holes on the bottom of it to allow water passage to the next material.

When the physical filter was done, we placed the plant on a conic plastic piece (the cover of the container we had fulfilled this purpose) so that water from the plant doesn't overflow to the tank directly but rather gets directed to pass through the filter.

By placing each module on top of each other we have constructed the filter module which we placed in a larger container that holds the exiting water. We drilled a hole in that container to move the clean water into the main clean water tank of the system using gravity. 

This process deserves a repo on its own which we plan to do in the upcoming months.


![](https://hackmd.io/_uploads/HyBs2gMPh.png)

![](https://hackmd.io/_uploads/HJBmTgMwh.png)

### Automated Pump

We developed a simple sensor by using the capacitive touch feature of the ESP32 chip we've used in this system. It's a simple wire that we placed in the lipid extractor tank. When the water touches the wire, the capacitance on the wire changes and it warns the system to run the pump.

Triggered by that, the pump starts running and pumps water up to the filter stage until the wire doesn't touch the water again. This way we make sure the lipid section is emptied continuously and water doesn't overflow.

![](https://hackmd.io/_uploads/rJT8JZGv3.jpg)

// ADD ARDUINO CODE

### Feet Pump

To operate the sink, we decided to use a manual pump rather than an electric one for many reasons such as maintenance, energy dependency, user interaction and amount of technology to develop and deal with.

We ended up converting a hand pump which is normally used to move gasoline out of a car's gasoline tank, into a feet pump so that the users' hands are free while operating the sink.

We made a feet stand with some old wood pieces and a soft ball to push pump easily. It ended up working pretty well.

![](https://hackmd.io/_uploads/S1WVJZGPh.jpg)

### Integrating the System

After testing each part on its own,wWe brought together all these elements of the system using different size pipes, and some water fittings and makes sure the whole flow of water in the system works. And that placement of the components and usage of the system is user-friendly.


The system works well so far, but we must mention that we are in the early days of its utilisation, and we're observing daily performance and utility of it.

---
Some final sketches of the prototype:
![](https://hackmd.io/_uploads/ryeBK96Pn.png)
![](https://hackmd.io/_uploads/Byo6Y9Twn.png)


## Future Developments

There are some potential improvements that we can already foresee:

- A full documentation of the process to make this system accessible to anyone looking to build it, with the whole building process explained step by step with photos and videos.

- Potentially separate the fresh water tank from treated water for alternative uses of water in different use cases

- Monitor maintenance needs as we use it and document it

- Monitor plant health and upgrade plant containers and fine-tune plant choice for the system.

## Conclusion

We aimed the grey sink to be an easy-to-use and effective system for treating waste water which can be constructed using locally available materials and resources. 

We look forward to seeing if it's a convenient, effective and practical solution for households and other settings such as off-the-grid water source needs or in rural areas where water supply may be limited, and proper waste management is essential for sustainable living. 

We hope to hear from anyone who constructs the system to hear their experiences and we'll continue to develop the system and share our findings in an open way.

Please reach out to us in our social channels for questions & comments: https://www.instagram.com/flowingfutures/

