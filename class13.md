## LOCAL STORAGE FOR WEB APPLICATIONS
*ersistent local storage is one of the areas where native client applications have held an advantage over web applications. the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.*

**Historically**
web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:
- Cookies are included with every HTTP request,thereby slowing down your web application by needlessly transmitting the same data over and over
- Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
- Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful
  - a lot of storage space
  - on the client
  - that persists beyond a page refresh
  - and isn’t transmitted to the server


## A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5
In the beginning, there was only Internet Explorer. Or at least, that’s what Microsoft wanted the world to think. To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer.

**In 2002**
Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment, the feature is properly known as Local Shared Objects. Briefly, it allows Flash objects to store up to 100 KB of data per domain. Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System), but it was limited by some of Flash’s design quirks. By 2006, with the advent of ExternalInterface in Flash 8, accessing LSOs from JavaScript became an order of magnitude easier and faster. Brad rewrote AMASS and integrated it into the popular Dojo Toolkit under the moniker dojox.storage. 

**In 2007**
 Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers. (We’ve previously discussed Gears in the context of providing a geolocation API in Internet Explorer.) Gears provides an API to an embedded SQL database based on SQLite. 

 *So this is the problem that **HTML5** set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.*

 ## HTML5 STORAGE
 is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons. Certain browser vendors also refer to it as “Local Storage” or “DOM Storage.” 


HTML5 STORAGE SUPPORT
- IE  8.0+
- FIREFOX	3.5+
- SAFARI 4.0+
- CHROME	4.0+
- OPERA	 10.5+
- IPHONE	2.0+
- ANDROID 2.0+
				

## USING HTML5 STORAGE
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string.

## TRACKING CHANGES TO THE HTML5 STORAGE AREA
 you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. For example, if you set an item to its existing value or call clear() when there are no named keys, the storage event will not fire, because nothing actually changed in the storage area.
 The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9).

 ## LIMITATIONS IN CURRENT BROWSERS
 how much storage space each origin gets by default?
  This is surprisingly consistent across browsers, although it is phrased as no more than a suggestion in the HTML5 Storage specification. One thing to keep in mind is that you’re storing strings, not data in its original format. If you’re storing a lot of integers or floats, the difference in representation can really add up. Each digit in that float is being stored as a character, not in the usual representation of a floating point number.
 Can I ask the user for more storage space?
    At time of writing (February 2011), no browser supports any mechanism for web developers to request more storage space. Some browsers (like Opera) allow the user to control each site’s storage quota, but it is purely a user-initiated action, not something that you as a web developer can build into your web application.

## HTML5 STORAGE IN ACTION
*Make a few moves, then close the browser tab, then re-open it. If your browser supports HTML5 Storage, the demonstration page should magically remember your exact position within the game, including the number of moves you’ve made, the position of each of the pieces on the board, and even whether a particular piece is selected.*

## BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
One vision is an acronym that you probably know already: SQL. In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database specification. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database.

The Web SQL Database specification has been implemented by four browsers and platforms.

WEB SQL DATABASE SUPPORT
- IE  ·
- FIREFOX	·
- SAFARI 4.0+
- CHROME	4.0+
- OPERA	 10.5+
- IPHONE	3.0+
- ANDROID 2.0+

## FURTHER READING
- HTML5 storage:

  - HTML5 Storage specification
  - Introduction to DOM Storage on MSDN
  - Web Storage: easier, more powerful client-side data storage on Opera Developer Community
  - DOM Storage on Mozilla Developer Center. (Note: most of this page is devoted to Firefox’s prototype implementation of a globalStorage object, a non-standard precursor to localStorage. Mozilla added support for the standard localStorage interface in Firefox 3.5.)
  - Unlock local storage for mobile Web applications with HTML5, a tutorial on IBM DeveloperWorks
 
- Web SQL Database:
  - Web SQL Database specification
  - Introducing Web SQL Databases
  - Web Database demonstration
  - persistence.js, an “asynchronous JavaScript ORM” built on top of Web SQL Database and Gears