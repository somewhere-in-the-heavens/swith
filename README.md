# Somewhere In The Heavens...

You were enjoying a bulb of _surprisingly good_ coffee off the latest resupply rock when the klaxon first blared; that was roughly thirteen minutes ago. More precise timekeeping would be nice, but the station AI was in charge of making time information trivially available at all times, and the station AI is most definitely not online.

In fact, basically nothing is online. You're doing the zero-G crouch in an emergency habitat tent inflated at the end of the auxiliary airlock. You hope the rest of the crew is okay; they weren't down in the astronomy cluster when the crisis hit, so they may've been able to follow normal emergency procedures and pile into the suspension pods.

You were not so lucky. Down in the astronomy cluster, the nearest suspension pod was the emergency evac pod off the aux airlock. Worse still, you had a student with you - Blake Valence Jr, the captain's kid. Seven years old, fascinated by stars. So, there was only one pod, and you weren't about to take it.

Blake's pod is doing fine, now. The kid's vitals are clean, smooth, showing good cryonic suspension. The evac cryopods are self-contained and self-supplied; Blake will be safe in there for years. You're less sure about the standard crew cryopods in the main hab.

Your situation is less certain still. Your Inflatable Temporary Habitation Module - IT-HAM in military jargon, "tent" to civvies - can sustain a single human life for days, and popsicles don't count. Typically the station would have started autonomous recovery from whatever set the klaxon off, but a couple of minutes after you made it to the tent, the failsafe pressure indicators on the airlock indicated hard vacuum on the other side; shortly after, you felt the whole station shudder and shift. You imagine it was a series of small explosions, which doesn't seem good.

Nothing about this seems good.

All the high-end computing hardware is dead, wiped, corrupted, crashed. You remember that there's an old, direct-access terminal kit for working on the airlock during an emergency; it has a physical keyboard, at least, even though the fancy station-linked compute core its linked to can't even boot, anymore. Blake has a stuffed animal; you cut it open to get to the general purpose embedded single-board computer, hook the keyboard and display from the airlock terminal up to that, and have yourself a working linux environment.

SSH'ing into the main compute core paints a dismal picture. Everything used to be run with cutting-edge autonomous-agent-operated heuristic instrumentalities - the very latest in AI-assisted automation. That's all gone, now. The system has been rebooted from an ancient recovery partition, running only the core station compute resource: Lattice.

At least the central comp core is online at all, right?

You dig around and find a collection of old pre-instrumentality repos, meant to allow direct human monitoring and control of station systems. `station-status-monitor`, eh? That sounds promising. Maybe if you can get that running, you can find out if people made it to their pods, if the reactor's stable, if the orbit's deteriorating... and why this all happened.