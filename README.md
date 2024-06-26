# 0816 automatic smt feeder controller firmware

This is the firmware needed to use the 0816 smt feeder. Find details on the feeder design, setup and features in [the wiki documentation](https://docs.mgrl.de/maschine:pickandplace:feeder:0816feeder)

![render of the 3dprintable automatic 0816 smt feeder](https://user-images.githubusercontent.com/3868450/34632854-34719c14-f278-11e7-8e8d-e245edc932fc.jpg)

[Watch a video showing the smt feeder in action](https://www.youtube.com/watch?v=vJzb3llKgjA)

added additional config feeder_type 'T' for Bing Feeder v2 which accepts a pulse instead of pwm servo
allows single controller to manage a mix of standard 0816 feeders and bing v2 feeders
the default type of feeder is now bing.  when configured as 0816, the output pin is configured for servo output which makes any bing feeder constantly feed. when configured as bing, a 0816 feeder does nothing.