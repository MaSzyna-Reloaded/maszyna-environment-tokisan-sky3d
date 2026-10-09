# MaSzyna environment - Tokisan Sky3D

A sky backend for libmaszyna's `MaszynaEnvironmentNode`, drawn by
[Sky3D](https://github.com/TokisanGames/Sky3D) (Tokisan Games): `SkyDome` with `TimeOfDay`, the
sun and the moon, clouds and fog following the environment's cloudiness, wind and fog.

`TokisanSky3DMaszynaEnvironment` extends libmaszyna's `MaszynaSkyEnvironment`, so it is set up
the same way as any other sky backend.

## Requirements

* libmaszyna (`addons/libmaszyna`) - `MaszynaEnvironmentNode` and `MaszynaSkyEnvironment`
* Sky3D 2.1 in `addons/sky_3d`, its plugin enabled

## Installation

1. Copy (or link) `addons/maszyna_environment_tokisan_sky3d` into your project's `addons/`.
2. Install Sky3D into `addons/sky_3d` and enable it in Project Settings -> Plugins.

## Use

Add a node with the `TokisanSky3DMaszynaEnvironment` script to the world scene and point its
`environment_node_path` at the scene's `MaszynaEnvironmentNode`. It creates its
`WorldEnvironment`, the sun and moon lights, `SkyDome` and `TimeOfDay` itself; the time of day
follows the simulation's clock, or the system time when the environment node uses it.
