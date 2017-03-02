# jQuery Quiz using JSON

[![Code Climate](https://codeclimate.com/github/Matt-Webb/jquery-quiz-using-json/badges/gpa.svg)](https://codeclimate.com/github/Matt-Webb/jquery-quiz-using-json)

This code enables you to render questions with optional answers using radio buttons. Using [valid JSON](http://jsonlint.com/)
you can provide a list of questions and answers which will render to the user in sequence.

Each question can be assign a score against each option, this allows for a range of score for each question.

### Bower
Install with [Bower][bower]
`bower install jquery-quiz-using-json`

[bower]: http://bower.io/

### DEMO

A basic js fiddle [demo](https://jsfiddle.net/Webby2014/t4p8x02b/)

### EXAMPLE USE:

__JSON__

    {
       "question": "What year was the film The Shawshank Redemption released?",
                "includeInfo": true,
                "info": "Two imprisoned men bond over a number of years, finding solace and eventual redemption through acts of common decency.",
                "answers": [
                    {
                        "answer": "1995",
                        "score": 0
                    },
                    {
                        "answer": "1994",
                        "score": 0
                    },
                    {
                        "answer": "1993",
                        "score": 5
                    }
                ]
    }

__HTML__

    <div id="quiz"></div>

__JQUERY__

*Note:* this is not currently implimented as a plugin and therefore no initialisation is required just a reference to the `jsonQuiz.js` file.

### TO DO

*   Convert jquery code into plugin and include settings on initialise
*   Abstract the rendered html question into templates for better customation
*   Refactor json data for better clarity e.g "answers" should be "options" etc.
*   ~~Add optional style sheets~~
*   ~~Configurate as bower package~~
