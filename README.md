# project-ideas
Some project ideas I would like to do in my spare time

## Quizzer ([first approach here](https://question-master.herokuapp.com/)) ([current approach here](https://github.com/DanielMSchmidt/quizzer))
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

## WageChecker
A react-native app to monitor your monthly wage via tickspot. 

- Maybe add a goal and see how much you have won it
- Maybe (if possible) get the data from not submitted, but ticking timers
- Add a cool graph of this year, vs last year etc on the amount of hours worked

## Graphql Rails engine
Build a Rails engine which provides a graphql scheme

- Build scheme from models `(acts_as_qraphql_field(for=:default))`
- Mountable rails engine for routes
- make more than one scheme possible
- have a default scheme (for one scheme applications)
- Maybe even generate a sort of documentation or documentation helper
- Goal: easy to use!
