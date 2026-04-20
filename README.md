# malcolm-code
i aim to misbehave


# i like narnia and firefly

here is a design for a functional, flying, tiltrotor edf drone based on Serenity, designed using Claude AI.

The specifications, as of Revision D:

2 x 70mm EFDs in the nacelles.
1 x 40mm EFD in the fuselage.
variable diameter thrust tubes remixed from:
Variable-area EDF nozzle
by BamJr
licensed under the Creative Commons - Attribution license.
https://www.thingiverse.com/thing:2991269

the drone is controlled by a raspberry Pico 2 with a custom sensor hat with GPS, imu, barometer, airspeed sensor connection, fpv camera, and control output for ESCs, nacelle and nozzle servos, payload release and winch, and navigation and anti-collision lights, all securedby a tpm.  jst gh connectors expose can fd (with selectable terminal jumper) and ethernet.
it's networked to a raspberry cm4 with 4gb ram on a carrier board with a tpm, 2.4ghz and 5ghz wifi and zigbee, a tf slot for an os micro SD with a forensicly sound write blocker and a pi zero 2 x 20 gpio header, with internal and sma antenna connections.

attached to the headder is a comms and recorder hat with its own tpm, 915mhz mavlink mavlink and lora radio, 49mhz rcrs time division dual simplex transceiver with dynamic channel assignment,and a tf slot for a micro sd card with hardware enforced non-executable log storage. the hat has can fd and ethernet with jst gh connectors, which allows dual routes for intra-platform network and signaling. 
