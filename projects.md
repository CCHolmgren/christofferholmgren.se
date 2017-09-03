---
layout: page
title: Projects
sidebar_link: true
---
### Millibar
![](/assets/img/ss+2017-09-03+at+09.59.49.png)
[Millibar](https://millibar.co/) is a Basecamp clone. Organizing projects with schedules, tasks and more. 

Languages: **PHP**, **JavaScript**, other techniques: **Laravel**, **Vue.js**, **Foundation 6**.

### theiterativeblog

### Reexguide (was Restaurant List)
![](/assets/img/ss+2015-10-25+at+02.07.36.jpg)
[Reexguide](https://www.reexguide.com/) is a page to find and explore restaurants. It's difficult to find new ones, tiresome to search for them, and which ones have you visited? Those are the problems that Reexguide tries to alleviate.

Languages: **Python**, **JavaScript**, other techniques: **Django**, **jQuery**, **Foundation 6**.

### PHPForms
![](/assets/img/ss+2015-04-30+at+03.41.48.png)
[PHPForms](https://github.com/CCHolmgren/PHPForms) is a library for creating and handling forms using nothing but PHP 5.4+.
The library tries to be feature complete with Laravel-form-builder, a library for PHP forms that has a dependency to Laravel, while at the same time not depend on it itself.  
I also wanted some features that are inspired from Django, such as the formatting of forms using ```to_p```, ```to_ul```, ```to_table``` functions. It has a ```asDivs``` method that allows you to format your form as divs, but you may also format it any way you please with a little less terse API.  
It also provides validators and allows you to easily create new ones, or use some built in ones if you please.  
The main goal was the compatibility with Laravel-form-builder, but also to have a modular system, so that as many parts as possible are extendable if you want some feature that is missing.  

Languages: **PHP**, other techniques: **composer**

* * *

## Projects done while studying at Linneaus University

# Projects TOC
* [Music Comparer](#music-comparer)
* [Kubus](#kubus)
* [Quiz-a-tron](#quiz-a-tron) 
* [Ruby on Rails and AngularJS project](#ruby-on-rails-and-angularjs-project)
* [Forum/bookmark site](#forumbookmark-site)
* [1DV449](#dv449)  
    1. [Laboration 1 and 2](#laboration-1-and-laboration-2-in-1dv449)

* * *

### Music Comparer
![](/assets/img/ss+2015-04-30+at+12.32.27.png)
Music Comparer is a page that gathers information from Last.FM and Spotify and compares artists with eachother. There was also an added requirement of it being offline-first, so Music Comparer caches searches to enable comparisons whilst offline.   
The task that we were given was to develop an application that uses at least two different API's, and also uses OAuth in some part of the application.  
Because my application doesn't rely on the OAuth part at all I used the Last.FM login API to prevent using the application without signing in.  
The backend runs Node.js and uses Redis with RDB enabled as a sort of  persistent in-memory database. 
Due to the lacking LocalStorage API that browsers provide there is no way to TTL mark the caching without using some library to provide this functionality, and as such the searches will not be updated. This shouldn't affect things, but it might hinder some things if more development is done.

Code can be found [here](https://github.com/CCHolmgren/Music-comparer).

Languages: **Javascript**, other techniques: **NodeJS**, **express**, **redis**  

### Kubus
![](/assets/img/ss+2015-05-04+at+02.29.46.jpg)
[Kubus](http://www2.kau.se/jorrbomm/) is a project developed in as a team exercise.  
Kubus is a cube builder application intended to be used on iPads and other mobile units, but can also be used on your computer without any problem. It uses ThreeJS and jQuery with a PHP backend.
This project involved all parts of a larger project. Meetings with the customer, desigining the application, risks, testing and so on. In the end we delivered an application that is focused on math education for school classes in the ages 7-12 years.

Languages: **Javascript**, **PHP**, other techniques: **ThreeJS**, **jQuery**, **SCRUM**, **Teamwork**, **Responsive**

### Quiz-a-tron
![](/assets/img/ss+2015-04-30+at+12.42.24.png)
[Quiz-a-tron](http://www.christofferholmgren.se/quiz-a-tron/) is a quiz-making/-taking page.  
The backend runs PHP 5.4 and uses PostgreSQL as the database.
Code can be found [here](https://github.com/CCHolmgren/Quiz-a-tron).

Languages: **PHP**, other techniques: **PostgreSQL**, **Bootstrap**

### Ruby on Rails and AngularJS project
[Ruby on Rails and AngularJS project](https://github.com/CCHolmgren/ch222kv_1dv450_kod)  
A project to build an API using Ruby on Rails and Angular. Ruby on Rails provided the basic CRUD API and AngularJS on the front-end to consume that API. A PostgreSQL database was used to develop it, but because the peer reviewer couldn't get PostgreSQL to run, I switched it out for SQLite instead. Because of this the search functionality, which relied on SQL functions that SQLite doesn't provide, stopped working. However, the main part of the code should still work just fine with this minor incompatibility.

Languages: **Ruby**, **Javascript**, other techniques: **AngularJS**, **Ruby on Rails**, **PostgreSQL**, **SQLite**

### Forum/bookmark site
[Flask and SQLAlchemy Python project](https://github.com/CCHolmgren/individuellt_mjukvaruprojekt)  
This service was born from the idea to share bookmarks. Bookmarks aren't easy to share in general, and I wanted a quick and easy way to do that. The idea is that you save your links/bookmarks in collections (folders) and then you can share these collections with anybody that you want, easily. The project also includes a forum. 
The site uses Python and Flask for the webservice and SQLAlchemy as the ORM. Markdown is used in the forum and in the collections to provide styling and such without security problems.

Languages: **Python**, other techniques: **Flask**, **SQLAlchemy**

## 1DV449
[Webbteknik II](http://coursepress.lnu.se/kurs/webbteknik-ii/)  

>Kursen Webbteknik II vid Linnéuniversitetet
>
>Denna kurs fokuserar helt på webben. Kursen tar upp webbens historia, utveckling och betydelse för samhället, problem inom forskningen kring webben (Web Science). Kursen tar också upp optimering och säkerhet i webbapplikationer. Stort fokus kommer att ligga i att kunna hantera öppna Webb-API:er för att sammanfoga data i så kallade mashup-applikationer.

All in all a course focused on the web, how to develop API's and how to consume those API's. We developed a mashup-application, and my is called [Music Comparer](#music-comparer). We also did two smaller practical tasks.  

### Laboration 1 and Laboration 2 in 1DV449
[1DV449](https://github.com/CCHolmgren/1DV449_ch222kv)  
The first task was to develop a web scraper and scrape the coursepress.lnu.se page for courses. I did this using PHP and libcurl. And the code can be found [here](https://github.com/CCHolmgren/1DV449_ch222kv/tree/master/Laboration-1).
Languages: **PHP**
The next task was to take some bad code and make it better. Improve the security of it, optimize the loadtime of the page and also implement a simple long polling functionality to provide a simple chat. The code can be found [here](https://github.com/CCHolmgren/1DV449_ch222kv/tree/master/Laboration-2) with all the notes of changes that I did. 

The last task was to do a mashup-application, which you can find above in the [showcase](#music-comparer).