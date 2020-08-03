# html-g20
HTML CSS Fundamental

An extension to preview HTML files while editing them in VSCode

The extension can be activated in two ways

Toggle Preview - ctrl+shift+v or cmd+shift+v
Open Preview to the Side - ctrl+k v or cmd+k v

lint
vscode-linthtml
Build Status

A Visual Studio Code extension to lint HTML with linthtml.

screenshot If you find some error message not explicit enough, please create an issue here

Installation
Execute Extensions: Install Extensions command from Command Palette.
Type @sort:installs linthtml into the search form and install the topmost one.
Read the extension installation guide for more details.

Usage
This extension automatically validates documents with these language identifiers:

HTML (html)
If you have a valid hmllint configuration file .linthtmlrc (all options available here) in the current workspace folder the extension will use it. Otherwise, the default configuration of linthtml will be used.

Extension settings
linthtml.enable
Type: boolean
Default: true

Control whether this extension is enabled or not.

linthtml.configFile
Type: string Default: null

Specified the path to a config file for LintHTML that will be used to lint all HTML files in the current workspace.


IntelliSense for CSS class names in HTML
A Visual Studio Code extension that provides CSS class name completion for the HTML class attribute based on the definitions found in your workspace or external files referenced through the link element.



Features
Gives you autocompletion for CSS class definitions that can be found in your workspace (defined in CSS files or the in the file types listed in the Supported Language Modes section)
Supports external stylesheets referenced through link elements in HTML files
Command to manually re-cache the class definitions used in the autocompletion
User Settings to override which folders and files should be considered or excluded from the caching process
Supported Language Modes
HTML
Razor
PHP
Laravel (Blade)
JavaScript
JavaScript React (.jsx)
TypeScript React (.tsx)
Vue (.vue) [requires octref.vetur]
Twig
Markdown (.md)
Embedded Ruby (.html.erb) [requires rebornix.Ruby]
Handlebars
EJS (.ejs)
Django template (django-html)
Specific Support
"@apply" directive in CSS, SASS and SCSS Files for Tailwind CSS
"className" and "class" in TypeScript React, JavaScript and JavaScript React language modes
Emmet abbreviations support triggered by typing a "." (comes disabled by default, check the User Settings topic for more information)
Contributions
You can request new features and contribute to the extension development on its repository on GitHub. Look for an issue you're interested in working on, comment on it to let me know you're working on it and submit your pull request! :D

What's new in version 1.18 (Jan 25, 2019)
Added support for Django template (django-html).
Check out the changelog for the current and previous updates.

Usage
If there are HTML or JS files on your workspace, the extension automatically starts and looks for CSS class definitions. In case new CSS classes are defined, or new CSS files are added to the workspace, and you also want auto-completion for them, just hit the lightning icon on the status bar. Also, you can execute the command by pressing Ctrl+Shift+P(Cmd+Shift+P for Mac) and then typing "Cache CSS class definitions."

User Settings
The extension supports a few user settings, changes to these settings will be automatically recognized and the caching process will be re-executed.

Folders and Files
You can change the folders and files the extension will consider or exclude during the caching process by setting the following user settings:

"html-css-class-completion.includeGlobPattern" (default: "**/*.{css,html}")
"html-css-class-completion.excludeGlobPattern" (default: "")
Emmet
Emmet support comes disabled by default, the reason behind this choice is because it the current implementation simply triggers completion when you type a "." (period) and this behavior might be considered a little annoying, but it might change in the future.

Currently it supports the following languages (those are language identifier): "html", "razor", "php", "blade", "vue", "twig", "markdown", "erb", "handlebars", "ejs", "typescriptreact", "javascript", "javascriptreact".

"html-css-class-completion.enableEmmetSupport" (default: false)


VSCode doesn't have HTML validation by default. But it allows you to add extensions and enable these features.

To add HTML validation (linting), Open VSCode, then press Ctrl + P and then paste ext install HTMLHint in it, and press enter. It will install a HTML validator. You may need to reload VSCode to load the extension.

Now if you open the same html document you had the syntax error, you should see there's an issue shown at the status bar at the bottom :) and it will also show you the errors in those lines.

VS Code default support code formatting and it track the syntactical error. If you create a new file and directly try to write the code than VS Code could not able to understand which language or type of syntax user want to format/correcting. So, first need to save the new file with the proper extension than visual studio properly identify the syntax.

The code formatting is available in VS Code through the following shortcuts:

On Windows Shift + Alt + F
On Mac Shift + Option + F
On Ubuntu Ctrl + Shift + I
You can add Auto Close Tag from VS Code marketplace.

Launch VS Code Quick Open (Ctrl+P), paste the following command, and press enter.

Automatically add HTML/XML close tag, same as Visual Studio IDE or Sublime Text

ext install auto-close-tag
VS Code integration for HTMLHint - A Static Code Analysis Tool for HTML

ext install HTMLHint
Provides CSS class name completion for the HTML class attribute based on the CSS files in your workspace. Also supports React's className attribute.

ext install html-css-class-completion

