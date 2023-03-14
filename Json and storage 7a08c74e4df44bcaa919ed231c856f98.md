# Json and storage

JSON JavaScript Object Notation (JSON) is **a standard text-based format for representing structured data based on JavaScript object syntax**
. It is commonly used for transmitting data in web applications

lightweight format for storing and transporting data

JSON is often used when data is sent from a server to a web page

JSON is "self-describing" and easy to understand

•its string with a specified data format — it contains only properties, no method

 it supports the following two data structures −

- **Collection of name/value pairs** − This Data Structure is supported by different programming languages.
- **Ordered list of values** − It includes array, list, vector or sequence etc.
- • Creation of an empty Object −

```jsx
var JSONObj = {};
```

- Creation of a new Object −
- 

```jsx
var JSONObj = new Object();
```

```jsx
<html>
   <head>
      <title>Creating Object JSON with JavaScript</title>
      <script language = "javascript" >
         var JSONObj = { "name" : "tutorialspoint.com", "year"  : 2005 };
		
         document.write("<h1>JSON with JavaScript example</h1>");
         document.write("<br>");
         document.write("<h3>Website Name = "+JSONObj.name+"</h3>");  
         document.write("<h3>Year = "+JSONObj.year+"</h3>");  
      </script>
   </head>
   
   <body>
   </body>	
</html>
```

## **storage**

there is two types of storage -****Local Storage, session Storage****

The main features of local storage are:

- Shared between all tabs and windows from the same origin.
- The data does not expire. It remains after the browser restart and even OS reboot.

## **session storage**

The session storage object is used much less often than session storage

Properties and methods are the same, but it’s much more limited:

- The session storage exists only within the current browser tab.
    - Another tab with the same page will have a different storage.
    - But it is shared between iframes in the same tab (assuming they come from the same origin).
- The data survives page refresh, but not closing/opening the tab.

Let’s see that in action.

Run this code…

```jsx
sessionStorage.setItem('test', 1);
alert( sessionStorage.getItem('test') );
```

But if you open the same page in another tab, and try again there, the code above returns null, meaning “nothing found”.

That’s exactly because session storage  is bound not only to the origin, but also to the browser tab. For that reason, session storage  is used sparingly.

Web storage objects local storage and session storage allow to store key/value pairs in the browser.

- Both key and value must be strings.
- The limit is 5mb+, depends on the browser.
- They do not expire.
- The data is bound to the origin (domain/port/protocol).

**local Storage**

Shared between all tabs and windows with the same origin

Survives browser restart

**session Storage**

Visible within a browser tab, including iframes from the same origin

Survives page refresh (but not tab close)

Here is an example of how to set a key in local storage using JavaScript:

```
// set key
localStorage.test = 2;

```

Here is an example of how to get a key from local storage:

```
// get key
alert( localStorage.test ); // 2

```

Here is an example of how to remove a key from local storage:

```
// remove key
delete localStorage.test;

```

Remember that both the key and the value must be strings, and the data will remain in local storage even after the browser is restarted.

Here is an example of how to set a key in session storage using JavaScript:

```
// set key
sessionStorage.setItem('test', 1);

```

**Here is an example of how to get a key from session storage:

```
// get key
alert( sessionStorage.getItem('test') ); // 1

```

Here is an example of how to remove a key from session storage:

```
// remove key
sessionStorage.removeItem('test');

```

Remember that both the key and the value must be strings, and the data will remain in session storage even after the page is refreshed. However, it will be cleared when the tab is closed or the browser is restarted.