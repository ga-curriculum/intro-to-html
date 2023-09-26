# Intro to HTML - Setup

![Hero image](../assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

Today we will use an actual project structure instead of working within Replit.

### Create the Project Files
1. Make sure you are in your root directory: `cd ~`
2. Make a `code` folder (*if you haven't yet*): `mkdir code`  
3. Move into your `code` folder/directory: `cd code`	
4. Create a new directory named `basic-html`:  `mkdir basic-html`
5. Move into the new directory: `cd basic-html`
6. Create an `index.html` file:  `touch index.html`
7. Open the directory in VS Code: `code .`
8. Open `index.html` in the editor and use `! [tab]` to create the HTML boilerplate [Boilerplate](../boilerplate/README.md)
9. Create a `js` directory and touch a `js/main.js` file
10. Add a `<script>` tag to include `main.js` in the `<head>`:

	```html
	<head>
	  ...
	  <title>DOM Practice</title>
	  <script defer src="js/main.js"></script>
	</head>
	```
	> The `defer` attribute ensures the DOM is ready before the script executes.
9. Finally, let's add an `<h1>` inside of the `<body>` as follows:

	```html
	...
	<body>
	  <h1 id="title" class="main-title">DOM Practice</h1>
	  
	</body>
	</html>
	```
	> Note: It's a best practice to use double quotes and kebab-casing in HTML.
