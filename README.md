CelShader
=========

Advanced CelShader project for Unreal Engine 4

### Example Screenshots and original thread

https://forums.unrealengine.com/showthread.php?7164-A-different-kind-of-cel-shader

### Content samples

Proper content samples (along with higher tier support) are available for users who have purchased this asset from the Epic Marketplace. If you'd like to see this shader appear on the Epic Marketplace and receive more support, please vote for it when it eventually appears on the Epic Marketplace Trello board!

### To use

1. Check out the branch correlating to the version of Unreal Engine you're using, e.g. 4\_5 or 4\_4.
2. Migrate the CelShader folder from the sample to your target content folder.
3. In your project create a post-processing object.
4. Go to the Misc tab and add a CelShader preset instance as a blendable, e.g. CelShaderDirtyManga.
5. Set the post-processing object to be "unbound".

It's that easy.

### Documentation

http://skull.co.nz/cel-shader-introduction/

### Final tip

If you're getting too many lines drawn on a particular texture but the rest of the scene looks alright, try either lowering the resolution of your textures or go into photoshop and apply a smart blur. The cel shader will pick up even tiny amounts of detail with the right settings, so go nuts and blur it a lot. If you're after a kind of water-colour fill effect, then smart blur is the way to go.
