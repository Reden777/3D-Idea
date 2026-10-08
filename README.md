# 3D Idea
A G3D 6.10-like renderer in 1 html file that will someday have SPOOK-like bounciness (PHUN) as an optional mode. In Version2.html, you can right click to spawn more red Gouraud shaded balls. All 3d shaders & everything it needs are included in the one file.

I am actually unsure if I want it full Roblox or mixed PHUN Physics in Roblox. Or even a separate, different engine:

1. Mixed Phun & Roblox would be an unique idea.
2. Pure Roblox already exists by itself and it has other preservation projects like Novetus. However, it's true that Novetus, the classic era of Roblox, does not run in mobile; while there are retro emulators within commercial Roblox itself, they sometimes have [unavoidable sometimes, sadly] differences compared to genuine old Roblox clients.
3. Therefore, mobile Roblox POSSIBLY satisfies that need, plus (last I heard) they still have the classic Gouraud renderer when you turn Graphics Quality down to 1-2.
4. Therefore, the combined idea is better to realize here.
5. (or the different engine idea...)

Some comments:

In Phun: The physics engine (SPOOK) was looser, springier, and far more chaotic. Things had a bouncy, rubbery, slightly unpredictable elasticity. If you built a chaotic machine, it would violently shake, flex, or glitch-explode in hilarious ways.

One of the most beloved features in Phun was the liquid simulation (SPH particles):
In Phun, water was gelatinous, bouncy, and had an almost magical "toy slime" feel to it. It splashed violently and sloshed with high energy.

Phun felt like dumping a bucket of bouncy plastic toys onto your living room floor.

SPH stands for Smoothed-Particle Hydrodynamics.
Instead of treating liquid or soft matter like a giant sheet of polygons, SPH breaks matter down into thousands of individual particles. Crucially:
Every single SPH particle is already a sphere.
Each particle has an invisible spherical influence radius (h).
When neighboring spheres get inside each other’s radius, they calculate density, pressure, and viscosity. If they are pushed together, pressure forces them apart. If they drift too far, cohesion pulls them back together.
In short: SPH is literally just smart spheres communicating with each other through force fields.
