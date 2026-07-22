# Coruscant-Garden
Building a browser theme that breathes: Coruscant Garden, my first published Opera GX mod

I wanted a project that let me combine three things I love — Star Wars lore, flower design, and full-stack build work — into something people could actually install and use every day.

The concept: Coruscant, 19 BBY, but reimagined as if the plant life of Akiva and Kashyyyk had crept up through the durasteel. I swapped in my personal favorite flowers — hydrangea, white lion daffodil, peony, and snowdrops — climbing over balconies with the galactic capital's spires glowing in the distance.

From there it became a real engineering project, not just a wallpaper:

- Designed and generated dark/light scene variants, then iterated on composition until the flowers read correctly (an early pass dropped the peonies entirely — small reminder that prompt specificity matters as much as code specificity)
- Converted still frames into looping animated wallpaper — moving traffic, flickering neon signs, swaying petals — using image-to-video generation, then hand-built a seamless loop in ffmpeg with a crossfade transition so the seam is invisible
- Sourced and licensed a royalty-free ambient track, wired it into a JSON manifest with vertical-remixed background music, and wrote the full Opera GX mod schema (wallpaper, theme colors, icon, credits) from scratch
- Packaged, tested locally via unpacked-extension loading, then published through GX.create to the public GX Store

It's a small project, but it touched a lot of the same muscles I'm building toward full-stack work: asset pipelines, media processing, schema design, packaging, and shipping something a real user can install.

Coruscant Garden is live on the GX Store now — (https://store.gx.me/mods/ndwsfy/coruscant-garden/). Would love feedback from anyone who tries it out, and always happy to talk shop about the ffmpeg loop trick or the manifest structure if you're curious.
