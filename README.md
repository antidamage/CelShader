CelShader
=========

Advanced CelShader project for Unreal Engine 4

**Example Screenshots and original thread**

https://forums.unrealengine.com/showthread.php?7164-A-different-kind-of-cel-shader

**To use**

1. Migrate the CelShader folder from the sample to your target content folder.
2. In your project create a global (unbound) post-processing object.
3. Go to the Misc tab and add the CelShader instance as a blendable.

It's that easy.

**Master**

Debug your shader here. You can enable/disable the shader entirely, or force it to only draw lines. This in itself is a neat effect.

**Cel Detail Shading**

This manages the lines drawn when detail in the scene and in textures are outlined. These lines default to light. Cel detail always shades near to the camera and you can control the falloff as distance increases.

**Cel Outline Shading**

These are the lines drawn around objects based on differences in screen-space depth. These lines default to heavy and can have a mask texture applied to roughen the edges. Cel outlines have a band in the scene depth that can be targeted for shading. Offset is the distance from the camera. Ramp is the linear fade-in and fade-out distance.

**Distance overbright**

This controls a blend_overlay fog that is useful for colour-grading the scene. In the screenshot above it's used to give distant objects a warm desert-feeling glow.

**Shadow Shading**

This controls the cross-hatching on your scene. The cross-hatching will target areas with AO shadows. You can also posterize your AO to give it a more cartoony feel. The values in this section have a quite narrow window where they look good, I'd recommend only adjusting them by a tiny bit at a time.

**Final tip**

If you're getting too many lines drawn, try either lowering the resolution of your textures or go into photoshop and apply a smart blur. The cel shader will pick up even tiny amounts of detail with the right settings, so go nuts and blur it a lot. If you're after a kind of water-colour fill effect, then smart blur is the way to go.
