# PRAT

## Objective 
Identify real-world Redis performance blocks with varying client and server configurations in a virtualized environment.

## Method
Leverage Hashicorp terraform and a distributed test environment to provision and run test-suites across any number of devices.  

## History
After Meltdown/Spectre, I started to see anomalous CPU and network activity on Redis environments running in AWS' Elasticache.  PRAT was conceived and developed to provide a way to leverage Redis' standard redis-benchmark tooling to better simulate distributed loads of varying state (e.g. consistent behavior vs. flushed cache).  The overall goal being to understand how an Elasticache Redis server looks in various levels of blocking post Meltdown/Spectre.  

The solution should be extensible to other Redis test loads, however its initial conceit and implication will be solely to abuse the ever-loving crap out of Redis in an idealized virtual environment.  What people want to do with it after that, is up to them.  

Also I suck at coding, so there's that.

--GM
