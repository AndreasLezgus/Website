# Personal website of Andreas Lezgus
Portfolio: https://www.lezgus.de

NOTE: This README is also available in <a href=https://github.com/AndreasLezgus/Website/blob/master/README.md>German</a>.

This document is intended for a technical audience and represents the code and components of my website. I'm always happy to hear about improvements and ideas on how to optimize the pages.


## About this project?
This documentation and the program code was created by myself and is used as my personal portfolio website. My old developer heart always tries to understand how something works. Trying, making mistakes, learning and desperately searching for the typo in the code. The blueprint and source code of these pages can be copied, checked, modified and improved by everyone.


## Who am I?
Andreas Lezgus, https://www.lezgus.de/story.html


## What is the goal of this project?
These portfolio pages are usually static and the frequency of changes is manageably low. The idea of the project was therefore to go back to the roots. Simple static HTML and CSS. No scripting language. No database. Publishing on low cost Amazon Web Services S3 storage with simple CI/CD tools for testing, versioning and publishing. Use of a worldwide distributed Content Delivery Network (CDN).
Updating the pages with a simple text editor platform independent from any device. Let's see how far I get with these simple tools?

Interactive content, such as my social media profiles, is merely linked to the respective platform by references. An English or german language version is offered manually via corresponding symbols and is not switched automatically.


## Technical Architecture and processes
My website is hosted on a secure Amazon Web Service S3 storage space. The static HTML pages there are read-only and not publicly accessible. The distribution and publication is done via a worldwide distributed content delivery network with Amazon CloudFront using a HTTPS protocol. The Amazon Lambda@Edge services provide regular updates of the caching mechanismen. 

The publishing and modification processes are done via a git client (I actually use Visual Studio Code https://code.visualstudio.com on the Mac and WorkingCopy https://workingcopyapp.com/ on iOS). Every change to this github repository automatically updates the website on Amazon S3 storage via Amazon CodePipeline and redistributes the pages via Amazon CloudFront.


## Privacy and information security
Information about the privacy policy of my portfolio website can be found here:
http://www.lezgus.de/transparency.html


## Copyrights
In order to provide a simple possibility for open access and the reproduction, editing and distribution of the content and source code I use the license regulations of the non-profit organization <b>Creative Commons</b>. Therefore, the license terms of CC-BY (free redistribution if the author is named) apply to the content created by me on these pages. For further information please see this short <a href='https://creativecommons.org/licenses/by/4.0/deed.en'>summary</a>. As far as the contents on this site were not created by me, the copyrights of third parties are respected. In particular, third-party content is identified as such. If a copyright infringement should nevertheless occur or no correct identification should be made, I ask for an appropriate reference. If I become aware of any infringements, I will remove such contents immediately. Please send a short information to: <a href=mailto:info@lezgus.de>info@lezgus.de</a>.


## Contributions and thanks
This webiste uses the following frameworks, code modules, graphics and symbols.
I would like to thank all authors for their work, publications and support.

Minimalistic CSS framework from milligramm
https://milligram.io/

CSS resets for older browsers from normalize
https://necolas.github.io/normalize.css/

Hamburger menu from Håvard Brynjulfsen
https://codepen.io/havardob/pen/zZvLgw

Vector graphics from freepic.com
https://www.freepik.com/free-photos-vectors/

Icons from fontawesome
https://fontawesome.com/

Fonts from Google fonts (provided from the local website)
https://fonts.google.com/specimen/Open+Sans


---

Many thanks and best regards from Steinfurt, Germany

Andreas Lezgus

info@lezgus.de
