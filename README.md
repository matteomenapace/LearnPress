# LearnPress

The most minimal WordPress theme starter ever :)

Designed for learning.




# Getting started

Download and extract the *zip* for this repository (or `git clone` it) into your `wp-content/themes` folder.

You want to end up with a `LearnPress` folder inside `wp-content/themes`

```
YOUR_WORDPRESS_FOLDER
├── wp-content
│   ├── themes
│   │   ├── LearnPress
│   │   ├ ...other themes that come pre-installed

YOUR_WORDPRESS_FOLDER
|-wp-content
  |-themes  
    |-LearnPress
    |- ...other themes that come pre-installed
```

### Adding libraries

Such as HTML5 Boilerplate, Skeleton, Bootstrap etc.

Instead of manually finding libraries, downloading them, extracting them into the right folder.. we can use a tool called [bower](http://bower.io/) which will do *that* (managing *packages*) for us. 

![](http://bower.io/img/bower-logo.png)

<!--It'll take a little set up, but once you're up and running everything will be smooth-->

![](img/terminal.png) ![](img/command-prompt.jpg)

1. Open Terminal (Mac) or a [Command Prompt](http://windows.microsoft.com/en-gb/windows-vista/open-a-command-prompt-window) (Windows).  
* Install [Node.JS](https://nodejs.org/)   
	
	To check if you have Node.JS installed..   
	In Terminal / CP, type `npm` and press the `↲` (Enter) key
* Install [bower](http://bower.io/)  

	To check if you have bower installed..   
	Type `bower` and press the `↲` (Enter) key
* If you're on Windows, install [msysgit](https://msysgit.github.io/)
* *Navigate* to the `LearnPress` folder  

	On Mac, drag the LearnPress folder onto the Terminal app icon  

	On Windows, drag the LearnPress folder inside CP, then change `C:` to `cd`, so that you'll end up with something like `cd  \wamp\www\YOUR_SITE_NAME\wp-content\themes\LearnPress`
* Type in `bower install` and press the `↲` (Enter) key

	Bower will install the **components** listed in `bower.json`.
	
	LearnPress comes with HTML5Boilerplate and Skeleton.
	
	If all goes well, you should end up with a new `bower_components` containing `html5-boilerplate` and `skeleton-css`
	
	```
	LearnPress
	|- bower_components
		|- html5-boilerplate
		|- skeleton-css
	```

<!--- [ ] Image of bower_components folder-->

### Want more libraries? 

Let's say you want to add [Bootstrap](http://getbootstrap.com/getting-started/#download-bower).

`bower install bootstrap --save`

The `--save` bit will add the Bootstrap dependency to your `bower.json`

Check [libraries.io](https://libraries.io/bower/) for even more libraries.

### Troubleshooting

* If you're getting a `ECMDERR Failed to execute ...` error:

	`git config --global url."https://".insteadOf git://`
	
* If you're getting a `git is not installed or not in the PATH` error in Windows, follow [these steps](http://stackoverflow.com/questions/20666989/bower-enogit-git-is-not-installed-or-not-in-the-path)
