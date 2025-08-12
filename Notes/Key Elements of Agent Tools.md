# Key Elements of Agent Tools

- What makes a great tool?
	- Versatility
		- Be able to accept different types of requests
		- Fuzzy inputs
		- Strongly typed outputs
	- Fault tolerance
		- Things might break when you give agents tools
		- Fail gracefully and try again (implemented by default)
			- Send error message back to agent
			- Ask agent to retry given the error message
	- Caching
		- Take the time to do the request and know when not to
		- Caching layer prevents unnecessary requests
		- Cross-agent caching: tool results are cached; if two agents are using the same tools with the same set of arguments, API call is not remade (would provide the same results)

- Examples of tools
	- Search the internet
	- Scrape a website
	- Connect to a database
	- Call an API
	- Send notifications
	- ... and many more

- Exceptions
	- Handling exceptions is very important (restart execution, move on, or something else?)

![1755019426318](image/KeyElementsofAgentTools/1755019426318.png)