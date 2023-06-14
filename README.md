# SLASS
SLicer AS a Service (because SLAAS looks silly)

The goal of this project is to create a single API with common slicer settings for popular slicers (starting with PrusaSlicer, Cura, BambuSlicer) and wrappers to call these APIs as a web service or from a command line interface.

This will allow easy testing of multiple slicer versions, web or mobile slicing with a remote host, comparisons of slicers and the ability to create better front ends for slicers (which in my opinion are very much needed).

The project will be written in node.js. If you are interested in helping, reach out. 

# Implementation
Unfortunately, to my knowledge most slicers do not currently expose an API (hence this project). To interface with the slicer we will either need to:
* Generate configuration files on the fly
* Create pull requests back to the original slicer with changes allowing API or CLI access
* Worst case: Maintain a separate API enabled fork of the slicer. (This would require manual intervention if the fork encounters merge-conflicts upon a new release)

Creating configuration files on the fly is the easiest starting point and should cover most scenarios.

# Road Map
The minimum viable product should 

# Licensing
The plan is to license the code under a commercial software friendly license, such as MIT. To avoid distributing other slicer code, we can add the ability to download those during setup from the official repositories.
