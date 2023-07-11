I've been having an idea about an anti-meta bot. Now it's time to make some serious commitments. 

# Initial idea
- Name: FLYING BEAGLE
- Namesake: [FLYING BEAGLE}(https://www.youtube.com/watch?v=HHOn8u-c2wk) (Himiko Kikuchi album)
- Weapon type:
  - "Lifter". It's not designed to be a lifter (but would be nice if it can be extended to a lifter), but more like a pair of keep-off arms. Like the "de-ICEr" of Ghost Raptor.
  - Rear-mounted horizontal blade, if weight allows.
- Why these weapons?
  - I want something that goes against the fork meta. Instead of playing the ground game, I want the chassis to be hollow in the front, so that if forks get underneath it, it won't disrupt anything.
  - Then the design would also need to counter the wedge meta. So the idea is to use a pair of arms to touch the wedges. Usually vert weapons' diameter is smaller than 3in, I assume (beater bars are 2.5"), so a pair of arms that reach out for longer than 3"/2 = 1.5" may be able to keep them from touching my bot.
  - But I'm not confident to win the control game as a very inexperienced driver whose previous bots all had weak or rarely controllable drivetrains.
  - So, in case the "lifter" design scores a pin, then the rear horizontal can still score some damage points by side-swiping. Kind of like Minimizer.
 
## More thoughts on the chassis

Main source of inspiration is SSP. 

#### SSP kit is 2lb without the servo and lifter module. My chassis design is likely never going to be lighter than that. 
However, there might be room for improvement? Such as deducing a pair of wheels, and sacrifice some armor? But the battery will also nearly double SSP's capacity, so no clear answer.

#### As a control bot, the drivetrain must be decent.
Easiest way out is buy SSP parts, I guess. But the Tarakan ESC was sold out. 

## More thoughts on the lifter design

Because the "lifter" is fairly unconventional, I'll start from listing some requirements. Not ranked yet. 

#### The lifter must be resistant to sudden impact

Kind of easy to achieve, but might still need some more thought. Current idea is to use TPU like Hot Wings [citation needed], and maybe add some aluminum or titanium "bone" inside each arm. 

From Discord it seems like 0.25" Al takes hits better than 0.125" Ti. But maybe weight would be the larger factor. 

**The lifter should survive vert hits.** I'm surprised how well Hot Wings' arms held up in June. Not sure if that can be transferrable - Hot Wings' arms move horizontally, but mine would be vertical. 

Here's hoping TPU fails in a good way. 

(For horizontal opponents: Consider wedge instead)

#### The lifter likely needs to have torque limiting features

This determines how the transmission is done. Clutch is too expensive (and requires more expeirience). Belt drive or gear drive fits my caliber. 

#### The lifter should be easy to swap

Reason: Would definitely need to prepare spares. Also, this opens up to different configurations. Example: When facing drum opponents, maybe arm can have a spoon-like curve at the end to fit into the back of drums. 

#### The lifter needs to have good bite power

Because that would bring several advantages: 
- When you get a hold onto the opponent, better bite power makes it harder to let loose.
- More power means possibility to self-right (although chassis should be designed to be drivable when inverted).
- More power means it may actually be able to work as a lifter in certain configurations. (Imagine forks that has downforce by itself)
But also some disadvantages:
- When clamping down, it may give the opponent more friction. Unless you don't hold off too much, and you hold off at parts further from opponents' wheels.
- 
#### The lifter mechanism is not exposed to the outside at any moment
(especially when inverted. Add some shield.)

## More thoughts on the horizontal design

There are 2 inspirations at this moment: Minimizer (or one of the similar bots), and The Chilli Daddy.

Notes from Minimizer design:
#### The wheels must be as up front as possible. 
Otherwise, when I spin the bot at a pin, the weapon won't be able to hit the opponent's side.

Due to the prior restriction, there's one more:
#### The bot can only have 2 wheels.
So that the center of spin resides as far away from the weapon as possible. 

Notes from The Chilly Daddy. design:

#### Chassis needs to be rigid enough to house a horizontal!
The Chilli Daddy. uses a CNC'd UHMW billet, I assume. That sounds rigid enough, because FTBBs usually do the same thing. 

But I would likely have to build the chassis without such fancy machinery. This is the time when I look at the Jolt! kit for help. 

#### Likely also would be gear drive
It's easy. And because a longer body means more weight and we likely won't have enough weight. 


# Design decisions

## Lifter mechanism

First we need to decide on a motor.
| Metrics | SSP Servo | DartBox |
|--|--|--|
| Resistant to sudden impact | Bad. But it's not direct drive, so maybe it'll work out? | Maybe equally bad |
| Torque limiting | Claims to have protection against stalling (0.6A after 8s) | Requires current limiting ESC. Otherwise it's toast. |
| Swap 
| Bite power 
| Weight & Size 
| Control |
Other options that were not followed-up with: 
- Repeat brushed drive: Only has 0.5 kg-cm stall torque. Scaling it up would be a challenge by itself.
  - I have tried to search for existing gearboxes. Pololu is an option, but even [the lightest (156:1)](https://www.pololu.com/product/3492) is about 46g. Add to original motor's 26g...
- Repeat brushless drive: It's more because I don't know how brushless can work for a lifter.
