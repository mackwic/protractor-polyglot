Protractor-polyglot
===================

[Protractor](https://github.com/angular/protractor) is awesome, but only speaks the language spoken by NodeJS. How about making it polyglot ?

Explain further, mon ami !
==========================

Protractor-polyglot wants protractor to speak more languages. *Das klingt gut !*, isn't it ? Let's drive into some details:

Here's the Protractor architecture:

    Your angular Application (in the browser)
         ^
         | Pool of browser maintained by Selenium
         v
    +---------------------------------------+
    'Selenium (java)                        '
    '    ^                                  '
    '    |                                  '
    '    v                                  '
    'Webdriver (add-on of Selenium)         '
    +---------------------------------------+
        ^
        |
        v
    +---------------------------------------+
    ' Protractor (NodeJS app)               '
    '   ^                                   '
    '   |                                   '
    '   v                                   '
    ' Embedded Jasmine driver               '
    '   ^                                   '
    '   |                                   '
    '   v                                   '
    ' Your E2E code                         '
    +---------------------------------------+

Complicated ? Not so much. Not *enough*.
    
