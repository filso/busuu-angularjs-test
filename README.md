# Busuu front end test

PLEASE DO NOT FORK THIS REPOSITORY. git clone, and send us completed test

In Busuu we use grunt for automating all front end build tasks, Sass with Compass for generating CSS.
In this simplified test we use LessCSS to help generate CSS quickly.  

We would like you to implement a very simple vocabulary game.  
The technology is AngularJS, Bootstrap and LessCSS on front end, with NodeJS communication endpoint on backend.

### App

You will find 11 words with keyphrases and spanish translation hardcoded in words AngularJS value in *public/js/services.js*.  

1. On every round one random word is chosen - question asked to the player. We show player english word with english keyphrase.  
2. We also provide 3 answers - shown to user in  Spanish - chosen randomly from 11 words provided (one of them is translation of previously randomly chosen word).   
3. The game consists of 3 rounds. If
the user chooses the wrong answer the game is finished.
4. When the game is finished the
 user can enter his name. If he does, the score is sent to the server, and will appear on "High score" subpage of the app. This subpage will download highscore list, using $http AngularJS service.

_Tip:
No need to use 
any database persistence on server-side - keeping data in NodeJS memory is sufficient for this test._

### Running the app

    npm install
    bower install
    nodemon app.js

then go to [http://localhost:3000](http://localhost:3000) 


### Test

To begin the test, please clone this github repository, and start coding. Use your local git repository, and commit any changes you make. After you finish your test, please send it to [filip@busuu.com](filip@busuu.com). PLEASE DO NOT FORK THIS REPOSITORY.  
The suggested time for this test is 90 minuteshour, but you are welcome to do it longer.

In Busuu we value productivity and code quality. Your code will be assessed on:   
- clean app structure (you are welcome to change files organisation)  
- code formatting and naming  
- object-oriented design and implementation
- proper use of components (controllers, directives)

In particular for this test you can ignore:  
- How the app looks. We included Bootstrap to make development process faster  

##### Senior position tasks
If you apply to senior position, we'd like to see also:
- Unit tests (we suggest Karma)  
- Add timing to game
- Correct OO architecture (directives, controllers, services)
- Performance
- Comments on performance and architecture decisions


## Directory Layout
    
    app.js              --> app config
    package.json        --> for npm
    public/             --> all of the files to be used in on the client side
      css/              --> css files
        app.less        --> less stylesheet
      img/              --> image files
      js/               --> javascript files
        app.js          --> declare top-level app module
        controllers.js  --> application controllers
        directives.js   --> custom angular directives
        filters.js      --> custom angular filters
        services.js     --> custom angular services
    routes/
      api.js            --> route for serving JSON
      index.js          --> route for serving HTML pages and partials
    views/
      index.html        --> main page for app
      partials/         --> angular view partials (pure HTML, you can use Jade as well)


##Useful links
#### [AngularJS](http://angularjs.org/), [LessCSS](http://lesscss.org/)

## Contact

This test code is based on Angular seed. If you have questions, don't hesitate to ask: [filip@busuu.com](mailto:filip@busuu.com), skype: fsobczak
