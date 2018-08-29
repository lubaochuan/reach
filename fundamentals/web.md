---
layout: default
title: Web Fundamentals
---

# Web Fundamentals

I'll put it bluntly: web development is hard. There are so many moving parts and the technology is constantly changing. I think it is important to establish a baseline of knowledge that I think you should pursue in order for web development concepts to make better sense. Once you are familiar with the fundamentals, it becomes easy to keep up with the changes. The Web may evolve rapidly, but this is a great thing. It becomes easier to do more with less and in less time. 

When I first learned, I had to drink from the firehose. I was given a project description from the client and a deadline. That's it. I had done programming before, but had never touched any Web technology. I was overwhelmed with the size of the learning curve. It eventually got easier, but it was much harder than it needed to be, starting out. I was given things to read and watch, but I would have liked to know exactly *what* I should be learning and *why*. That is the purpose of this page.

## A note about resources

Any link I provide to learning material, whether book or video, is just an example. I do not provide an exhaustive list. You will likely need to do some research on your own if the resources I provide do not fit your learning style or your specific project needs.

## Read the docs

Learning how to learn, I think, is the basis of successful software development. I spend more time reading documentation, watching videos, and practicing concepts than I do actually developing software. Once you get something down, it's typically easy to do. Laying the foundation is the hardest part. You will have to get used to looking up a problem online if you don't know the answer or ask a question if it hasn't been answered already. Unless there is a bug, you will find most of your answers within the documentation provided by the tool you're using. If the tool does not provide any docs, it is not worth using.

## CLI (Command Line Interface)

You need to become comfortable with the command line. Most web technologies you will face do not have a GUI, because it is much easier to type commands into a terminal, for certain things. If you had to install a GUI program for the amount of different things you will be using, you would be overwhelmed with the amount of windows you would have to have open. With a CLI, you can keep fewer windows open and get certain things done much faster. 

You should know how to manage and navigate your OS's file system via the built-in terminal. You have to be comfortable running different commands and reading the documentation on how to use them.

Otherwise, you may find yourself just copying and pasting commands you find on the Web, without knowing what exactly it does. This is unhelpful for when something goes wrong, and something always does.

Not all tasks are suited for command line either. Once you have mastered CLI, it becomes easier to see when using a GUI is appropriate and when a CLI can be the better option.

## Open source (Don't reinvent the wheel)

One thing you need to understand and appreciate about web development and software development in general is the beauty and superiority of open source software. You've heard the saying "Don't reinvent the wheel." That is one of the underlying principles of open source, which coincides with the popular DRY (Don't Repeat Yourself) software development mindset.

So, in the effort to keep things DRY and not reinvent the wheel, open source software is produced. This means for you as a developer that if there is a problem you need solved for your specific language or platform, it may have already been solved and provided as a library for you to use in your code. Often, this means that there are multiple libraries that perform the same basic functionality, with some differences in the details. It is up to you to explore different ones that have become popular, are easy for you to use, and/or better fit your project needs. There are always blog posts that recommend different libraries. I tend to go along with what the majority of the web development community is using or recommending.

See the section on [Package Management](#package-management) where I explain how open source works for web applications.

Of course, this is a give and take effort. If you use open source software, it would be great if you contribute back to the open source community (Hint: employers like to see you contribute to open source!).

There are tons of resources on why open source is superior, even for a business (Microsoft is one of the largest contributers to GitHub and which is what helped motivate them to purchase GitHub).

[10 Reasons Open Source Is Good for Business](https://www.pcworld.com/article/209891/10_reasons_open_source_is_good_for_business.html)

[opensource.com](https://opensource.com/open-source-way)

## HTML

Hypertext Markup Language (HTML) is the structure of web page content. If you have yet to be exposed to HTML (preferably HTML5), you can find a great tutorial on [W3Schools](https://www.w3schools.com/html/). Creating any web-based application requires some knowledge of HTML. You should also take some time to learn the differences of HTML5 over previous versions. If you are creating a new application, you will be using HTML5.

Other resources:
- [html.com](https://html.com/#beginners)
- [codecademy](https://www.codecademy.com/learn/learn-html)

## CSS

Cascading Style Sheets (CSS) is the the styling language of the Web. It defines how web pages look. [W3Schools](https://www.w3schools.com/Css/) also has great CSS tutorials. Once you are familiar with CSS, it's time to learn how to use it in a full web application.

CSS can become clunky, tedious, and repetitive. Several languages and libraries are being actively developed to make styling web pages easier.

Libraries provide CSS classes with pre-defined styles so that all you need to do is add classes to HTML elements. They make it very easy to get a great looking site with much less effort. Here is a list of some of the most popular ones. All of them contain a grid system, which is very important for creating [responsive web pages](https://www.w3schools.com/html/html_responsive.asp).

- [Bootstrap](https://getbootstrap.com/)
- [Materialize](https://materializecss.com/)
- [Semantic UI](https://semantic-ui.com/)

Libraries are great. However, that passes the burden of writing CSS to someone else. How do the creators of CSS libraries like Bootstrap address the tediousness of plain CSS? The answer is CSS preprocessors.
CSS preprocessors are languages that add new features and simplicity to CSS and, in the end, compile down into plain CSS. How do they apply to you then? Often, CSS libraries can be very opinionated. If you want to make a change to something, you will need to use whichever CSS preprocessor they use so you can properly overwrite their styles. CSS library docs should explain how to do this.

Three of the most popular CSS preprocessors are [Sass](https://sass-lang.com/), [Less](http://lesscss.org/), and [Stylus](http://stylus-lang.com/).

## JavaScript

JavaScript is the language behind the functionality of web pages. When you click a button on a modern website, or do almost any action (even just loading the page), JavaScript was likely involved. This is why according to the [Stack Overflow Developer Survey 2018](https://insights.stackoverflow.com/survey/2018/#most-popular-technologies), JavaScript is the most popular language in the world. In the effort to simplify application development, JavaScript is finding its way into other parts of computing, not just web pages. (See [Node.js](#node-js)).

When you write code in Java or Python or any other language, the code gets compiled (or interpreted) before it can be run. JavaScript is the same way. One of the greatest features of modern browsers is the ability to read and run JavaScript. See the section on [Single Page Applications (SPA)](#single-page-applications) for more information on why this is.

Okay, you get it. JavaScript must be amazing. The user and developer experience is much better with the power of JavaScript. However, just like anything else in existence, it is not without flaws.

### EMCAScript

EMCAScript is the standard upon JavaScript (and other languages) are built. It is not a programming language. JavaScript is just one (albeit, the most popular) implementation of the EMCAScript standard. Because JavaScript has flaws like everything else, it often gets improved. When a new EMCAScript standard is released, JavaScript gets an update, and browsers get an update supporting new JavaScript features.

However, these changes are not immediate. It takes time for JavaScript to adopt a new language feature, time for browsers to support that feature, and even more time for websites to use that new feature (if it becomes necessary or useful). This creates a problem for developers. That means they need adjust their programming based on which browsers (and the version of those browsers) the users use. For example, a developer can use [Can I Use?](https://caniuse.com/usage-table) to get an idea of what versions of browsers users are using, though this creates a lot of extra work. What if a developer could always use the latest features of JavaScript without having to worry about browser compatibility?

### Babel

Babel is the solution to the problem described in the previous paragraph. It allows developers to use the latest JavaScript features, then translates it into JavaScript that browsers support. Rather than waiting around for updates to Google Chrome, Firefox, etc., a developer can always use the latest and greatest features, which often speeds up development time and makes the code easier to read and understand.

You can read more about Babel [here](https://babeljs.io/).

## Browser Developer Tools

Every modern browser has built-in tools for developers. You may have right-clicked on a web page and clicked "Inspect Element". This is one of the ways to open developer tools for your browser.

What can you do with developer tools? Some of the details are different between browsers, but here is a general overview. With these tools, you can see the HTML, CSS and JavaScript for a page. You can view console output, all of the assets loaded by the page (images, etc.), and network requests (which are very useful when communicating with an API in the cloud). You can see statistics on the performance of your application (how much memory it uses, how long things take to load, etc.). Best of all, you can debug applications. You are able to set breakpoints and step through your code line by line so that you can see what values are changing and when.

If you have never debugged an application on any IDE with any language, you may want to read about debugging for [Chrome](https://developers.google.com/web/tools/chrome-devtools/) or [Firefox](https://developer.mozilla.org/en-US/docs/Tools). Debugging in one language is pretty much the same concept for all. If you have debugged before, you may still want to view that article to know exactly how it works for web apps.

Both Chrome and Firefox have great developer tools. I recommend using either one, as they are pretty much the same.

## Node.js

Originally, JavaScript was a client-side language only understood by browsers. [Node.js](https://nodejs.org/en/about/) is an engine that expands the usage of JavaScript outside of performing actions on web pages. With Node, devs can use JavaScript to access lower-level functionality of a machine, such as networking. This makes Node very popular for creating servers and building APIs. It is now possible to create a full stack web application (server-side and client-side) with a single language, JavaScript. Node.js has been rapidly overtaking other things used for server-side applications such as [PHP](https://secure.php.net/), because of its speed and ease of use.

## Package Management

Remember the section on the benefits of open source software? A topic that is closely tied to open source is package management. If developers create software for free, where is it all going to go? You may end up using tens or hundreds of different open source packages in a single project. Can you imagine going to a website for each one, clicking the download link, and adding it to an appropriate place in your project? Not only would that take a large amount of time, there would be inconsistency of how these packages are added to different projects. What if the package got an update? Does it make sense to go back to the website and download the latest version? Probably not. All of this could benefit from automation, and that is exactly the purpose of package management. A package manager is a tool with some interface that allows for the downloading, updating, and installation of packages. All of the packages are stored in some uniform place (called a repository) where every developer can go to find them, or, even better, every developer can use the same tool that gets packages from the same place. Because Unix-like OS's are built on open source software, they come with package managers for this purpose. On Debian-based Linux distributions, the popular package manager is [apt](https://wiki.debian.org/Apt). Arch Linux comes with [pacman](https://wiki.archlinux.org/index.php/Pacman). Java developers may use [Apache Maven](https://maven.apache.org/) or [Gradle](https://gradle.org/). Python devs use [pip](https://pypi.org/project/pip/)...

You get the idea. How about JavaScript? Node.js ships with a package manager called [npm](https://www.npmjs.com/), or Node Package Manager. To create web applications, you need to know how to use this tool, as this is how you will manage dependencies for your project. Any JavaScript library you may need can be found on npm's website. You can even do a manual search to find packages that fit your project needs.

There is a project similar to npm called [Yarn](https://yarnpkg.com/en/). Yarn is a package manager for JavaScript, just like npm. However, many developers prefer Yarn, because it often performs much faster than npm.

Use whichever one you prefer. Try both and figure out which one you prefer. It may be beneficial to start with using npm, for it is still the most widely used.

## Testing

Testing is an integral part of any software application. When you write tests, you are creating a foundation for your application's expected functionality.

Further explanation of testing:

- [JavaScript Testing: Unit vs Functional vs Integration Tests](https://www.sitepoint.com/javascript-testing-unit-functional-integration/)
- [JavaScript Unit Testing for Beginners](https://designmodo.com/test-javascript-unit/)

There are several different testing frameworks. Experiment with them and find the one you like best, or you can find comparisons [here](https://raygun.com/blog/javascript-unit-testing-frameworks/) and [here](https://medium.com/welldone-software/an-overview-of-javascript-testing-in-2018-f68950900bc3).

## Git

[Git](https://git-scm.com/) is the current standard source control program because it is far superior than previous ones, both in speed and ease of use. You probably have already been introduced to Git. I encourage you to become more comfortable with branching/merging and using the CLI. Explore different git workflows that developer communities are using and find one that works best with your team and your project.

## Text Editors

A developer is much more productive with the right tools. This includes what you use to write your code. The two most popular text editors for web developers are [Visual Studio Code](https://code.visualstudio.com/) (often called VSCode) and [Atom](https://atom.io/). Though, at the core, they are just text editors, they become the most useful with the help of extensions. With extensions, both can reach or even surpass the functionality of standard IDEs like Visual Studio or Eclipse. Because their UIs are cleaner and simpler than an IDE like Visual Studio, they encourage more use of the command line, which provides a great opportunity to better your CLI skills. You may be surprised with how many programming languages they support, and, as a result, I use them for all of my programming, not just web development.

## Markdown

Markdown is a language to create great-looking content quickly. README files on GitHub and this page you are currently reading are all written in Markdown. It has a simple syntax and is great for writing documentation. It is a good skill to have. You can read more about it [here](https://daringfireball.net/projects/markdown/).

## Front End Frameworks

### React

### Angular

### Vue


## Networking

## Protocols

### HTTP

### HTTPS

### SSH

### FTP

### SFTP

## Domains

## URLs/URIs

## SPA

## Routing

## Component Libraries
