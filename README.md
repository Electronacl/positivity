# Positivity
Positivity is a WIP rewrite of Anode with a goal of better performance and cross-platform compatibility. It's a NES emulator with the goal of high accuracy with real-time play.

## Plans for this project
The main idea for this project is to update the Anode emulator with C++ as opposed to C#, as well as a better UI framework like ImGui rather than Winforms.

Hopefully, by the point where this project reaches the state of Anode 2.0.0, it should be more stable and performant (on top of allowing for better 3D emulation for future plans)

Unfortunately, this project isn't guaranteed to be complete as it'll be a bit of a learning curve, as I'm having to move to a lot of stuff I haven't used before. As usual though, these projects never use Artificial Intelligence in any step of the project and the goal is to always do all of the work as human effort
(although this sometimes means looking up a LOT of stack overflow lol)

## Current status of the project
Initialisation - getting the main thing working so I can then start working on the NES emulator later

## Versioning system
-# *The versions shown here are for display purposes only and do not represent real versions of this software*
Versioning is mostly based around the semantic versioning, and has 2 separate forms: a form like `v0.1.0-alpha1 (a12)` for pre-releases and `v0.1.0` for releases.

The first part of the version name is the semantic version name. It consists of 3 numbers: `M.m.p`.
- M is the major version - this increases when a huge change or addition is made, usually drastically impacting the software.
- m is the minor version - this increases with less big changes that are still pretty important, often including many bugfixes and new features.
- p is the patch version - this increases when a small change needs to be made, such as a hotfix, bug patch, or feature addition.
For example, you could have `1.4.2`

The second part of the version is displayed on all pre-releases and *does* exist for full releases but is only included as a footnote. It is formatted as such: `-cv (bV)`
- c is the channel. This can be one of the following values:
  - `alpha`, which is the first stage of development (unstable and quite incomplete)
  - `beta`, which occurs after and is more stable and has most features but still needs quite a bit of work
  - `prerelease`, which is close to release time and is just polishing up features and patching bugs
  - `release`, which is the final release of the version
- v is the channel version. This increases every time a new build for the overall version is released, but resets to 0 once it has reached the next channel stage.
- b is the branch. Different branches may have new features but lack features from other branches. As the features may be lacking, there may be multiple of the same channel versions, e.g `1.0.1-alpha2 (a24)` and `1.0.1-alpha2 (b25)`
- V is the build version and counts up from the first release/pre-release. It never resets and can serve as an identifier if you want to list a specific version with a number. No 2 releases/pre-releases will have the same build version, even with different branches.
For example, you may have `1.4.2-beta5 (a63)`

The current branch identifiers are:
- a: main (Active)
