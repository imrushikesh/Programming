# Angular Topics
npm install - g@angular/cli
ng version
ng new <application name>
1. Introduction ---
    - Developers	Google
   -  Initial release -->	2.0 / 14 September 2016
   -  Current release --	> 14.1.0   20 July 2022
   -  Written in	TypeScript
   -  Documentation - 	angular.io
   -   SPAs Mostly, scaleble web applications
   -   component based.
   -   code consistency and easy testing
   -   Module for everything - forms, routing,animation, state management- not much need for 
   3rd party packages/modules.
---

2.   file structure ---

```main.ts -- start point
APP.MODULE.TS -->  bootstrap: [AppComponent]
APP.COMPONENT.TS -->  selector: 'app-root',
INDEX.HTML -- >  <app-root></app-root>
selctor match render the app.compoment.html code.
```
### note --> 
    bootstrap array --only for root module, entry point.

---

3. compoments ---
     - ng generate component name
    -  UI building block
     - html, css, ts and specs.ts file.
    - @NgModule--decorator tell angular what is role of class that perticular class - metadata of class. properties of class
    - "selector" - id/class
    - "template "- direct html
    - template url- path to html page
    - style - direct css
    - styleurls- path to stylesheet 
---
4.  bindings

-  interpolation -- expresssions into text--
    - variable into text.
    - <p>{{variable}}</p>

- event  one way binding --  actions on browser - user/custom event
    - (click)='OnSave()'
    - (target event name) = 'template statement()''

- two way binding --  listen events and update values  between parent and child 
Component

    - <input type="text" [(ngModel)]="variable"/> 

----------

5.  Directives 

    - add additional behaviours to angular application
    - we can use built in directives to manage forms, styles.

    - basic : 
      - NgClass
      - NgStyle
      - NgModel

- structural directive (imp)
    - *NgIf ="condition"
    - *NgFor ="let variable of list; let i=index"  
    - *NgSwitch

-----
6. pipes 
    -  ng generate pipe name
    - function transform  values, nostly display purpose. - titlecase,currency,date
    - use througout application anywhere in template

----
7. style  
    - angular,json - styles[] bootstrap link
    - style.css- global
    - component.css- only for component level
    -  note- dont use inline css. hard to maintain
-----

8. parent to child data-- vice versa
use -
@Input () 

child to parent--
Use @Output  and EventEmitter

-------------------------------------------------------------------------------------------

9. LifeCycle Hooks-->
    -  Mostly used - 
ngOnChange()
ngOnInit()
NgOnDistory()


    -  Note --> 
first contructor runs then OnInit
class initiate constructor then compoment is mounted on dom then ngOnInt called

-------
10. Service 
    - ng generate service name
    - local/global
    - class with well defined purpose.
    - services can depends on another servvices.
    - @injectable for services -providedIn: 'root'
    - initalize object in contructor when want to use service.

----
11. routing
    - appModule-- import appRoutingModule
    - routes[]; -- path in array for urls
    - routerlink in html.
----


12. Forms
    - template - FormsModule
    - reactive -  include  ReactiveFormsModule
    - use reactive better control and structure.


















































































































































