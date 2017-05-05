# 387-Security-System-Final

The purpose of this project was to notify the owner of an apartment at the top of some steps when there is a guest knocking at the door. This is an issue in my apartment in particular because my door is at the bottom of 20 steps, so I can never hear when someone is at the door. The original idea was to simply create a system to detect a knock and relay it up the stairs. Then I thought it would be cool create a knock password. Once I got this working, I thought it would be cool to create a different passcode with something entirely new. I found a capacative touch breakout, which simply detected when one of the pins was touched. I thought it would be cool to connect these leads to different metal parts on the door, so that the guest could enter a touch password more discreetly to enter and not disturb me. Obviously this pass code would only go out to a certain few, but I though it was a cool idea. I have a video in the wiki demonstrating that the pins can actually be connected to other metal objects and it can still detect a touch. In order to add functionality to the project, I integrated a simple tilt sensor to detect if the doorknob was turned without either of the pass codes being entered correctly. At this point I was left with a simple, but unique security system.

If either of the pass codes are entered correctly, then the system will disarm itself and allow the guest to enter without the alarm going off. If the knock is either too hard or out of timing, then the system will say that there is a break in. This is to indicate that their is either the police or my landlord at the door because anyone else would call me before pounding on the door obnoxiously hard. The over or guest can then rearm the system by holding the pin on the captivate touch breakout that I have set to reset the system.

The data is sent from the bottom of the steps to the top through a simple one way RF link. This allowed easy and relatively reliable communication between Arduinos. When there was either a touch detected on the metal component or a knock, then it would send a signal to the Arduino at the top of the steps. The unit at the t0 of the steps will display whether or not it was a touch or a knock detected at the door. It would also buzz a piezo speaker to help get the owner's attention. I describe the project more in depth in the wiki.
