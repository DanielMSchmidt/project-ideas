# Ideas

This are all ideas of programming related stuff, that I might do in my free time. Just a reminder for me, but if you need a project you are free to implement something from his list. It currently includes

- Projects
- Blog Posts

## Projects
Some project ideas I would like to do in my spare time, not ranked anyhow. Please let me know if you are working on a similar problem and if you need help with it.

### Quizzer ([first approach here](https://question-master.herokuapp.com/)) ([current approach here](https://github.com/DanielMSchmidt/quizzer))
An application which quizzes you exam questions and shows the answers after a test. The optimal workflow would be

1. As you prepare your learning materials in Latex (a summarization would be optimal) annotate them with sections, subsections etc that would be answers to questions. Notate that questions with ```#Q: What does the fox say?``` in the corresponding block (highest gets choosen)
2. Copy & Paste (or pass via CLI, don't know, maybe both) the .tex to the application
3. See your questions in a list, possibly edit them
4. Click a test button, which takes a unasked (or worst rated) bulk of questions for you to answer
5. Click on a Question to see answer and rate how far you were away from this
6. Study faster and better
7. Win exam
8. ???
9. Profit

### WageChecker
A react-native app to monitor your monthly wage via tickspot. 

- Maybe add a goal and see how much you have won it
- Maybe (if possible) get the data from not submitted, but ticking timers
- Add a cool graph of this year, vs last year etc on the amount of hours worked

### [Rain & Water Effect](https://github.com/DanielMSchmidt/rn-rain-and-water-effect) 
~ WIP ~

Rebuild rain effects as easy to use react component

- Effect from [Rain & Water Effect Experiments](http://tympanus.net/codrops/2015/11/04/rain-water-effect-experiments/)
- WebGL bindings from [gl-react-native](https://github.com/ProjectSeptemberInc/gl-react-native)


### ServiceWorker Loader
A [webpack loader](https://webpack.github.io/docs/how-to-write-a-loader.html) which adds a section into a script (or generates a new one to include) with service worker functionality using the [sw-toolbox](https://github.com/GoogleChrome/sw-toolbox). E.g.:

- precache attribute, which adds item to toolbox.precache (for link and script elements)
- meta keyword for default request method?
- overwrites for request method in a tags (e.g. networkOnly for strictly uncachable pages)


### Breakpoint Tester Plugin

Opens the page in multiple iframes which have the same width as breakpoints in CSS

- optional: height breakpoint support
- optional: have the click & scroll events mirrored in all iframes so we have kinda browsersync behavior

### [Hub](https://github.com/github/hub) for Stash

Most important features: 

- `git pull-request`
- `git create`
- `git browse`
- `git checkout`


## Blog Posts

### I <3 ES6

Write about increased clarity of es6 due to deconstructing, easy moduling, etc.

### React-Native Module Generator

Present my react-native module generator and talk about the reason to write it and the roadmap.

### React-Native iOS View Lib

How to use a iOS lib with a view component as rn module

### Electron vs. RN Desktop 

Compare both in terms of usability, stability, speed of development, etc


