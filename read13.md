# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS 

For native applications, the operating system typically provides an abstraction layer for storing and 
retrieving application-specific data like preferences or runtime state. These values may be stored in the
registry, INI files, XML files, or some other place according to platform convention. If your native client 
application needs local storage beyond key/value pairs, you can embed your own database, invent 
your own file format, or any number of other solutions.


What we really want is

a lot of storage space
on the client
that persists beyond a page refresh
and isn’t transmitted to the server
Before HTML5, all attempts to achieve this were ultimately unsatisfactory in different ways.

So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value 
pairs locally, within the client web browser. Like cookies, this data persists even after
you navigate away from the web site, close your browser tab, exit your browser, or what
have you. Unlike cookies, this data is never transmitted to the remote web server (unless you 
go out of your way to send it manually). Unlike all previous attempts at providing persistent
local storage, it is implemented natively in web browsers, so it is available even when third-party 
browser plugins are not. 

 you can use Modernizr to detect support for HTML5 Storage.

if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}

__________________________________________________________________________________________________________________________________________________________

## USING HTML5 STORAGE
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};


At this point, the variable e will be a StorageEvent object, which has the following useful properties.

## STORAGEEVENT OBJECT
PROPERTY	TYPE	DESCRIPTION
key	string	the named key that was added, removed, or modified
oldValue	any	the previous value (now overwritten), or null if a new item was added
newValue	any	the new value, or null if an item was removed
url*	string	the page which called a method that triggered this change
* Note: the url property was originally called uri. Some browsers shipped with that property before the
specification changed. For maximum compatibility, you should check whether the url 
property exists, and if not, check for the uri property instead.


## LIMITATIONS IN CURRENT BROWSERS
In talking about the history of local storage hacks using third-party plugins, I made a point
of mentioning the limitations of each technique, such as storage limits. I just realized that I haven’t
mentioned anything about the limitations of the now-standardized HTML5 Storage. 


 actual working code in 4 browsers

openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {
  db.changeVersion('', '1.0', function (t) {
    t.executeSql('CREATE TABLE docids (id, name)');
  }, error);
});
As you can see, most of the action resides in the string you pass to the executeSql method.
This string can be any supported SQL statement, including SELECT, UPDATE, INSERT, and DELETE
statements. It’s just like backend database programming, except you’re doing it from JavaScript!
Oh joy!

the Web SQL Database specification has been implemented by four browsers and platforms.
I’ll give you the answers first, then explain them. The answers, in order of importance, 
are “5 megabytes,” “QUOTA_EXCEEDED_ERR,” and “no.”


