---
layout: post
---
<img src="/images/fulls/02.jpg" class="fit image">
<h2>Modularizing in Angular</h2>

You’ve built out all of your models, correctly placed your “ng-app" statement in either the body or the html tag. You’ve created separate pages for your controllers and your views. When you go to put it all together you cross your fingers and hope that all of your meticulous work falls together perfectly. Unfortunately for many of us we can easily run into complications. I’ve ran into this problem myself and have decided to share with you my check list for troubleshooting connections when modularizing a Angular app:

<strong>Step One:</strong> Makes sure all of you corresponding JS files are loaded as scripts in the index html.

<strong>Step two:</strong> Your “ng-app" statement defines that name of the application. This should be placed at the top of your JS file when defining your Angular Model. If you are modularizing you files into separate pages the instantiation of your application should occur in your config file. This file sets the routes for your application and serves as the first page Angular should look to for further information.

<strong>Step three:</strong> Add all of the additional files that you have created as separate pages into the dependencies array of the instantiation model, or of the config file. These should be the names of the corresponding modules, not the names of the controllers or factories/services.

If you have insured that all three of these step are complete and you are still having trouble its very likely that one or more of your files are failing for various other reasons. One way to troubleshoot this is to add each file one by one and determine which is the failing file.

Angular does not provide the most clear error messages. Many people have trouble when trying to debug. There is an angular debugger add-on available in the chrome store. I have attached a link to that debugger for your convenience.

<a href="https://chrome.google.com/webstore/detail/angularjs-batarang/ighdmehidhipcmcojjgiloacoafjmpfk?hl=en">Angular Debugger</a>

good luck in your adventures with Angularjs.
