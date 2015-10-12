WCAG/WUHCAG 2.0 JSON
===============

The WCAG 2.0 guidelines in JSON format. This special release of the WCAG Guidelines has been suplimented with content from the [Wuhcag.com checklist](https://www.wuhcag.com/wcag-checklist/). We added this content because it is much easier to understand than the docs as is.

## Contributing
The project is [Grunt](http://gruntjs.com/)-based and leverages YAML partial files that are converted to JSON format and then compressed into a single file.

**Important**
You should only edit `/src/*.yml` files. When ready to build run the `grunt build` command. If you get errors double check your YAML formatting.

### Setup
`npm install` will setup the required modules
`grunt build` will build the JSON files.

## Yaml outline:
``` yaml
guidelines:
	1.1.1:
		id: "..."
		title: "..."
		description: "..."
		uri: "http://www.w3.org/TR/WCAG20/#text-equiv-all"
		techniques:
			- "..."
		wuhcag_summary: "..."
		wuhcag_detail: |
			...
		wuhcag_related:
			- "..."
```