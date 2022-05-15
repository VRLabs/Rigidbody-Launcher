# Rigidbody Cannon
  
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-informational.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-informational.svg)](https://vrchat.com/home/download)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Rigidbody-Cannon/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Rigidbody-Cannon/total?label=Downloads)](https://github.com/VRLabs/Rigidbody-Cannon/releases/latest)

Launch an object with collision against the world.

## How it works

Physics joints, constraints, a particle system, and contacts are animated to shoot a rigidbody with a collider and change a parameter on collision with the world.

## Preview


## Install guide

You must be using the latest [Avatars 3.0 Manager](https://github.com/VRLabs/Avatars-3.0-Manager) version, as it adds "IsMirror" as a default parameter.

[Local Mirror Detection](https://github.com/VRLabs/Local-Mirror-Detection) is required for this package to work. Import and merge the FX controller.

Merge the FX controller from this package to your own FX controller, using the [Avatars 3.0 Manager](https://github.com/VRLabs/Avatars-3.0-Manager) tool.
 
"Rigidbody Cannon.prefab" should go to the base of your Unity scene, which will give it base Unity scaling.

Unpack the prefab by right-clicking it.

Place "Rigidbody Cannon" at the base of your avatar.

Remove "Rigidbody Cannon Target" outside of "Rigidbody Cannon" and place it anywhere in your avatar's hierarchy. Adjust the transforms as you need.

## How to use

**"RigidbodyCannon.Control" parameter must be true for the system to fire, and false to reset.**

You can edit the projectile velocity with the configurable joint on the "Rigidbody Cannon/Kinematic Rigidbody/Collision" object. Change the "Maximum Force" property under the "Z Drive" section. Alternatively, edit the "Fire.anim" clip and change the "Target Velocity".

## Downloads

You can grab the latest version of the Rigidbody Cannon in [Releases](https://github.com/VRLabs/Rigidbody-Cannon/releases/latest).

## License

Rigidbody Cannon is available as-is under MIT. For more information see [LICENSE](https://github.com/VRLabs/Rigidbody-Cannon/blob/main/LICENSE).

## Contact us

If you need help, our support channel is on [Discord](https://discord.vrlabs.dev).
