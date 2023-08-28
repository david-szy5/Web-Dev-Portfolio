# University of Southern California - CSCI 571 - Web Technologies
## David Szymulewski Project Portfolio

### Table of Contents
- [Projects overiew](#overview)
- [Project 1: Events Search Web Application - Version 1](#homework-1)
  * [Application Overview](#application-overview-1)
  * [Demo Video](#demo-video-1)
  * [Screenshots of Key Features](#screenshots-1)
- [Project 2: Events Search Web Application - Version 2](#homework-2)
  * [Application Overview](#application-overview-2)
  * [Demo Video - Desktop](#demo-video-2)
  * [Screenshots of Key Features - Desktop](#screenshots-2)
  * [Demo Video - Mobile](#demo-video-2-1)
  * [Screenshots of Key Features - Mobile](#screenshots-2-1)
- [Project 3: Events Search iOS App](#homework-3)
  * [Application Overview](#application-overview-3)
  * [Demo Video](#demo-video-3)
  * [Screenshots of Key Features](#screenshots-3)

### Course and Projects Overview
CSCI 571 at the University of Southern California is a graduate-level course that covers many of the current technologies and languages related to web, such as

- Front-end design with HTML, CSS, Bootstrap and SwiftUI
- Back-end programming implemented with Python and JavaScript using frameworks like Node.js, Express.js and Flask
- Client-side programming using JavaScript, TypeScript and Swift
- Building scalable, component-based web applications using Angular
- Designing iOS apps
- How to host applications on cloud platforms such as AWS, GCP and Azure
- Responsive web design
- AJAX and JSON

Students apply the knowledge that they have learned over the course of the semester by designing and building from scratch several iterations of an events search application--two web applications and one iOS app. Despite employing various frontend and backend technologies, all three iterations of the application share a common theme: to allow the user to search events--ranging from concerts to sporting events to theater--happening anywhere in the world and to view all information related to that event. Users have at their fingertips artist or team info such as Spotify profiles or future event dates, venue info such as location, hours or rules and, of course, general info about the event itself.

With this general theme in mind, the subsequent sections describe each iteration of the application in terms of the technologies used and their implementations. Each section includes a demo video and screenshots & explanations of the key features of each application.

### Project 1: Events Search Web Application - Version 1
<a name="homework-1"/>

#### Application Overview
<a name="application-overview-1"/>

##### Front-end / Client-side:
- HTML & CSS rendered dynamically via user interaction (clicks, searches, etc.)
- Client-side programming using JavaScript to send requests and receive responses from backend server
##### Back-end:
- Programmed in Python using Flask as the routing framework
- Fulfills client requests asynchronously by making calls to the Ticketmaster, Google Maps, Google Geocoding and Ipinfo APIs
- Hosted on AWS Elastic Beanstalk

#### Demo Video
<a name="demo-video-1"/>

[![Demo video](https://github.com/david-szy5/Web-Dev-Portfolio/assets/89551660/99aec398-d0ec-49fd-8c1e-2c6d1f14f5ae)]([https://youtu.be/vt5fpE0bzSY](https://youtu.be/0HZWqXPD634))

#### Screenshots of Key Features
<a name="screenshots-1"/>

| **Search form** <img width="1218" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/340b07f7-9d11-46a5-8390-43ec531f6217"> |
|:--:|
| The main search form of the application. User can input a keyword (e.g., "Basketball" or "Taylor Swift"), search radius, search category and search location. After the "SEARCH" button is pressed, the query parameters are collected and relayed to the back-end for parsing. |

| **Sample query and results** <img width="1552" alt="hw6_img02" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/64b4b47c-b307-494f-b37f-0983017a114a"> |
|:--:|
| An example query using manual input for location (Los Angeles). Search results are sorted in descending order of date and time. Users are able to click an individual row for more information about that event. |

| **Event information** <img width="1552" alt="hw6_img03" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/a37c05e6-5a62-462b-aad9-fa14477214f4"> |
|:--:|
| A details card containing useful information pertaining to the selected event. The Ticketmaster API provides information such as event date and time, artist and team Ticketmaster links, venue name, genres (if relevant), ticket price and status, and a link to the event's Ticketmaster page. |

| **Example Ticketmaster page** <img width="1373" alt="hw6_img04" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/d8452986-bd5b-42ac-9bbf-951ab7f579d7"> |
|:--:|
| An example Ticketmaster page for Taylor Swift after clicking the "Taylor Swift" hyperlink under the Artist/Team subheader in the above details card. |

| **Buy tickets** <img width="1416" alt="hw6_img05" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/43d7650c-8c8c-413a-b479-383ff216160e"> |
|:--:|
| An example Ticketmaster page for purchasing tickets to a Taylor Swift concert. In this case, none are available. |

| **Show venue details** <img width="1238" alt="hw6_img06" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/f8351fef-dc9f-4da2-ab16-9f7d314160fd"> |
|:--:|
| A button located under the event details card to display more information about the venue. |

| **Venue Details** <img width="1238" alt="hw6_img07" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/bff16758-8a83-4e12-bd22-4349b1e7f7d4"> |
|:--:|
| A details card containing information about the selected venue. The user can find the venue on Google Maps and explore other events at the venue. |

| **Example Google Maps view** <img width="1353" alt="hw6_img08" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/250f8553-5e6d-43d6-9adb-ad17293dc972"> |
|:--:|
| An example view of the location of the venue on Google Maps. |

| **Explore other events at the selected venue** <img width="1357" alt="hw6_img09" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/60833d3a-9d24-4ec3-a5b9-a86d5ea3ba39"> |
|:--:|
| The view of the Ticketmaster page after the user clicks the "More events at this venue" hyperlink on the venue details card. |

### Project 2: Events Search Web Application - Version 2
<a name="homework-2"/>

#### Application Overview
<a name="application-overview-2"/>

##### Front-end / Client-side:
- HTML, Bootstrap, and _minimal_ CSS rendered dynamically via user interaction (clicks, searches, etc.)
- Angular, TypeScript and Bootstrap combined to deliver a responsive client experience on desktops _and_ mobile phones
- Use of Bootstrap classes allow for a more interesting and interactive user experience with carousels, modals, etc.
- Client-side programming using TypeScript (Angular) to manage state variables and user information (e.g., favorited events), and to send/receive requests/responses to/from the back-end server
##### Back-end:
- Programmed in JavaScript using Node.js as the server and Express.js as the routing framework
- Fulfills client requests asynchronously by making calls to the Ticketmaster, Spotify, Google Maps, Google Geocoding, Ipinfo, Facebook and Twitter APIs
- Hosted on AWS Elastic Beanstalk

#### Demo Video - Desktop
<a name="demo-video-2"/>

https://github.com/david-szy5/david-szy5.github.io/assets/89551660/0930f16e-9c00-46dd-b04e-47f89215d9dc

#### Screenshots of Key Features - Desktop
<a name="screenshots-2"/>

| **Events search home page** ![hw8_img01](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/57cda07d-ace8-4792-8bc2-9d23e77171b2) |
|:--:|
| This is the home page for the application. It features a search form that is very similar to that of version 1. The top-right corner of the page allows the user to switch between the search form and a list of their favorited events. |


**_Auto-complete feature_**
| ![hw8_img02](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/43f72f58-213d-4a9d-a401-993c02df6a00) |
|:--:|
| A debounced auto-complete feature using the Ticketmaster Suggest API. |


**_Sample search results_**
| ![hw8_img03](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/db3130a4-8500-46e4-827a-7ce90732158f) |
|:--:|
| A redesigned search results table using Bootstrap classes. A user may click any individual row to view more information about that event. |


**_Event details tab_**
| ![hw8_img04](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/e95c5f07-130d-406f-a700-89ea22244a8c) |
|:--:|
| After clicking a row in the results table, the user is first presented with a details card containing various information about the event they selected. The user is also able to share the event on Facebook and Twitter. |


**_Artist details tab_**
| ![hw8_img05](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/6bf38eb8-a233-4446-8418-79abdb1a84ad) |
|:--:|
| Clicking the "Artist/Teams" tab presents the user with information about the artists or teams related to the event they are viewing. For music-related artists, various information about their Spotify profiles is displayed along with their top-3 albums. |


**_Artist details tab - navigating the carousel_**
| ![hw8_img06](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/0577a546-a5e4-42a7-8455-5a6fc1f22bd9) |
|:--:|
| The user is able to click the left & right arrows on the details card to cycle through the other artists or teams related to the event. |


**_Example artist Spotify page_**
| ![hw8_img07](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/a8b524d7-1a30-4473-ad92-8d7123fe7ca2) |
|:--:|
| After clicking an artist's Spotify link the user is presented with the associated Spotify profile. |


**_Venue details tab_**
| ![hw8_img08](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/ffe3ebc4-1cd0-4d34-b6b3-d139f261f46d) |
|:--:|
| The user can also view various information about the venue at which the event is held at. |


**_Google Maps modal_**
| ![hw8_img09](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/a8dc0fbf-5e8d-4512-b7eb-0e991f82ed26) |
|:--:|
| An example Google Maps modal showing the location of the selected venue. |


**_Add an event to your favorites_**
| ![hw8_img10](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/b86655f3-462f-4cdf-a7c4-48c0a4fef6f2) |
|:--:|
| Simply click the heart-shaped icon near the event name to add it to your favorites! |


**_List of your favorite events_**
| ![hw8_img11](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/62a7d29a-c851-42be-8815-ad6cdefb13d2) |
|:--:|
| The favorites page containts a list of all your favorited events. |

#### Demo Video - Mobile
<a name="demo-video-2-1"/>

https://github.com/david-szy5/david-szy5.github.io/assets/89551660/ca867334-7eb3-4909-9521-18b8a8279559

#### Screenshots of Key Features - Mobile
<a name="screenshots-2-1"/>

**_Search form - mobile_**
| ![hw8_img_20](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/27664dea-8c67-4fde-98fd-670a8c36d298) |
|:--:|
| Mobile view of the search form. |


**_Search results - mobile_**
| ![hw8_img_21](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/2d62e963-f3a5-43b2-bd6b-b8afa4b1fad4) |
|:--:|
| Mobile view of the responsive results table. |


**_Event details tab - mobile_**
| ![hw8_img22](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/57c3593e-c00f-489a-a186-c7b4b174ed45) |
|:--:|
| Mobile view of the event details tab. |


**_Artist / Team details tab - mobile_**
| ![hw8_img23](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/ba1fa429-18f1-4990-847e-ae9360fd692d) |
|:--:|
| Mobile view of the artist / team details tab. |


**_Venu details tab - mobile_**
| ![hw8_img24](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/2680c5e4-0b12-4cc9-b526-de8ee1210bef) |
|:--:|
| Mobile view of the venue details tab. |


**_Favorited events - mobile_**
| ![hw8_img25](https://github.com/david-szy5/david-szy5.github.io/assets/89551660/2690edd2-9439-4db8-91b7-d35d4e5d3e01) |
|:--:|
| Mobile view of the user's favorited events. |

### Project 3: Events Search iOS App
<a name="homework-3"/>

#### Application Overview
<a name="application-overview-3"/>

##### Front-end / Client-side:
- Swift and SwiftUI combined to deliver a clean and simple app interface, iterating on previous versions of the application
##### Back-end (identical to Version 2):
- Programmed in JavaScript using Node.js as the server and Express.js as the routing framework
- Fulfills client requests asynchronously by making calls to the Ticketmaster, Spotify, Google Maps, Google Geocoding, Ipinfo, Facebook and Twitter APIs
- Hosted on AWS Elastic Beanstalk

#### Demo Video
<a name="demo-video-3"/>


https://github.com/david-szy5/david-szy5.github.io/assets/89551660/c0e6d0e4-4cd2-4396-acec-fc6a0a9c8825


#### Screenshots of Key Features
<a name="screenshots-3"/>


| **Sample query and results** <img width="408" alt="hw9_img1" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/6f4436e8-18f4-4ecf-9e13-06ee3857a339"> |
|:--:|
| An example query using the auto-detect location feature. Search results are sorted in descending order of date and time. Users are able to click an individual row for more information about that event. |


| **Event information tab** <img width="408" alt="hw9_img2" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/d92cffa1-1264-4e83-86d5-7f53aef4cd3d"> |
|:--:|
| After tapping on a row in the results table, the user is presented with a details card containing various information about the event they selected. The user is also able to share the event on Facebook and Twitter. |


| **Artist information tab** <img width="408" alt="hw9_img3" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/28c5587f-4164-424f-a57e-961ae815b36a"> |
|:--:|
| Tapping the "Artist/Teams" tab presents the user with information about the artists or teams related to the event they are viewing. For music-related artists, various information about their Spotify profiles is displayed along with their top-3 albums. |


| **Venue information tab** <img width="408" alt="hw9_img4" src="https://github.com/david-szy5/david-szy5.github.io/assets/89551660/9385c104-1a1e-4b0e-ad33-7c5cf0fee89a"> |
|:--:|
| Users can also view information pertaining to the venue at which the event is hosted. |
