<div align="center">

# Rigidbody Launcher

[![Generic badge](https://img.shields.io/github/downloads/VRLabs/Rigidbody-Launcher/total?label=Downloads)](https://github.com/VRLabs/Rigidbody-Launcher/releases/latest)
[![Generic badge](https://img.shields.io/badge/License-MIT-informational.svg)](https://github.com/VRLabs/Rigidbody-Launcher/blob/main/LICENSE)
[![Generic badge](https://img.shields.io/badge/Unity-2019.4.31f1-lightblue.svg)](https://unity3d.com/unity/whats-new/2019.4.31)
[![Generic badge](https://img.shields.io/badge/SDK-AvatarSDK3-lightblue.svg)](https://vrchat.com/home/download)

[![Generic badge](https://img.shields.io/discord/706913824607043605?color=%237289da&label=DISCORD&logo=Discord&style=for-the-badge)](https://discord.vrlabs.dev/)
[![Generic badge](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Fshieldsio-patreon.vercel.app%2Fapi%3Fusername%3Dvrlabs%26type%3Dpatrons&style=for-the-badge)](https://patreon.vrlabs.dev/)

Launch an object with collision against the world

![RigidbodyLauncher](https://github.com/VRLabs/Rigidbody-Launcher/assets/76777936/c475c245-c1f9-4360-ae27-72c2daebb460)


### ⬇️ [Download Latest Version](https://github.com/VRLabs/Rigidbody-Launcher/releases/latest)

<!-- 
### 📦 [Add to VRChat Creator Companion]() -->

</div>

---

## How it works

* A configurable joint is connected to a [world-constrained](https://github.com/VRLabs/World-Constraint) kinematic rigidbody and given velocity on the Z-axis.
* The joint has collision and stops against the world.
* A particle system under the joint dies with collision, causing a [particle stop action disable](https://docs.unity3d.com/ScriptReference/ParticleSystemStopAction.html), triggering a contact-driven parameter change.

## Install guide

https://github.com/VRLabs/Rigidbody-Launcher/assets/76777936/9f288264-7a4b-4790-b6c3-38a1180a3ea5

* Merge the Animator Controller ``Rigidbody Launcher FX`` to your own FX Controller, using the [Avatars 3.0 Manager](https://github.com/VRLabs/Avatars-3.0-Manager) tool.
* Drag & drop the ``Rigidbody Launcher`` prefab into the base of your Hierarchy.
* Right click and unpack the prefab, then drag & drop it onto your avatar.
* Move ``Rigidbody Launcher Target`` outside of ``Rigidbody Launcher`` and place it anywhere in your avatar's hierarchy. Adjust the transforms as needed.

## How to use

* Place the objects you want to to use inside ``Rigidbody Launcher`` -> ``Container``.
  * Alternatively you can constrain the objects to ``Container``.
* ``RigidbodyLauncher/Control`` parameter must be true for the system to fire, and false to reset.
* To change speed, you can edit the ``Launcher Fire.anim`` animation clip and change the ``Target Velocity``. You need to use a negative value.
  * You can also change the ``Maximum Force`` property under the ``X/Y/Z Drive`` sections of the ``Rigidbody Launcher/Kinematic Rigidbody/Collision`` configurable joint.
  * Other properties of the joint on ``Collision`` are editable depending on the rigidbody motion you want to achieve.
* To launch the rigidbody perfectly straight, freeze rotation for XYZ on the ``Collision`` rigidbody (not the configurable joint), and set the X and Y motion on the ``Collision`` configurable joint as locked.
  * This will make it so only Z-axis motion is possible.

## Performance stats

```c++
Audio Sources:      2
Colliders:          1
Constraints:        4
Contact Receivers:  1
Contact Senders:    1
FX Animator Layers: 2
Lights:             1
Particle Systems:   1
Rigidbodies:        3
```

## Hierarchy layout

```html
Rigidbody Launcher
|-Container
|  |-Cube
|  |  |-Point Light
|  |-Collision Audio
|  |-Fire Audio
|-Kinematic Rigidbody
|  |-Collision
|  |  |-Box Collider
|  |  |-Contact
|-Rigidbody Launcher Target
```

## Contributors

* [lin](https://github.com/oofdesu)

## License

Rigidbody Launcher is available as-is under MIT. For more information see [LICENSE](https://github.com/VRLabs/Rigidbody-Launcher/blob/main/LICENSE).

​

<div align="center">

[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/VRLabs.png" width="50" height="50">](https://vrlabs.dev "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Discord.png" width="50" height="50">](https://discord.vrlabs.dev/ "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Patreon.png" width="50" height="50">](https://patreon.vrlabs.dev/ "VRLabs")
<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Empty.png" width="10">
[<img src="https://github.com/VRLabs/Resources/raw/main/Icons/Twitter.png" width="50" height="50">](https://twitter.com/vrlabsdev "VRLabs")

</div>

---
