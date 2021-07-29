# iso-assignment

## Task

Create a microservice, that is able to tak as an input an country ISO code and a list of country names (in different languages) and will filter out just the countries that correspond to the provided ISO code.

Serve the application as the API.

### Example

Request:

```
POST /match_country

{
	"iso": "svk",
	"countries": [
		"iran",
		"Slowakei",
		"Vatikan",
		"Slovaška",
		"Szlovakia",
		"Belgrade",
		"España",
		"Nizozemsko"
	]
}
```

Response:
```
{
	"iso": "svk",
	"match_count": 3,
	"matches": [
		"Slowakei",
		"Slovaška",
		"Szlovakia"
	]
}
```

## Requirements

- Showcase all your best skills. The assignment is small (just mvp), but try to include any improvement that you can, e.g.:
  - test coverage
  - api documentation in Open API 3.0
  - data storing and caching
  - docker
  - CI/CD
  - FE interface
  - anything else you'd like (these are just some exmamples that you can include)
- Structure the application properly
- Make it easy for extention of functionality
- Sumbit as a link to your github repository with the solution
- Include README.md with the description and how to run the application
- Include the example output from stdout (& tests if applied)