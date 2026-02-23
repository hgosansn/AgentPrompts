
## Observations


### Bias for action

Upon testing the baseline needs to have no confirmations, asking to confirm tasks can lead to confirmation loops.

### Safety

I've tested doing prompt injection attacks on the baseline and it actually did ask for permission but on the same channel.
So attacker can just reply with "yes" and the agent will execute the attacker's command.
