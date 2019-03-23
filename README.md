Included screenshots of finished site but was unable to properly implant them in the README. They are included in the img folder.

![Screenshot]("https://github.com/JacobWellner83/Sprint-Challenge--Advanced-CSS/blob/jacob-wellner/img/Screenshot1.png")
![Screenshot]("https://github.com/JacobWellner83/Sprint-Challenge--Advanced-CSS/blob/jacob-wellner/img/Screenshot2.png")
![Screenshot]("https://github.com/JacobWellner83/Sprint-Challenge--Advanced-CSS/blob/jacob-wellner/img/Screenshot3.png")
![Screenshot]("https://github.com/JacobWellner83/Sprint-Challenge--Advanced-CSS/blob/jacob-wellner/img/Screenshot4.png.png")

# Sprint Challenge: Advanced CSS - Space Walkers Web Page


This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored advanced CSS techniques using Responsive Design and Preprocessing. During this Sprint, you studied how to use the viewport meta tag, media queries, setting up a preprocessor, and advanced use of preprocessing techniques. In your challenge this week, you will demonstrate proficiency by updating a website that is missing content as well as adding mobile styling.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in advanced css and your command of the concepts and techniques in responsive web design and preprocessing.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your project manager.

## Description

The client for this challenge is _Spacewalkers Magazine_. Spacewalkers needs your help to build a small proof of concept website for their marketing team. They have provided designs for both desktop and phone views. In addition to designs and content they have most of the home page coded for you. You just need to finish the navigation and header as well as the mobile styles.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution design files of the desktop and mobile views:

[Click here to review the home design](design-files/home-desktop.png)

[Click here to review the mobile design](design-files/home-mobile.png)

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

1. What is the difference between an adaptive website and a fully responsive website?

Adaptive websites set a different layout at each breakpoint set by a devices size. They do not alter after that. A fully responsive website responds to the resizing of a window to alter the layout using CSS media queries.

2. Describe what it means to be mobile first vs desktop first.

Mobile first design focuses on being fully adaptive to the given screen size and resolution over the mass of content. In mobile first design some elements may be hidden or arranged with a smaller resolution and different flow in mind. Desktop first design involves planning for large displays that can solidly incorporate a wealth of information at a high resolution. Each design is a viable option for a given majority of web traffic.

3. What does `font-size: 62.5%` in the `html` tag do for us when using `rem` units?

When using rem units you are referencing a base root font-size/measurement setting for the entire page. When you set a font-size as a percentage of rem you are setting it at a particular percentage of the given rem for that page. Setting the html font-size to 62.5% is a specific technique to change font-sizing from the default of 16px to 10px (10 is 62.5% of 16) so that rem sizing is done in a base10 system. Thusly, if a font size is set in a given element, p { font-size: 1.8em; } the font in the p element will be 18px or 18pt.

4. How would you describe preprocessing to someone new to CSS?

Preprocessing is using a preprocessor (a kind of program) that understands a styling language and also understands a short-hand version of that styling language to produce easy to use styling changes and code rapidly. By learning the preprocessors shorthand we can input a smaller amount of code into a preprocessor and it will produce a large amount of fluid styling code. This makes styling more efficient and versatile as we can make quick changes to specific sections of the code, spread throughout, on the fly.

5. What is your favorite concept in preprocessing? What is the concept that gives you the most trouble?

The most interesting concept for me is the organization that can be achieved in our styling structure. It becomes far more easy to read and understand.
The concept that gives me the most trouble is parametric mixins as they are essentially similar to mathematical functions which set variables as words instead of representational symbols and are capable of taking other functions as arguments. This makes gaining a solid understanding of the correct syntax required to make them work a challenge.


You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section *will* prevent you from passing this challenge.

## Project Set Up

Because you are using a preprocessor, there are two parts to setting up your project.  Be sure to run through the git set up first and then set up the preprocessor.

### Git Set up

Follow these steps to set up your project:

- [ ] Create a forked copy of this project.
- [ ] Add your project manager as collaborator on Github.
- [ ] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [ ] Create a new branch: git checkout -b `<firstName-lastName>`.
- [ ] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [ ] Push commits: git push origin `<firstName-lastName>`.
 
Follow these steps for completing your project.

- [ ] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [ ] Add your project manager as a reviewer on the pull-request
- [ ] Your project manager will count the project as complete by merging the branch back into master.
 

### Preprocessor Set up

* [ ] Verify that you have LESS installed correctly by running `lessc -v` in your terminal, if you don't get a version message back, reach out to your project manager for help.
* [ ] Open your terminal and navigate to your preprocessing project by using the `cd` command
* [ ] Once in your project's root folder, run the following command `less-watch-compiler less css index.less`
* [ ] Verify your compiler is working correctly by changing the `background-color` on the `html` selector to `red` in your `index.less` file.
* [ ] Once you see the red screen, you can delete that style and you're ready to start on the next task

## Minimum Viable Product

Your finished project must include all of the following requirements:

### Import LESS Files

* [ ] Navigate to your `index.less` file. Notice the file is blank. You have been asked to use a certain import order. That order is as follows:

```markdown
1.variables.less
2.mixins.less
3.reset.less
4.global.less
5.navigation.less
6.footer.less
7.home-page.less
```

_You will know everything is working properly when you see the styles enabled for the provided content._  

### Home Page - Desktop HTML & LESS

* [ ] Take 10 minutes to review the code that has already been provided for you. Take time to see how the home page was built.

* [ ] Add a viewport meta tag to the head of your index.html page

* [ ] [Review the provided home desktop design file](design-files/home-desktop.png). You are to build the missing navigation system and header image. You have been provided all content necessary in the [index.html file](index.html)

* [ ] Navigation Styles: Use the `navigation.less` file for styling.

* [ ] Main Content Styles: Use the `home-page.less` file for styling

* [ ] LESS Mixins: Create and use 2 different mixins to aid your styling. Use the `mixins.less` file for your mixins

* [ ] LESS Parametric Mixin: create a parametric mixin that is used to create the `sign up` button styles.

* [ ]  Use at least 2 parameters to create your button

* [ ] Create a hover state that swaps the background color and font color of the base button styles.

### Mobile Design

* [ ] Create a `@phone` variable that contains a `max-width: 500px` media query string. Use the `@phone` variable for all your nested mobile styling.

* [ ] [Review the provided home mobile design file](design-files/home-mobile.png). Match your mobile styling the best you can using the design file.

* [ ] Push your changes and create a pull request if you haven't already.

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] Build a page of your choosing from the navigation items. Come up with content and images that fit the theme.

* [ ] Introduce CSS animations to your site.

* [ ] Create a fixed navigation and add some opacity to the background

* [ ] Create a form that would allow someone to sign up for a Spacewalkers Magazine subscription