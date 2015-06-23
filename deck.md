<!--
master: title-page
custom: 
  0:
    margin-top: 72px
  2: 
    margin-top: 100px
    color: "#888"

todo: |
      demo some es5 code
      demo some es6 features
      (will this be live or just code examples?)
      


-->

# Growing up with JavaScript
## History & Future of an Oddball
## @davidmarkclem

---
<!--

master: image-caption
custom:
  1:
    margin-top: 15px
  2:
    width: 550px
    margin-top: 1px
notes: |
        in many ways this talk will be more 
        gratuitously egotistical and self involved than 
        a Facebook profile

        I assure you though, it's just for fun, it's
        not like I have a Russel Brand complex, a.k.a
        a messiah complex.... 

        in 32 BD... 

-->

# Warning: Gratuitously Egotistical

![](/images/fb.png)

...more self-involved than a Facebook Profile


---
<!--
master: section-title
-->

# 32 BD

---
<!--
master: section-title
notes: |
        John W Backus gets fed up with ASM
        submits a proposal to his employer, IBM: fortran
        mathematical formula translating system
        first fortran compiler, 1957
        reduced necessary statements by factor of 20

-->


# 32 BD
## (1953)

---
<!--
master: image
custom:
  1:
    margin-top: 40px
notes: |
        John W Backus gets fed up with ASM
        submits a proposal to his employer, IBM: fortran
        mathematical formula translating system
        first fortran compiler, 1957
        reduced necessary statements by factor of 20
-->

# FORTRAN

![](/images/fortran.jpg)

---
<!--
master: code

-->

# FORTRAN

<pre class="language-fortan">
<code class="language-fortan">
C AREA OF A TRIANGLE - HERON'S FORMULA
C INPUT - CARD READER UNIT 5, INTEGER INPUT
C OUTPUT - LINE PRINTER UNIT 6, REAL OUTPUT
C INPUT ERROR DISPAY ERROR OUTPUT CODE 1 IN JOB CONTROL LISTING

      INTEGER A,B,C
      READ(5,501) A,B,C
  501 FORMAT(3I5)
      IF(A.EQ.0 .OR. B.EQ.0 .OR. C.EQ.0) STOP 1
      S = (A + B + C) / 2.0
      AREA = SQRT( S * (S - A) * (S - B) * (S - C) )
      WRITE(6,601) A,B,C,AREA
  601 FORMAT(4H A= ,I5,5H  B= ,I5,5H  C= ,I5,8H  AREA= ,F10.2,12HSQUARE UNITS)
      STOP
      END
</code>
</pre>

---
<!--
master: section-title
notes: |
  two extremely important developments to JavaScript
  lisp and algol-58

  lisp, algol and fortran are the three (great) grandfathers 
  of JavaScript
  (but fortran is more like a step-grandfather)
-->


# 27 BD
## (1958)

---
<!--
master: code
notes: |
        ALGOrightmic Language

        ALGOL-58 === IAL === International Algebraic Language

        inspiration for many, many modern langs
        design by committee (European and American computer scientists)

        lots of subsequent ALGOL flavours (system driven, need driven)

        example code was for the Elliot-803 Computer's implementation 
        (a large subset of Algol 60). example creates a table
-->

# ALGOL

<pre class="language-algol">
<code class="language-algol">
 FLOATING POINT ALGOL TEST'
 BEGIN REAL A,B,C,D'
  
 READ D'
  
 FOR A:= 0.0 STEP D UNTIL 6.3 DO
 BEGIN
   PRINT PUNCH(3),££L??'
   B := SIN(A)'
   C := COS(A)'
   PRINT PUNCH(3),SAMELINE,ALIGNED(1,6),A,B,C'
 END'
 END'
</code>
</pre>

---
<!--
master: code
notes: |
        used for AI

        homoiconicity
          data structure and programmatic syntax are the same
          that is, instructions are represented as lisp lists,
          (a data structure). It means you don't need to parse
          the code to generate an AST, the code IS the AST.

        Lots of Irritating Superfluous Parentheses
          again this goes back to homoiconicty, the parens
          make expression boundaries completely clear to the interpreter

        in JS, the example is actually parseable. 

        wrap in a function without calling it, or declare the vars
        var LABEL, LENGTH, LAMBDA, Y, COND, NULL, QUOTE, T, SUM, CDR
        or function l() { /* etc */ }
-->

# LISP

<pre class="language-lisp">
<code class="language-lisp">
(LABEL,LENGTH, (LAMBDA, (Y), (COND, ((NULL, Y), <BR>(QUOTE,0.0)), (T, (SUM, (LENGTH, (CDR, Y)), <BR>(QUOTE, 1.0))))))
</code>
</pre>



---
<!--
master: section-title
notes: |
        1960 - Theodore Nelson coins the term "hypertext"
        1962 - Creation of Simula, the first OOP language
        1964 - creation of the original BASIC language
        1965 - two MIT's computers communicate with packet switching
        5th August 1968 - first public demo of packet switching
                          (instead of circuit switching, point to point, like phones)
        29th October 1969   first successful message sent over ARPANET
                            an hour prior the letter "L" and "O" were sent
                            but the system crash, the full message was "LOGIN",
                            but maybe, just maybe the first message was actually
                            "LOL! HERE COMES TEH GOOGLE TUBES!!!11!!"

-->

# 25 - 15 BD
## (1960 - 1970)

---
<!--
master: section-title
notes: |
       70's saw development of the actor model
       early 70's: scheme (71-72ish), C,  72-80 development of smalltalk
       79 release of C++, 80 release of smalltalk 80
       smalltalk was an educational tool
       but turned out to have some really powerful paradigms (WHAT PARADIGMS?)
       1974 - first ever ISP, Telenet, commercial version of ARPANET
       1978 - great chicago blizzard, two guys cobble together first BBS
       1979 also saw the first proprietary consumer online services
       1979 - The Source "It's not hardware, it's not software. But it can take your personal computer anywhere in the world". 
       1979 - CompuServes MicroNET
       CompuServe later bough the Source, and was eventually bought by AOL
-->

# 15 - 5 BD
## (1970 - 1980)

---
<!--
master: section-title
notes: |
        1982
        Former bassist of the band "Oceanrock", finds that most 8-bit
        adventure-style games are "too verbose" - he essentially
        believes that taking a subset of the "good parts" of a
        traditional adventure game will lead to an elegant and entertaining 
        action game. He's right, after writing a medieval game originally
        called "Knightsoil", Atari notice the talent and hire him. 
-->

# 3 BD
## (1982)

---
<!--
master: image
notes: |
        1982 also saw the release of an awesome cartoon called Danger Mouse
-->

# Galahad and the Holy Grail
![](/images/gallahad.png)

---
<!--
master: section-title
notes: |
        born
        release of the Atari 65XE
        first ever registered domain - symbolics.com (symbolics computer corp)
          the creators of lisp!
          mentioned in jurrasic park :D in the 90's
        
        National Science Foundation Network (NSFNET) is launched, 
        it has 2000 connected computers

        Hypercard is created, followed by hypertalk in 1986
-->

# 0 DB (1985)

---
<!--
master: image
custom:
  1:  
    width: 680px
notes: |
        1985
        Hypercard is created, 
-->

# Hypercard

![](/images/cyberpunkstack.jpg) 

---
<!--
master: section-title
notes: | 
        self designed in 86
        compiler written in 87
        prototype language (smalltalk without classes)
        self was released to public in 1990
        hypertalk added to hyperscript  
        By two years I would have been in
        stage 3 of *self* awareness "identification",
        ability to recognize myself in the mirror. 



-->

# 1986

---
<!--
master: image
custom:
  1:
    margin-top: 65px
notes: |
        1986
        logo says it all, objects are referenced by other objects
        not by classes

-->

# Self

![](/images/self.png)

---
<!--
master: code
custom:
  1:
    width: 630px
    height: 210px
notes: |  
        1986
        JS ancestor
        Applescript ancestor
-->

# Hypertalk

```javascript
on mouseDown
  answer file "Please select a text file to open."
  if it is empty then exit mouseDown
  put it into filePath
  if there is a file filePath then
    open file filePath
    read from file filePath until return
    put it into cd fld "some field"
    close file filePath
    set the textStyle of character 1 to 10 of card field "some field" to bold
  end if
end mouseDown
```

---
<!--
master: section-title
notes: |
        Compuserve introduces the GIF format
        much better than RLE (color, and anim)
-->

# 1987

---
<!--
master: image
custom:
  1: 
    width: 750px
notes: |
        1987
        Compuserve introduces the GIF format
        much better than RLE (color, and anim)
-->

# CompuServe brings us GIF

![](/images/cat-walking-funny.gif)

---
<!--
master: image
custom:
  1: 
    width: 575px
    margin-top: 13px
notes: |
        1987
        one of my earliest memories, very surreal,
        no one explains puppetry to 2 year olds
-->

# I was watching Rainbow

![](/images/zippy-o.gif)


---
<!--
master: section-title
notes: | 

        TCP/IP becomes the global standard for interconnected networks

        CERN (nuclear research org) opens it's first TCP/IP ports,
        exposing it's former internel intranets

        Australian universities also began using IP protocols to 
        unify network infrastructure

        Japan connected to NSFNET

        first commercial dial up access: world.std.com
-->

# 1989

---
<!--
master: image
custom:
  1:
    width: 350px
    margin-top: 10px
notes: |
        1989
        ...everything is awesome
-->

# And I was all like...

![](/images/young-me.jpg)


---
<!--
master: section-title
notes: | 
        1990

-->

# 1990

---
<!--
master: image
notes: |
        Tim Berners Lee architects the concept of the internet, 
        from the combined work of the last 60ish years.
        
        Derives HTML from SGML (Standard Generalized Markup Language)
        creates HTTP and brings it all together (TCP/IP, DNS etc)

        Tim Berners Lee writes the WorldWideWeb browser 
        (later called Nexus) - it was limited to BSD-flavoured NExT computers 
-->

# The Architect

![](/images/tim-berners-lee.jpg)


---
<!--
master: section-title
notes: | 
        High Performance Computing and Communication 
        Act of 1991 supplies funding to 
        National Center for Supercomputing Applications

        Work starts on a multi-protocol client (mosaic)
-->

# 1991


---
<!--
master: image
custom:
  1:
    img:
      padding-top: 0
      margin-top: 55px
notes: |

        honestly... I found the choo-choo more interesting

        but I had a babysitter, I haven't seen him since
        I was 6, but he looked something like this:
-->

# My Christmas Present

![](/images/Commodore-64.png)


---
<!--
master: image
custom:
  1:
    img:
      padding-top: 0
      margin-top: 55px
notes: |
        I called him michael blackhead, but that wasn't his name

        I identify with JS because we both have colourful backgrounds
-->

# My Babysitter

![](/images/michael blackhead.jpg)



---
<!--
master: image
custom:
  1:
    img:
      border: "5px solid #a19dff"
      border-left: "7px solid #a19dff"
      border-right: "7px solid #a19dff"
      border-radius: 3px
      padding-top: 0
      margin-top: 3%
-->

# This is what he showed me...

![](/images/PRINT DAVID.png)


---
<!--
master: image
custom:
  1:
    img:
      border: "5px solid #a19dff"
      border-left: "7px solid #a19dff"
      border-right: "7px solid #a19dff"
      border-radius: 3px
      padding-top: 0
      margin-top: 3%
-->

# ...I was astounded.

![](/images/RUN.png)

---
<!--
master: section-title
notes: |
       work begins on Mosaic - a multi-protocol client (ftp, gopher, http)

       multi-platform - Unix, Windows, Macintosh

       initial launch enabled the ability to inline images
       this was not per spec, Tim Berners Lee did not like it. 


       this dynamic (and some would have said reckless) approach
       also brought in the blink tag, the marquee tag, and eventually
       DOM scripting in the form of JavaScript (and also terrible
       GIF overcrowding)

       it gave people what they wanted - the visuals
       scripting also gave people what they wanted - the behaviours
       
       HTML was intended for docs not apps, Mosaic were the first to 
       begin re-purposing it for distributed networked app GUIs.

       The Erwise browser was also released, it underlined text links, 
       language barriers prevented larger adoption (docs were in Finnish)

       I received a mega drive, the commodore sees much less usage,
       we moved from the "tech creator generation" to the "tech consumer generation". No more command lines, just entertainment consoles. 

-->

# 1992

---
<!--
master: image
-->

# Got me a mega drive
![](/images/mega-drive.jpg)

---
<!--
master: section-title
notes: |
        Mosaic released to the public

        The mega drive and commodore get stolen by a customer
        of my step dad. 

        My step dad gets caught importing large containers
        of drugs onto Margate beach and goes to jail, I 
        get a new step dad. (like JavaScript, my history is coloured)

        My new step dad goes to bootfairs most weekends, we tend
        to get the about 6:30am on a sat or sun. People are selling
        Atari's for between one and three pound, I get a pound week
        pocket money. I end up with 4-5 Atari's, and a book on how
        to programme in basic. 

-->

# 1993


---
<!--
master: image
custom:
  1:
    width: 400px
    margin-top: 20px
notes: |
        also .. violaWWW, released 2 years prior was precursor to mosaic, 
        which used viola (an OO scripting language)
        to control elements (also had rudimentary form of CSS)

        the creator of violaWWW said, he basically took the concepts in the HyperCard manual and reimplemented them on X Windows (unix), 

        creator of viola then learned about Tim Berners Lees
        idea for URL's, he implemented those on top of "hyperlinks",
        Unix already TCP stack etc. ViolaWWW was ahead of it's time

-->

# Mosaic Released to the Public

![](/images/mosaic-logo.gif)

---
<!--
master: image
custom:
  1:
    width: 600px
    margin-top: 45px
notes: |
        Also in 1993 I began to pick up Atari's from bootfairs
-->

# Ataris!!!

![](/images/Atari-130XE.jpg)

---
<!--
master: image
custom:
  1:
    width: 600px
    margin-top: 30px
-->

# Ataris!!!

![](/images/Atari_1200XL.jpg)



---
<!--
master: image
custom:
  1:
    width: 600px
    margin-top: 5px
-->

# Ataris!!!

![](/images/Atari_800_2008_new.png)


---
<!--
master: image
custom:
  1:
    width: 600px
    margin-top: 45px
-->

# Ataris!!!

![](/images/Atari-800xl.jpg)



---
<!--
master: image
custom:
  1:
    width: 600px
    margin-top: 0px
-->

# Ataris!!!

![](/images/1280px-Atari_XEGS.jpg)


---
<!--
master: section-title
notes: |
        Mosaic Communications Corporation - April 4 1994
        Becomes Netscape Communications Corporation
        Rewrite Mosaic from scratch, call it Mosaic Netscape, 
        which is then renamed to Netscape Navigator
        Internal name for Netscape Navigator is... Mozilla,
        a portmanteau of "Mosaic Killer"

        Spyglass Inc. purchase NCSA Mosaic rights for millions,
        and also rewrite from scratch (because they inherit
        3 codebases, one for each OS but want a shared code base
        moving forward).

        We now live in a house with a basement, the ideal place
        for ... people like us. I get hold of a TV screen and 
        hook up an Atari, then work through the Basic programming 
        book. I really enjoy the short iteration cycles basic allows
        for, and immediate feedback of the CLI. 
        
-->

# 1994

---
<!--
master: section-title
-->

# Browsers Wars <span style="font-family: times">I</span>

---
<!--
master: image
custom:
  1:
    width: 450px
    margin-top: 10px
notes: |
        December 1994 - free for non-commercial use
-->

# Netscape is born

![](/images/netscape_logo.png)


---
<!--
master: section-title
notes: |
        netscape change their policy - only educational and non-profits
        could use it for free

        Brenden Eich, consulting with Netscape designs JavaScript in 10 days, in May 95


-->

# 1995

---
<!--
master: image
notes: |
        using an old IBM PC
        I'm not living with grandparents, 
        my Grandma has been doing a fairly out of
        date college course, using an old green screen IBM PC

        I'm addicted to this machine, on it for 2-3 hours a day
        after school. Eventually I manage to break it irreparably,
        Grandma loses all her coursework, never finishes the course.

        Replaces the IBM PC with a 386 with windows 3.1, 
        built by an IT teacher, his name was Mr Bean.
        For real. I broke the 386 several times,
        Mr Bean would come round and fix it for me. 
custom:
  1:
    width: 450px
    margin-top: 2px
-->

# I ruined my Grandmas education

![](/images/ibmpcat.jpg)

---
<!--
master: image
custom:
  1:
    width: 500px
    margin-top: 20px
-->

# i386, win 3.1

![](/images/win-3.1-pc.jpg)


---
<!--
master: image
custom:
  1:
    width: 450px
    margin-top: 120px
notes: |
        MicroSoft enter a license agreement with Spyglass Mosaic
        (another reimplementation, rights purchased from NCSA)

        MicroSoft bundle Internet Explorer with Windows, "for free",
        which means they avoid Spyglass license fees.
        Spyglass later sue for 8 million.
-->

# Internet Explorer is born

![](/images/ie1.png)


---
<!--
master: image
custom:
  1:
    width: 450px
    margin-top: 7px
-->

# 10 Days? np.

![](/images/brenden eich.jpg)


---
<!--
master: diagram
notes: |
        JavaScript is a language based on multiple compromises
        Brenden Eich was a fan of both
        self and scheme, when he came
        on board with netscape he said
        he wanted to write a scheme interpreter.
        
        When it came down to it, his mandate
        was to write a script language that 
        looks like Java. So he wrote a scheme
        interpreter with prototypical inheritance
        with Java-like syntax.

        Scheme also had dynamic typing 

-->

# JavaScript Ingredients


```diagram
graph LR;
  Scheme --First-class Functions--> JavaScript
  Self --Prototypal Model--> JavaScript
  Java --Obligatory Syntax--> JavaScript
```


---
<!--
master: diagram
custom:
  1:
    max-width: none
    padding-top: 0
    zoom: 0.5
    svg:
      padding-top: 2%
      max-width: none
notes: |
        Basic isn't in direct lineage but it was based on 
        fortran and algol 60

        lisp, algol and fortran are the granddaddies of js

        BCPL was first program to use braces,
        inspired the C syntax inherent in Java
        and JavaScript

        Smalltalk brought the "everything is an object" thing
        (primitives are actually immutable objects in JS)
-->

# JavaScript Heritage


```diagram
graph LR;
  subgraph
    Lisp --> Scheme
    Lisp --> Smalltalk
    Algol --> Simula
    Algol --> Pascal
    Algol --> CPL
    Fortran --> B
  end

  subgraph
    Simula --> Smalltalk
    Smalltalk --> Self
    Self --> JavaScript
    Smalltalk -.-> Actor{Actor Model}
    Smalltalk --> C++
  end

  subgraph
    Actor --> Scheme
    Scheme --> JavaScript
  end

  subgraph
    CPL --> BCPL
    BCPL --> B
    B --> C
    Pascal --> C
    C --> C++
    C --> Java
    C++ --> Java
    Java --> JavaScript
  end

  subgraph
    JavaScript
  end
```

---
<!--
master: section-title
-->

# 1996

---
<!--
master: image
custom:
  2:
    padding-top: 0
    zoom: 1.4
notes: | 
        March 1996 - 2.0 , August 1996 - 3.0 - IE 3.0 also Aug 1996, 
-->

# Netscape 2.0, Netscape 3.0
## JavaScript 1.0, JavaScript 1.1

![](/images/netscape-2-3.png)

---
<!--
master: image
custom:
  1:
    padding-top: 12.5%
    zoom: 1.8
notes: |
        July 16, 1996 - IE3 launches with JScript
        reverse engineered clone of JavaScript

        Faithfully reproduced all the bugs

        By this point, typical response was to JS: 
        JavaScript Sux
-->

# IE3 - JScript

![](/images/Internet_Explorer_3.0_banner.gif)

---
<!--
master: section-title
notes: |
        but as someone pointed out later...
-->

# JavaScript Sux

---
<!--
master: section-title
notes: |
        As someone pointed out later, 
        parts of it suck
-->

# JavaScript Has Sucky Parts

---
<!--
master: diagram
custom:
  1:
    svg:
      padding-top: 4%
notes: |
        Java syntax, not because of Java per se 
        but because of the application of the syntax
        to the scheme/self paradigms
-->

# Sucky Parts

```diagram

graph TD;
  
  Why --> Noob[Noob Friendly]
  Why --> Java[Java Syntax]
  Why{Why} --> Rushed

  Noob -.e.g.-> Implicit[Implicit Globals]
  Rushed -.e.g.-> n[typeof null]
  Java -.e.g.-> new
```


---
<!--
master: section-title
notes: |
        November 1996 - netscape submits JS to Ecma
        June 1997 - EcmaScript 1.0 released
        European Computer Manufacturers Association 
-->

# 1997-1998

---
<!--
master: image
custom:
  1:
    padding-top: 10%
    zoom: 1.2
notes: |
        Ecma-262
        EcmaScript 1 1997
        EcmaScript 2 1998 - 2 was minor alterations to work 
        it into ISO format
        ES 2 implemented in IE 4 and Netscape 4.x
-->

# JavaScript Gets Standardised

![](/images/ecma_logomini.jpg)

---
<!--
master: diagram
custom:
  1:
    margin-top: -15px
notes: |
        Ecma-262
        EcmaScript 1 1997
        EcmaScript 2 1998 - 2 was minor alterations to work it into ISO format
        ES 2 implemented in IE 4 and Netscape 4.x
-->

# JavaScript Gets Standardised

```diagram
graph TD;

1.3[JavaScript 1.3]---|Standardisation|ecma[Ecma-262 1st Ed & 2nd Ed]
ecma---|Implementation|ns[Netscape 4.x]
ecma---|Implementation|ie[Internet Explorer 4.0]

```

---
<!--
master: diagram
custom: 
  1:
    margin-top: -20px
    "#Clearly":
      transform: translateY(118px) translateX(67px) rotate(4deg) scale(0.8)
-->

# One of the two hard things...

```diagram

graph LR;


subgraph Netscape
Mocha --> LiveScript
LiveScript --> JavaScript
JavaScript --> JScript
end

subgraph Standardisation
JavaScript --> EcmaScript
JScript --> EcmaScript
end


subgraph Microsoft
JScript
end

Clearly[Clearly the<br> best name]
style Clearly fill:#FADA5E,stroke:#ccc,stroke-width: 1px

```

---
<!--
master: image
notes: |
        1997-1998
-->

# I "rung up" up a £300 phone bill

![](/images/modem.jpg)

---
<!--
master: image
notes: |
        this and neopets,
        and the worms2 tournament ladder site
-->

# Dialing up for this action:

![](/images/ie4-htmlgoodies.jpg)

---
<!--
master: section-title
-->

# 1998

---
<!--
master: image
custom:
  1:
    margin-top: 20px
-->

# Netscape Open Sources Codebase, Calls it Mozilla

![](/images/mozilla.gif)


---
<!--
master: section-title
notes: |
        I was playing worms2 a lot
        oriented towards visual:
        using delphi (object pascal)
        using flash and actionscript
        played guitar in a band
--> 

# 2000

---
<!--
master: image
custom:
  1:
    margin-top: 90px
notes: | 
        2000
        Added regular expressions, better string handling, new control statements, try/catch exception handling, tighter definition of errors, formatting for numeric output and other enhancements

-->

# IE 5.5 - EcmaScript 3rd Edition


![](/images/ie5.png)


---
<!--
master: section-title
notes: |
        2000
        actually a premature release of the mozilla rebuild, 
        released under pressure to compete with ie, wasn't ready
-->

# Netscape 6
## It isn't good.


---
<!--
master: section-title

-->

# 2001

---
<!--
master: image
custom:
  1:
    margin-top: 90px
notes: |
        ...still ES3, JS innovation is over for now
-->

# IE 6 - EcmaScript 3rd Edition


![](/images/ie6.png)


---
<!--
master: image
custom:
  1:
    margin-top: 45px
    width: 625px
-->

# Netscape Market Share: 9%

![](/images/netscape-usage.svg)


---
<!--
master: section-title
-->

# 2002

---
<!--
master: image
custom:
  1:
    margin-top: 4px
    width: 575px
-->

# This guy...

![](/images/douglas crockford.jpg)

---
<!--
master: image
notes: |
        facilitating the rise of AJAX
        became official standard in 2013 - as ECMA-404
        (v. funny, the standard that should have been...)

        2002
        age 17
        stepped out for a while, no internet
        started to take an interest in linux around age 19ish,
        learnt a lot by reading linux mags, and using an old PC
        with no internet
        interestingly became about as inactive as JS progress
        between 2002 and 2007
-->

# ...launches JSON.org

![](/images/json.org.png)

---
<!--
master: section-title
notes: |
        more like 05-06, started making websites for free,
        used PHP for backend. 

        worked at mcdonalds, then a homeless hostel (make
        slides for this?)
-->

# 2007

---
<!--
master: image-caption
custom:
  1:
    margin-top: 20px
notes: |
        lot of politics and grandstanding
        lot of different opinions and directions
        lots of incompatibilities
        wasn't well thought out
        
        tried to take it more in the classical direction
        not understanding the strengths that came 
        from scheme and self


-->

# EcmaScript 4 Whitepaper

![](/images/es4-whitepaper.png)

It was not well received...

---
<!--
master: section-title
-->

# 2008

---
<!--
master: image
custom:
  1:
    margin-top: 4px
    width: 575px
-->

# This guy...

![](/images/douglas crockford.jpg)

---
<!--
master: image
custom:
  1:
    zoom: 0.38
    margin-top: 19px
    img:
      border: "1px solid #cdcdcd"
-->

# Releases this book

![](/images/good-parts.jpg)


---
<!--
master: image
custom:
  1:
    width: 400px
    margin-top: 15px
notes: |
        v8 is a performance revolution
        JavaScript is a v. dynamic runtime language, 
        a naive implementation is slow, however a bunch 
        of intelligent guys got together and wrote a highly
        optimized implementation, proving that JS can be 
        a useful, grown up, production level language
-->

# Google launch Chrome, and with it the v8 JavaScript engine

![](/images/chrome.png)

---
<!--
master: section-title
-->

# TC39 Moves in new direction: EcmaScript 3.1

---
<!--
master: image
custom:
  1:
    margin-top: 47px
    width: 360px
    position: absolute
  2:
    margin-top: 47px
    width: 406px
    position: absolute
    margin-left: 280px
-->

# These guys were catalysts...

![](/images/brenden eich.jpg)

![](/images/douglas crockford.jpg)

---
<!--
master: section-title
-->

# "ES.next" (ES6) also announced as syntactic extensions specification

---
<!--
master: section-title
-->

# 2009

---
<!--
master: section-title
-->

# EcmaScript 3.1 becomes EcmaScript 5
## Final TC39 Approved Draft Released

---
<!--
master: image
custom:
  1:
    width: 650px
    margin-top: 3px
notes: |
        This added to momentum of JS innovation
        both in the language, and in the applications
        of JS
-->

# Ryan Dahl creates Node.js

![](/images/unofficial-node.png)


---
<!--
master: image
custom:
  1:
    width: 510px
    margin-top: 15px
notes: |
        Significant because it's comparable to performance of v8
-->

# Firefox 3.5 comes with the SpiderMonkey JS engine

![](/images/firefox-3-5.png)

---
<!--
master: image
custom:
  0:
    font-size: 40px
  1:
    margin-top: 30px
    width: 600px
notes: |
        Significant because community interest helps to
        drive innovation, and innovation helps to drive
        community interest
-->

# Chris Williams organises the first JSConf

![](/images/jsconf2009.png)

---
<!--
master: section-title
notes: |
        Chris Williams is a productive guy, runs a flower shop too
-->

# Chris Williams writes node-serialport, triggering...<br><br> The rise of JS Robots


---
<!--
master: section-title
-->

# 2011

---
<!--
master: section-title
notes: |
        Injection of freshness
-->

# EcmaScript 5.1

---
<!--
master: bullets
custom:
  1:
    margin-top: -7px
    li:
      line-height: 23px
-->

# EcmaScript 5

* Strict mode
* Array
  * forEach, map, reduce, filter
* Object
  * keys, create, defineProperties, freeze
* String
  * trim
* Function
  * bind
* JSON



---
<!--
master: section-title
-->

# 2012

---
<!--
master: image
custom:
  0:
    font-size: 41px
  1:
    width: 420px
    margin-top: 30px
notes: |
        As part of community involvement,
        many variants of this logo now exist
        (e.g. JS Robots)
-->

# Chris Williams creates unofficial JS logo

![](/images/js.png)

---
<!--
master: image
custom: 
  0:
    font-size: 45px
  1:
    width: 375px
    margin-top: 15px
notes: |
        Wrote this while working in homeless hostel
-->

# Shameless Plug: A common idiom

![](/images/node-cookbook-1st-ed.jpg)

---
<!--
master: section-title
-->

# 2013

---
<!--
master: image-caption
custom:
  1:
    width: 350px
    margin-top: 20px
    margin-bottom: 10px
-->

# Node reaches 0.8

![](/images/node-logo.png)

Early-adopters in Enterprise <br>begin to use it in production

---
<!--
master: section-title
-->

# 2014

---
<!--
master: image-caption
custom:
  1:
    width: 350px
    margin-top: 20px
    margin-bottom: 10px
-->

# Node reaches 0.10

![](/images/node-logo.png)

Good, stable all round improvements, easy migration

---

<!--
master: image
custom: 
  0:
    line-height: 50px
  1:
    width: 400px
    margin-top: 15px
-->

# Node Cookbook Update

![](/images/node-cookbook-2nd-ed.jpg)


---
<!--
master: image-caption
custom:
  1:
    width: 350px
    margin-top: 20px
    margin-bottom: 10px
notes: |
        fork sees commit explosion, whereas node
        had been faltering for up to a year
-->

# io.js fork

![](/images/io.png)

Developer discontent leads to fork

---
<!--
master: section-title
notes: |
        Let's take a look at the state of JS today

        (certainly not comprehensive, just what I see..)
-->

# 2015

---
<!--
master: diagram
custom:
  1:
    zoom: 0.8
    margin-top: -100px
notes: |
        tessels run time is called t1-runtime
        it's built on lua
        it's also compatible with node api
-->

# JS Overview 

```diagram

graph LR;

tessel(<img src="/images/tessel.png" width=32 height=32>)
espruino(<img src="/images/espruino.png" width=32 height=32>)


chrome[<img src="/images/chrome.png" width=32 height=32>]
chromium[<img src="/images/chromium.png" width=32 height=32>]
node[<img src="/images/node-logo.png" width=32 height=32>]
io[<img src="/images/io.png" width=32 height=34>]
nw[<img src="/images/nw-small.png" width=32 height=34>]
electron[<img src="/images/electron.png" width=32 height=34>]
serial>node-serialport]
bots(<img src="/images/jsrobots.png" width=32 height=32>)
cylon(<img src="/images/cylonjs.png" width=32 height=34>)
nodecopter(<img src="/images/nodecopter.png" width=32 height=32>)
runtime(<img src="/images/runtimejs.png" width=32 height=32>)

tessel --> bots
espruino --> bots
node -.- tessel
io -.- tessel

v8 --> chrome
v8 --> chromium
v8 --> runtime

v8 --> node
node -.-> io
v8 --> io


chromium --> nw
io --> nw
chromium --> electron
io --> electron


io -.-  serial
node -.- serial
serial --> cylon
cylon -.- bots
cylon -.- nodecopter
nodecopter -.- bots

runtime --> bots



```

---
<!--
master: diagram
custom:
  1:
    zoom: 0.65
    margin-top: -100px
notes: |
      jxcore is a node-compatible
      development platform for mobile 
      and embedded apps,

      runtime.js will probably influence 
      this space also

      NativeScript is a much lighter weight,
      more immature alternative

      theres also a ms fork of node based on chakra
      it's temporary.. aprntly
-->

# JS Overview 

```diagram

graph LR;

chakra(chakra)
spidermonkey(spider<br>monkey)


win8(<img src="/images/win8.jpg" width=32 height=32>)
edge(<img src="/images/edge.png" width=32 height=32>)
firefox(<img src="/images/firefox.jpg" width=32 height=32>)
firefoxOS(<img src="/images/firefox-os.png" width=32 height=32>)
asm.js(asm.js)

jxcore(<img src="/images/jxcore.png" width=32 height=32>)

gnome(<img src="/images/gnome.png" width=32 height=32>)
webasm{WebAssembly}
perf{High<br>Performance}



chakra --> edge
chakra --> win8
chakra --> asm.js

edge -.- win8

asm.js -.-> webasm

asm.js --> perf
webasm --> perf

v8((v8)) ---|Optimized For| asm.js

spidermonkey --> jxcore
spidermonkey --> firefox
spidermonkey --> firefoxOS
spidermonkey --> asm.js
spidermonkey -.-> Gjs
Gjs --> gnome

firefox -.- firefoxOS

```

---
<!--
master: image-caption
custom:
  1:
    width: 350px
    margin-top: 20px
    margin-bottom: 10px
notes: |
        2015
        took a lot to get it out of the door
        io.js will now start feeding into next version of node
        for high stability - use 0.10
        for progressiveness use io.js
        not sure if I trust 0.12 (developer drop off etc.),
        might take a while to stabilize, io.js will fix issue

-->

# Node reaches 0.12

![](/images/node-logo.png)

Projects stewards motivated by fork to release<br>
Best to stick with 0.10 while 0.12 matures a little

---
<!--
master: section-title
notes: |
        Next version of node will be iojs + 1,
        e.g. Node 3 (unless theres another release of iojs first)

        Developer efforts will feed into node
-->

# Creation of Node Foundation
## Agreement between io.js and node project to merge


---
<!--
master: section-title
-->

# ES6 renamed to ES2015
## ES7 === ES2016 ... ?

---
<!--
master: section-title
-->

# ES2015 Approved
## June 17th 2015

---
<!--
master: section-title
-->

# Future


---
<!--
master: image
custom:
  1:
    margin-top: 35px
-->

# Soylent

![](/images/soylent.jpg)


---
<!--
master: image
custom:
  1:
    width: 350px
-->

# Future Me

![](/images/future-me.jpg)


---
<!--
master: bullets
-->

# EcmaScript 6

* Lots of implementing to be done yet
* Chrome, Firefox, io.js - latest support
* Transpilers
* let, const (block scoping)
* Promises, Generators
* Classes (sugar), Modules
* Spread, rest, destructuring
* Lambdas, and lots more

---
<!--
master: bullets
-->

# EcmaScript 7 (2016?)

* Async/Await
* Guards
  * Enforcing arbitrary constraints
  * Typing Primitives
* Event loop concurrency
  * Sharing state between event-loops
  * (instead of workers/multiple processes)


---
<!--
master: section-title
-->

# Future future

---
<!--
master: bullets
-->

# EcmaScript 8 (2017?)

* Macros
* SIMD
  * Single instruction, multiple data
  * Parallel array processing

---
<!--
master: image
notes: |
        When we all take wearables too far

        Got some apple watch, google glass, myo armbands,
        brain signal integration, built in soylent delivery system,

-->

# Future Future Me

![](/images/future-future-me.jpg)

---
<!--
master: section-title

-->

# Thank you.

---
<!--
master: section-title

-->

# Thank you.

## @davidmarkclem




