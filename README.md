# Vue CDN Template

This repo contains a boiler-template for minimal Vue and TailwindCSS web applications.

It is perfect for testing and prototyping purposes.


## Adding the template as a user snippet to VS Code

This template can be used as a user snippet for html files in VS Code. In order to add the snippet, follow these steps:

1. On MacOS, click on Code > Preferences > User Snippets
1. Click on 'html'
1. Add the following script:

```json
	"Vue3 TailwindCSS Boilerplate": {
		"prefix": ["vuetail", "vue-tail", "vue-tailwindcss"],
		"body": [
			"<!DOCTYPE html>",
			"<html class=\"antialiased leading-tight\">",
			"\n<head>",
			"\t<meta charset='utf-8'>",
			"\t<meta http-equiv='X-UA-Compatible' content='IE=edge'>",
			"\t<title>Template</title>",
			"\t<meta name='viewport' content='width=device-width, initial-scale=1'>",
			"\t<script src=\"https://unpkg.com/vue@next\"></script>",
			"\t<link href=\"https://unpkg.com/tailwindcss@^1.0/dist/tailwind.min.css\" rel=\"stylesheet\">",
			"</head>",
			"\n<body>",
			"\t<div id=\"app\">",
			"\t\t<!-- Your App Here -->",
			"\t</div>",
			"\t<script>",
			"\t\tconst App = {",
			"\t\t\t//App Data Here",
			"\t\t}",
			"\t\tconst app = Vue.createApp(App)",
			"\t\t//Your Components Here",
			"\n\t\tapp.mount('#app')",
			"\t</script>",
			"</body>",
			"\n</html>\n"
			
		],
		"description": "A Vue 3 and TailwindCSS CDN template."
	}
}
```

1. Save snippet

You will now be able to call the code snippet in VS Code by typing *vuetail*, *vue-tail*, or *vue-tailwindcss* and clicking enter.
