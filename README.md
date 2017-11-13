# SpikeyNUC Workshop

This repository contains the tutorial material for *SpikeyNUC*-based tutorial.


## Rationale

*SpikeyNUC* provides:

* the capability to run experiments on locally attached Spikey and BrainScaleS-DLS systems
* utilizes JupyterHub provides per-user Juypter sessions
* provides arbitrated access to the local chips (tested up to 30 users)

The typical setup comprises:
* the SkullNUC (ESSID: `DemoBrainScaleS`, usually hidden)
* two Access Points providing WiFi access for large numbers of users
  (ESSID: `DemoBrainScaleS1`, `DemoBrainScales2`)
* a laptop (of the tutor) providing access to the Internet (using DNAT)

After joining one of the WiFi networks, the user can access the demo machine.
Currently, the machine's IP address is provided by the tutor (i.e. no name lookup yet)
to the users. A HTTP server (port 80) provides a welcome page providing links to the
interactive part of the tutorial and a snapshot of the Spikey School documentation.
Users can now open individual Jupyter sessions to interactively work with the systems.
After logging in example notebooks are copied into the individual home folders and can
be opened by the user.
The main workspace (which is copied to the temporary user sessions) can be found in
`~/spikey-workshop`.


## Internal Information and Administration

* Ask @khs, @mueller or @kindler for admin passwords
