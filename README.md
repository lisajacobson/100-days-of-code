# 100 Days Of Code - Goals + Log
Tracking my 100 days of code journey.

## Goals

#### Frameworks to learn:
- React Native
- NodeJS

#### Applications:
- Build at least 5 new React Native applications
- Finish Podshelf React web app
- Master authentication in Node/React apps, e.g. Spotify and Twitter

#### CSS
- Master Flexbox in React web apps
- Learn and use JSS
- Learn and practice CSS animations

## Log

### Day 1: July 4, 2020

**Today's Progress**: Committed and  MyWeatherApp repo on GitHub; added API constants for local development; and fixed Alert response JSX and Forecast css.

**Thoughts:** I struggled with getting the right css for my Forecast tab page, but eventually through trial and error with Flexbox properties, I got it to look the way I wanted it.

**Link to work:** [MyWeatherApp](https://github.com/lisajacobson/MyWeatherApp)

![Current weather](https://user-images.githubusercontent.com/7946801/86827553-20ecba80-c060-11ea-9f63-a28389c76b6f.png)   ![5-day Forecast](https://user-images.githubusercontent.com/7946801/86827554-20ecba80-c060-11ea-8211-f1ee1a755351.png)   ![Alerts](https://user-images.githubusercontent.com/7946801/86827556-21855100-c060-11ea-973e-aa91bc590186.png)



### Day 2: July 5, 2020

**Today's Progress**: Did some crowdsourcing on Twitter to get more ideas of apps to build; learned some NodeJS on Udemy; and started a bookmarking app at my friend's suggestion.

**Thoughts:** Node seems really great and I'm excited to learn more and be able to start creating fullstack apps with JS.

### Day 3: July 6, 2020

**Today's Progress**: Working my way through a NodeJS course on Udemy; building a notes command line app with CRUD; have used yargs, process.argv, and file system modules; and learned how to export modules from one component to another and import modules into components.

**Thoughts:** Node is a lot of fun and the fact that it's written in JS makes it that much easier to learn. Also, I forgot how fun command line apps can be to build.

**Work:** ![app.js](https://user-images.githubusercontent.com/7946801/86828072-c30ca280-c060-11ea-9b3d-351496a19b43.png)   ![notes.js](https://user-images.githubusercontent.com/7946801/86828074-c30ca280-c060-11ea-9c75-204c070e2de0.png)

*due to work work, I wasn't able to make the time the past few days, so I am counting the days starting with when I was able to pick things back up*

### Day 4: July 11, 2020
**Today's Progress**: I wrapped up the notes command line app I was building using Node JS. It has 4 commands that allow you to add a note, read a single note, list all notes (titles and contents), and remove a particular note. I used the chalk module to play with colors and highlight the outputs, which made it more aesthetically pleasing to read what's logged to the console as a result of each command.

**Thoughts:** My first foray into Node was a simple command line app that was more for learning than for the resulting app itself. Through the exercise, I learned some more JS, as well. I got more practice using the filter and find methods on arrays, and learned that find is more efficient because it stops at every point where your function *finds* a match (or non-match, depending on how your code is written).

**Work:** screen cast coming soon but here's the repo: [NodeJS command line notes app](https://github.com/lisajacobson/notes-cmd-app)

### Day 5: July 12, 2020
**Today's Progress**: I went through a couple of NodeJS video courses and coded along in VS Code. I learned about OS, Path, and Events modules, as well as how to use EventEmitter and an event listener to listen for the event and do something after the event. Also learned about the HTTP method, as well as how to structure CRUD in an API built with the Express library.

**Thoughts:** I can see already how Express lets you write APIs on top of Node in a succinct way, much more than if you simply had if statements or a switch and cases for each call. Express lets you write your API routes very explicitly, and I can see how useful this will be when I start building my own APIs to connect with front ends.

**Work:** Some coding in my IDE but nothing too exciting for today.

### Day 6: July 14, 2020
**Today's Progress**: I walked through some written tutorials to learn how to set up a MERN app. That's MongoDB/Mongoose, Express, React, Node, and scoped out my app. I also creted an entity relational diagram for the app that I'm calling markit. I'll eventually post the ERD in the readme once I create it for the rep.

**Work**: [markit app](https://github.com/lisajacobson/markit)

### Day 7: July 15, 2020
**Today's Progress**: Due to an upcoming project at work for which I need to learn Angular, I started to learn the framework by walking through and coding along with the sample project on the [official Angular website](https://angular.io/start). I learned about template syntax: ngIf and ngFor, interpolation {{ }}, property binding [ ], and event binding ( ). I learned how to work with and set up new routes. I'm also getting used to working with the MVC structure, similar to how Ruby on Rails is set up, which was the first MVC framework I learned.

**Thoughts:** There's a lot of what I'd call overhead, many files that are required for a single component in Angular, including a typescript file for the actual component business logic, a css file for styles, and an html file for markup. It seems strange - after working with hooks and functional/pure components in React - to have class-based components everywhere, no matter what your component is in charge of doing. Looking forward to learning more about how to build apps using Angular including how to use and manipulate data in Angular. 

**Work:** Below is one component from my coding along, but note that I ran into what seems like, based on a cursory google search, a very common error: unless you import `core-js` into your `polyfills.js` file, there's an issue with the import statements of two components in your `app.module.ts` whose solution is not apparent. But after I added the package to the pollyfills file, the StackBlitz browser tab prompts you to install it, which fails repeatedly. I plan to continue the tutorial using my IDE and running it in the browser, which is what many have suggested online. 
![one component of my code](https://user-images.githubusercontent.com/7946801/87680452-748b9200-c74b-11ea-9074-1c7df07534b5.png)

### Days 8-18: July 15, 2020
**This week.5's Progress**: I have been getting acclimated to an Angular codebase with a Java backend that is also connected to a bunch of C# applications. In addition to learning Angular and working on my first feature for this new project I'm on, I've spent some time reviewing C# code, as well, which I am delighted that I can do with my programming knowledge even though I've never coded even a single line of C# in my life. Re: Angular, it's been an interesting and fun week. I've been working on code that takes in some statuses from the backend and displays an icon conditionally if specific statuses are coming in as true values. I had to parse it because it was in bitmap as JSON format, so that manipulation process was neat. `JSON.parse()` helped me get rid of the beginning and trailing special chars (`/`s) surrounding the keys and values in the incoming JSON object. There are many different parts of the front end that needed to be modified to accept this new data, so in addition to figuring out how to conditionally show the icon, I had to make sure I was processing the data correctly and in the right files. With Angular's MVC architecture, this meant working in the models, views, and controllers; or, models, templates (HTML files), and `component.ts` files. And I feel like I've gotten the hang of working in Angular. However, using `ngClass` to conditionally show the CSS classes - based on simple methods in the component itself - has proven to be tricky because it's finicky.

**Thoughts:** see above ^ because I combined progress and thoughts today. 

**Work:** Sadly I cannot show any visuals from my efforts because this is for work and is proprietary.
