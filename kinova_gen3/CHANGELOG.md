# Changelog – Kinova Gen3 Description

All notable changes to this model will be documented in this file.

## [2026-11-10]
- Added a contact exclude between `base_link` and `shoulder_link`. Their collision meshes overlap by 12 mm, and because `base_link` is welded to the world, MuJoCo's automatic parent-child filtering does not apply, so `joint_1` could not rotate.

## [2026-09-13]
- Added joint armature to stabilise the low-inertia joints with the existing position-controller gains.

## [2024-06-28]
- Initial release.
