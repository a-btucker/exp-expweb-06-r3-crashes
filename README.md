exp-expweb-06-r3-crashes
========================

This is to keep track of the current status of things that are going on with expweb-06-r3 crashes.


## Current Tracks

We are going to go after the following items one at a time to see which ones have the effect of stopping the crashes.

### Shutdown expweb5551 on all servers
* **Current Status** Evens are done - In progress 

### Start process of getting Hao's zip fix build and prepared for propping
* **Current Status** Aaron has unshelved change, and is in progress of running PCP

### Roll Back to 06-R1 JVM settings
* **Current Status** Pending

### Stop recent abacus experiments
* **Current Status** Pending

### Gather forensics on servers that have crashed
* **Current Status** Pending
* We will want to take each server that has crashed and gather
  * Up Time
  * ???

# Reference information

## Splunk query that shows crashes
* index=app sourcetype=expweb_crash_dump | transaction keepevicted=true host _time | stats count by host _time

