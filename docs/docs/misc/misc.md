# New lit effects

![type:video](separate_animation_test.mp4)

here’s the toys in action

the cessna wing has a gradient alpha window cut out of it in the albedo, the emissive channel has NO alpha.

i’ve animated LIT level and alpha albedo separately to pitch and roll of the aircraft

note that the emissive can show through EVEN when the albedo is FULLY gone (0% alpha!) and it creates Z artifacts and cuts away the aircraft door.

(just like it would at 1% alpha)

I believe this provides _almost_ a superset of the functionality 11 can do and covers every case anyone seems to have.

(the only case it can’t do is if you had alpha in the lit AND alpha in the albedo that were different and were somehow trying to use both — i haven’t herad of anyone doing that yet.)

## new attributes

```ATTR_albedo_opacity <low> <high> <dataref>```

```ATTR_albedo_opacity_reset```

if these seem exactly like ATTR_light_level it’s because they are - they provide th animation factor for an alpha channel - except the alpha goes in your albedo.
If you have an alpha animation effect that’s broken, replacing the ATTR_light_level directives with these and moving the alpha to your albedo shuold be a 100% fix.

new directive for the header

```SEPARATE_LIT```

If your lit texture is being lost because of the albedo’s clear alpha (and you can’t “Fix it” by using lit channel albedo) put this directive in and go home happy.
use this for when you have an emissive overlay as a separate mesh directly on top of  another mesh.

