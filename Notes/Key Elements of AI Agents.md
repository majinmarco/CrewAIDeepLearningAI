# Key Elements of AI Agents

- Role Playing
	- Role playing instructions should be very granular. Take note of precise keywords being used to influence the agents' comportment.
	- Roles, goals and backstory

- Focus
	- Placing too many duties on a single agent will make models lose important information, opening the door to hallucinations.
	- The amount of tools accessible is also very influential on an agent's focus

- Tools
	- Do not give a lot of tools to a single agent
	- You do not want to end up with a jack of all trades, master of none

- Cooperation
	- Collaboration creates a huge difference in outcomes
		- Take feedback
		- Delegate tasks

- Guardrails
	- Important to limit agents to their duties.
	- Guardrails also introduce help for smaller models that loop through using the same tools over and over.

- Memory
	- Memory informs new decisions and future executions.
	- Out-of-the-box, CrewAI provides agents the following types of memory:
		- Long-term memory
			- Memory stored after execution of current tasks
			- Can be used in any future tasks
			- Leads to "self-improving" agents

		- Short-term memory
			- Memory during execution of a task.
			- Share knowledge, activities, and learnings with other agents.
			- Share intermediate information even before providing "task completion" output.
		
		- Entity memory
			- Stores entities in context and input
			- Reliable and increasingly better agents