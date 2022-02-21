# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

Analysis:
	App Service:
		- Cost. The cost  factor is cheaper as there are less resources involved and additional apps can \
		can be leveraged to share the same Service plan.
		- Scalability. Can scale horizontally and vertically and can do so automatically with  auto-scaling \
		There are limits to how much compute can be aligned with App Service plans.
		- Availability.  App Services can be made highly available, not as much as a VM, but it is much simpler \
		and cheaper to configure with an App Service.
		- Workflow. App Services can have code deployed to them very quicly and easily.
	Virtual Machines:
		- Cost. More expensive than App Services but can be configured more granular.
		- Scalability. Can scale horizontally and vertically. They can provide more compute resources if needed \
		than App Services.
		- Availability. Higher availablility than App Services but require more configuration.
		- Workflow. Code deployment needs to coincide with other considerations such as OS upgrades, OS patching, \
		global library version, etc. 

Choice:
	I have chosen App Service for this deplyoment of the CMS app.

Justification.
	There were no special needs or requirements that demanded a VM be used. there were no security requirements that \
	would require hardening/changing the OS. No cpu/mem requirements that the App Service plan couldnt achieve and the \
	cost is cheaper.	

