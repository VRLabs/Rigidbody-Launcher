# Rigidbody Launcher
  
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-informational.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-informational.svg)](https://vrchat.com/home/download)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Rigidbody-Launcher/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Rigidbody-Launcher/total?label=Downloads)](https://github.com/VRLabs/Rigidbody-Launcher/releases/latest)

Launch an object with collision against the world.

## How it works

A configurable joint is connected to a world-constrained parent kinematic rigidbody and given velocity on it's free Z-axis. The joint has collision and stops against the world. A particle system under the joint dies with collision, causing a stop action disable, triggering a contact-driven parameter change.

## Preview

https://user-images.githubusercontent.com/45078979/168454568-639289fe-722f-496f-9209-bbc07eef3620.mp4

## Install guide

https://user-images.githubusercontent.com/45078979/168454577-6244e54b-6531-4861-bfde-2265e35c88ab.mp4

Merge the FX controller from this package to your own FX controller, using the [Avatars 3.0 Manager](https://github.com/VRLabs/Avatars-3.0-Manager) tool.
 
"Rigidbody Launcher.prefab" should go to the base of your Unity scene, which will give it base Unity scaling.

Unpack the prefab by right-clicking it.

Place "Rigidbody Launcher" at the base of your avatar.

Remove "Rigidbody Launcher Target" outside of "Rigidbody Launcher" and place it anywhere in your avatar's hierarchy. Adjust the transforms as you need.

## How to use

**"RigidbodyLauncher.Control" parameter must be true for the system to fire, and false to reset.**

To change speed, you can edit the "Fire.anim" clip and change the "Target Velocity". You can also change the "Maximum Force" property under the "X/Y/Z Drive" sections of the "Rigidbody Launcher/Kinematic Rigidbody/Collision" configurable joint. Other properties of the Collision joint are editable depending on the rigidbody motion you want to achieve.

## Downloads

You can grab the latest version of the Rigidbody Launcher in [Releases](https://github.com/VRLabs/Rigidbody-Launcher/releases/latest).

## License

Rigidbody Launcher is available as-is under MIT. For more information see [LICENSE](https://github.com/VRLabs/Rigidbody-Launcher/blob/main/LICENSE).

## Contact us

If you need help, our support channel is on [Discord](https://discord.vrlabs.dev).
