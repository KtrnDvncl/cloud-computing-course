# Final Reflection: From Trainee to Enterprise Cloud Architect

Looking back at where we started in Mission 1, learning basic Linux commands, reaching Mission 10 feels entirely surreal. When we first read the mission brief from our "CEO" and saw the strict rule—*no step-by-step guides*—there was definitely a moment of panic. We were no longer just following a manual; we were expected to write one. 

Taking off the training wheels was intimidating, but it was exactly what we needed to realize how much we’ve actually learned. We chose to deploy a WordPress and MySQL stack. In previous labs, we might have just copy-pasted a `docker-compose.yml` file without thinking twice. But this time, we had to truly understand every line of code to ensure our database utilized persistent volumes so our data wouldn't vanish after a reboot. 

The hardest part wasn't necessarily writing the code, but integrating everything securely. Configuring the UFW firewall to a strict default deny policy and allowing only exactly what was needed (like SSH and our web ports) made us think like real security professionals. Writing our own Bash script for backups and automating it with a Cron job finally made all the fragmented concepts we've learned over the semester click together. It felt like we were building a living, breathing system that could take care of itself.

As a team (James, Vicel, Mark Lester, and Katrina), we spent hours troubleshooting, reading documentation, and testing our infrastructure. There were moments of frustration when containers wouldn't link or the server wouldn't boot correctly, but the satisfaction of finally running `docker compose up -d` and seeing our application go live on a fresh server was incredible. 

This project proved to us that we are no longer just passengers in the cloud. We want to express our deep gratitude to our instructor, Ma'am Jenkielyn C. Torres, for pushing us out of our comfort zones and trusting us with this "blank check" enterprise project. We are walking away from CCM101 not just as students who passed a class, but as capable Cloud Architects ready for the real world.
