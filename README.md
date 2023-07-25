Well...After a few days of trying to figure this out, I finally finished my SIEM in Azure. I will not try to explain everything I did because that will take too long. However I will talk about the main things that went into this project.

These are the main programs that I used to make this possible:
Virtual Machine
Log Analytics
Microsoft Sentinel
Microsoft Defender

I used virtual machine as a honeypot and with the combination of the other three programs, created a map of where the attacks on my honeypot are coming from.

The virtual machine ran a script that created a log of the failed attempts and that log was sent to Log Analytics. From Log Analytics, I was able to parse out the data coming from the logs to send to Microsoft Sentinel and that program created a map of where the attacks are coming from.

I let it run for a full 24 hours and just look how many attacks there were on this machine in only that small amount time. It's crazy. But this lab was fun. It gave me a chance to work with Azure which I never worked with before. I didn't realize it was just like AWS, but with that said, on to the next project!
