# Initial Thoughts on Breakdown
1/9/2025

Fun to break it down! Wasn't expecting a NiMH battery, I assumed it would be lithium, but that's nice to see. 
I'd never taken apart one of these bump sensors before, so I was expecting some kind of a pressure sensor, but it 
turns out, no! At least for this vacuum, the bump sensor works by breaking a beam. Interestingly, they have the 
sensors all kind of hooked together into two harnesses, one of which contains the right side bump and cliff sensors,
the other of which contains the front and left cliff sensors and the left bump sensor. Kind of weird, but whatever. 
I was additionally surprised not to see wheel encoder feedback. I've always been a software first person, but my expectation
was to find motor drivers and wheel encoders, but again no. 

I believe I understand most of everything in the package, with one noteable exception. There's a power line that runs to the 
actual vacuum fan, which connects to the fan, but also to what I currently believe to be a 12v-4v convertor. The only issue 
is that the output (I think) is just...stubbed into the plastic? Not connected to anything at all? Weirder still, it uses a 
larger guage wire than the 12v. Very curious, probably just something I've never encountered but is standard.

As it stands, my current plan is to somehow replace/replicate the functionality of the microcontroller, while providing 
connectivity to a Raspberry Pi5 that I'll mount on top, which will also be where I place any more advanced sensors for area
mapping (LiDAR/cameras). If I could just get communication and code control on the microcontroller, that would be amazing, 
so I'll definitely look into it for a while, but I believe it's a custom board, so I'm not sure how to go about doing that. 
Maybe identify the processor, try to identify the communication protocol, and then try to get the code off the board? If I
was able to do all of that (which I doubt), I'd be able to simply add a communication harness and add sensor output/command
input functionality to the code. However, I think I'm more likely to have luck replicating the capabilities of the 
microcontroller with new hardware of my own, and providing that I/O harness that way. 
