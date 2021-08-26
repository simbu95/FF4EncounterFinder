Maximum number of steps: Number of steps until giving up on the first encounter and resetting 

Maximum number of encounters: Maximum number of encounters to search. If a fight can't be guarenteed in less encounters, suggest a reset. 

Seconds per step: Used to calculate average time to find a battle. This is how long it takes you to count a step when walking around.

Seconds per encounter: Used to calculate average time to find a battle. This is how long it takes to run or kill the encounters where you are manipulating. 

Seconds per reset: USed to calculate average time to find a battle. This is how long it takes you to see your current step is bad, reset the game, and start walking again. 

Location Name: This is an identifier for which location you can find your battle at. 

Encounter Indexes: This is to mark all the slots the encounter you are looking for has for a particular location. 

How To Use:

Set the above parameters as you like. You may want to refer to a a guide to find out where your particular encounter can be located, and which slots it occupies

You can enter in multiple locations for your encounter. This will greatly increase the rate of finding the encounter if different encounter indexes are used. 

Once you press calculate step manipulations, you will be shown how many seeds (out of 256) will result in finding a battle. As well you will be given an average estimate of how long it will take to complete the manipulation for the battle. This includes the potential for resetting (multiple times) attempting to perform the manipulation. 

You will also be given a list of what an encounter on a specific step means. If a step says Encounter 3 is your desired fight, it is assumed you will take 2 more encounters, then set encounters to off, walk to your destination, turn encounters on, and get in the fight. 

Otherwise standard manipulation rules should apply. You should be outside baron, turn encounters on, save, reset and load the save, and then count steps. It is worth noting that if more encounter locations are added, there are some tiles that don't count as steps, usually a bridge or staircase that will not increase the step counter. 

Notes:

Currently only supporting manipulations at Baron. 

The average time to find a battle includes resetting. The math should be correct, but might be wise to verify. The current math could probably be simplfied a lot, and better organized. 

Time is not included to travel from baron to your destination. It is also assumed that you continue taking fights at baron until the next encounter is the one you desire (this time is accounted for). Since keeping track of steps to the location of your encounter isn't possible, you may also spend some time walking after arriving to find an encounter. 

The default values were mostly chosen at random. It is suggested that you time yourself, and use those values if you are tring to optimize based on time. 
ToDo:

Improve Formatting: Improve html/css layout, display manipulation data better, potentially generate a graphical representation. 

Formation Data: Allows using formation data of the first encounter to improve accuracy.  

Other Locations: Allows chosing from several locations for generating the manipulation data. 

Common Searches: A list of location/encounter data that is commonly desired. This could be ueful grinding locations, encounters for Edge to steal useful items, etc. 

Encounter Chain: Allows a chain of encounters to be considered. i.e. It could be the 2nd or 3rd encounter in a location. This is most helpful when running is allowed, and the formation you are looking for is visually unique at the start of the battle. 

Second Encounter: Allows using the steps to the second encounter to decide to reset or not. 

Iterative Optimization: Instead of specifing a set number of max encounters/steps, Use the time calculation for each encounter step to determine if it is optimal to reset, or continue searching. 