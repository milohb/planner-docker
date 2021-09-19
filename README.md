# Dockerfiles for planner public transport information system

This repo contains dockerfiles needed for the public transport information system described in the milohb/planner-pulumi repo:

* initcontainer is used as kubernetes init container for photon and tileserver-gl
* otp is the OpenTripPlanner
  * you need a OTP jar file named 'otp-2.jar' inside your directory or change the dockerfile accordingly
* photon is the photon geocoding software by komoot
  * you need a photon jar file named 'photon-0.3.5.jar' inside your directory or change the dockerfile accordingly

The needed digitranit-ui container is build from the dockerfile in milohb/digitransit-ui

