# Terse introduction to web programming

## Me
  Murilo Pereira
  http://mpereira.com
  @mpereira

  Computer science dropout

  Meleva
  Helping people share taxis in Brazil

  I've been programming professionally since 2010, which is just 2 years after
  I started programming. My first job was at an american company earning more
  than my graduated peers just one year after I started programming. They also
  flew me to the US periodically to attend to conferences and company meetings.

## Why should you care?
  If you plan to start your own company you'll find it hard to encounter good
  engineers (programmers, system admins, etc.) to implement your idea.
  Outsourcing or working with freelancers is also hard to get it right and is
  not a sustainable way to build complex products.

  Learning to program computers will not just allow you to start implementing
  your ideas yourself but also will help you hiring technical people. It will
  also help you understand and appreciate the technology and science around
  things made with computers.

## What's the world wide web made of?

### Web browsers and servers

  When you open your web browser (IE, Firefox, Chrome, etc.) and type in
  www.facebook.com, the browser figure out the *address* of that *URL*

  URL: www.facebook.com (what I want)
  Address: ? (where is it)

  Analogy:

  Venue: Costanera Center (what I want)
  Address: Avda. Andrés Bello 2425, Providencia, Santiago, Chile (where it is)

  Addresses on the internet are called *IP Addresses*. They are a sequence of
  numbers and dots like *31.13.69.160* (this is www.facebook.com's IP address as
  I prepare this presentation).

  After the web browser has the address of the website you want to visit, it
  sends a request to that address asking for the web page.

  [Web browser] --- I want the web page for www.facebook.com --> [31.13.69.160]

  This request is going to be received by a Facebook computer, *a web server*.
  It's called a **server** because it serves web pages.

  The server responds to the request with the web page, which is a file. The
  web browser receives this file and renders it, showing your timeline, filled
  with pictures from last night of your friends partying and videos of cats
  doing funny things.

### HTML
  The file sent by the server and rendered by the web browser is an HTML file.
  This kind of file is made of text formatted in a special way that browsers
  understand. This format is the language used to write web pages.

  Example:

  File name: index.html

  File contents:
  <html>
    <body>
      <h1>Hello World</h1>

      <p>First steps in HTML<p>
    </body>
  </html>

  This is an HTML file. That's what you would see if you opened it on a text
  editor like Notepad on Windows or TextEdit on a Mac.

  If you open an HTML file on a web browser, it does not display the tags
  enclosed in angle brackets. It interprets them to understand the contents of
  the file. On the example above, the browser would know that the file consists
  of a header and a paragraph, represented by the *h1* and the *p* tags,
  respectively.

  HTML is used to represent the *content* of web pages (text, images, links,
  etc.).

### CSS
  Along with the HTML file may come a CSS file. CSS is a language used to
  specify how the HTML should be rendered on web browsers. It says how the
  layout, colors and fonts should look like.

  Example:

  File name: style.css

  File contents:
  body { background-color: yellow; }

  h1 { font-size: 30px; }

  p { font-family: Helvetica }

  CSS is used to describe the *presentation* of web pages (how they look).

### JavaScript
  JavaScript is a programming language used to manipulate web pages. With it
  it's possible to make changes to the HTML file that your web browser receives
  from the web server.

    https://www.facebook.com/zuck

    var profilePic = document.getElementsByClassName('profilePic')[0];
    profilePic.src = 'http://i276.photobucket.com/albums/kk8/martinthurssoon/th_ZuckerMovie.gif';
    profilePic.src = 'http://cdn.uproxx.com/wp-content/uploads/2012/05/mark-zuckerberg.jpg';
    var profileName = document.getElementsByClassName('-cx-PRIVATE-fbTimelineLightHeader__nameLink')[0];
    profileName.innerHTML = 'Marky Zubemkerg $$$';
    var nyanCat = document.createElement('img');
    nyanCat.src = 'http://fc05.deviantart.net/fs70/f/2012/168/e/4/nyan_cat__sparta__gif__by_lookincool45-d53trrz.gif';
    nyanCat.style.position = 'absolute';
    nyanCat.style.top = '250px';
    nyanCat.style.left = '150px';
    nyanCat.style.width = '80%';
    nyanCat.style.zIndex = '1000';

    http://en.wikipedia.org/wiki/Barack_Obama

    var image = document.getElementsByClassName('image')[0].getElementsByTagName('img')[0];
    image.src = 'http://i.minus.com/ibnMfO5dXlo1FG.gif';

## Practical uses
  You can use HTML, CSS and JavaScript to make lots of things:
  - Web sites
  - Games
  - Mobile applications

  With JavaScript alone you can program pretty much anything:
  - Web servers
  - Robots
  - Flying robots
  - Laser beams

### Example game made using HTML, CSS and JavaScript
  http://youtu.be/YCb81WvFg4U

## Summing up
  - Learning how to program allows you to implement your own ideas
  - Getting the basics is not hard and can get you a long way
  - Even if you are not interested in following a programming career, having
    a decent grasp of how computers work will change the way you solve problems
  - Programming is fun and you should do it

## Inspiration
  http://youtu.be/nKIu9yen5nc

## Further reading
  "Aprende como hacer sítios web", by Mozilla
  https://developer.mozilla.org/es/learn

  Video series introducing HTML, CSS and JavaScript, by Google
  http://youtu.be/60O1CJqh8IM

  Video of a JavaScript powered robot
  http://youtu.be/GVGMjsKy3WQ

  Programming flying robots with JavaScript
  http://nodecopter.com/

  Create mobile applications with HTML, CSS and JavaScript
  http://phonegap.com/
