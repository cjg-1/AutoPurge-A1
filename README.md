AutoPurge A1 lets your Bambu Lab A1 automatically clear the build plate between jobs so a queue can run end-to-end without you standing by. A small bolt-on, 3D-printed scraper mounts to the toolhead and gently pushes finished parts off once the bed cools into the release range. The motion routine brings the nozzle to a safe glide height, sweeps the plate, catches the corners, and homes—leaving the surface ready for the next print. 

The companion AutoPurge Merger app (simple GUI) takes multiple G-code files you’ve sliced in Bambu Studio and combines them into one continuous print file. It inserts the AutoPurge “MID” sweep between each job automatically, and—if you choose—adds a final “FINISH” sweep at the very end. The app also removes a few specific shutdown lines that can halt queued motion, and verifies the output so the printer can hand off cleanly from print to purge to next print.

To use it, install Python (or build the Windows one-file EXE), run the Merger, paste your G-codes in order, and save the combined file. Mount the printed scraper, create a duplicate printer profile in Bambu Studio with the provided End G-code text, and start your queue. The result is unattended, multi-job runs with a reliably cleared plate between prints.

Make sure to go through all the README files, as they are crucial to understand in order for Autopurge to run correctly.


Important: Please keep in mind that every item printed with Autopurge assistance is recommended to be at least 7 MM tall in order to prevent jams. 


DISCLAIMER: Description is AI-assisted as well as part of the GCODE additions
