This plugin adds the option to insert code snippets in the rich text editor, as well as adding a custom code snippet fieldtype that can be used with custom templates to create things like Github Gist styled posts.

# Notice

If you JUST want the code fieldtype, I have a second plugin [Clean Code](https://github.com/xkisu/CraftCleanCode) which implements a standalone code fieldtype a lot cleaner and with better usage. This works better for single code fields and code blocks in a Matrix.

# Installation
Create a folder called `redactorcodesnippets` in the `craft/plugins` directory. Enter the directory and either:
 * Run 'git init; git git remote add origin https://github.com/MusicalCreeper01/Craft-Code-Snippets.git; git pull origin master'
 * Or download and copy all the files from this repository into it the folder

Next go to the plugins page in the admin control panel and enable the plugin.

## Enabling Rich Text code Snippets

To add the code snippets button in the Rich Text fields, edit `craft/configs/redactor/Standard.json` and add `codesnippets` to the `plugins` array. Done!

# Using the Code Snippet field type in templates

```HTML

<pre class="code">{{ entry.code }}</pre>

```

Replace `entry."code"` with the id for your code snippet field. The pre tag will automatically be detected and code formatting will be applied.

# Notes
Please report and bugs and suggestions in the issues section on Github :)


# TODO
 * Add Ace configuration for theme, font size, etc. 
