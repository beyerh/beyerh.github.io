---
{"dg-publish":true,"permalink":"/py-mol/7-animations-movies/","title":"Exercise 7: Animations and Movies"}
---

# PyMOL Exercise 6: Animations and Movies

This exercise will teach you how to create simple animations and export movies directly from PyMOL. Animations are an excellent way to visualize structural changes, binding events, or showcase a complex molecule from different angles.

---

## **Step 1: The Basics of PyMOL Movie Making**

Before creating a movie, you need to set the total number of frames. PyMOL uses a frame-based animation system.

1. Open PyMOL and load a structure, for example: `fetch 1mbo` (Myoglobin).
2. Set up your initial view (e.g., `show cartoon`, `color cyan`).
3. Set the total number of frames to 120 (for a 4-second movie at 30 frames per second):
   ```pymol
   mset 1 x120
   ```
   *`mset` stands for movie set. `1 x120` means state 1 will be duplicated across 120 frames.*

4. You should now see the movie timeline bar at the bottom of the PyMOL viewer. You can click play to run through the frames (nothing will move yet).

---

## **Step 2: Simple Camera Rotation (Y-axis Spin)**

The easiest animation is a simple 360-degree rotation of the molecule.

1. Tell PyMOL to rotate the camera along the Y-axis over the course of the movie:
   ```pymol
   util.mroll 1, 120, 1
   ```
   *(This tells PyMOL to roll the camera from frame 1 to 120, completing 1 full rotation).*
2. Press the **Play** button in the bottom right corner to see your molecule spin.
3. If you want to clear the movie and start over, type `mclear`.

---

## **Step 3: Keyframe Animation (Interpolating Views)**

For more complex camera movements, you can store specific views (keyframes) at different frames, and PyMOL will automatically calculate the smooth transitions between them.

1. Clear any previous movie: `mclear`
2. Set up a 90-frame movie: `mset 1 x90`
3. Go to **frame 1** by clicking on the timeline or typing `frame 1`.
4. Position your molecule so you see the whole structure. Store this view as a keyframe:
   ```pymol
   mview store
   ```
5. Go to **frame 30** (`frame 30`). Zoom in on the heme group (`zoom resn HEM`).
6. Store this new view:
   ```pymol
   mview store
   ```
7. Go to **frame 90** (`frame 90`). Zoom back out to the full structure.
8. Store this final view:
   ```pymol
   mview store
   ```
9. Play the movie. PyMOL will smoothly interpolate the camera between your stored views.

---

## **Step 4: Exporting the Movie**

Once your animation is ready, you can export it as a video file.

1. Set the movie generation quality (ray tracing makes it look better but takes longer):
   ```pymol
   set ray_trace_frames, 1
   ```
   *(Set to `0` for a faster, lower-quality export without ray tracing).*
2. Save the movie as an MPEG or MP4 file:
   ```pymol
   movie.produce my_animation.mp4, quality=90
   ```
   *(Note: Depending on your PyMOL installation, you may need to export as individual PNG frames (`mpng frame_`) and compile them with a tool like FFmpeg if the direct video export fails).*

---

### Summary

1. Use `mset` to define the length of your movie.
2. Use `util.mroll` for quick, automated rotations.
3. Use `mview store` at specific frames to create custom, interpolated camera paths.
4. Export the final animation using `movie.produce`.

---

[[PyMOL/6_scripting\|← Previous]]
