food-truck
==========

Food-Truck finder for UBER

![alt text](https://raw.github.com/rajeshsegu/food-truck/master/public/img/Uber%20FoodTruck.png "Uber Food Truck Screenshot")

User Experience:
====

### Highlights:

1. Google Based UX gives flexibility and completness to the location aware services
2. Geo Locate HTML5 API ( but restricted it to Powel Station as the results are based in SF )
2. Simple List View approach that is straigh forward
3. Search and Sort by Distance to filter
4. Scrolling the List View has a Page flip effect ( CSS3 transitions / anitmations )

TECHNOLGIES
======

This is the first Backbone based application that I have built end to end. Backbone in my opinion is bare bones and can be augmented to any custom framework but as a complete application framework it feels short compared to Ember and AngularJS. Anyway, I really enjoyed learning something new and delivering my best. 

In addition, added Jasmine unit test cases to make sure the sanity is maintained even after aggresive code changes. Used Grunt as the build script ( good learning experience )

Backend  - NodeJS, Express Framework, REST interfaces

Frontend - Bootstrap, Backbone, jQuery, Underscore, Google Maps & Stroll framework

Dev      - Jasmine Unit Tests, Grunt, PhantomJS


### Needed Improvements:

1. Better Performance, we plot 700 different points on Google Maps. We could definitely lazy create them in batches or render only things for a 3mile radius. I had problems with Google Maps performance when I was turning off and on points as per the reuslts. Google Maps does not like such heavy operations with basic Markers. It recommends we use Overlays.
2. I keep resetting Collection View from AppView and ListView. We could definitely reduce the cycles of filtering and resetting the collections on different triggers.
3. A definite improvement on frameworks side is use of highlevel frameworks like Mariotte to handle collection views implicitly and delegate events naturally. 
4. More Jasmine unit test cases
5. LESS based CSS istead of static as included.

PRODUCTION
======

Hosted the NodeJS based application on Heroku platform. ( Wow, Damn easy! )

Access hosted application @ http://evening-sands-7465.herokuapp.com/

DEVELOPMENT 
======

#### Code

###### Front-End: 

Frameworks: food-truck/public/lib

BootStrap: food-truck/public/css/

App Code:  food-truck/public/

###### Back-End:  

NodeJS

Routes:    food-truck/app/routes
( Rest End-point GET /foodtruck is at foodtruck.js )

WebServer: food-truck/webserver.js

#### Local Setup 

In case if you are interesting in running this locally, please 

> git clone https://github.com/rajeshsegu/food-truck.git

> npm install

> node webserver.js 

> Access http://localhost:5000/

#### Unit Tests 

![alt text](https://raw2.github.com/rajeshsegu/food-truck/master/public/img/unittests.png "Jasmine Unit Tests")

> ( install compatible PhantomJS for your OS vairant )

> npm install -g grunt

> grunt (or) npm test

GitHub
======

Proud of my recent open-source projects

### AngularJS Template i18n Validator

https://github.com/rajeshsegu/angular-i18n-template

This NodeJS solution makes sure every possible text is i18n-ized in every template so that translations are not missed. This is mission critical for SAAS application that caters to various regions of the world. Meanwhile, it can be easily be integrated into the CI setup.

