<H1>Angular Interview Quick Book<H1>

#### 1. [What is Angular?](#1-what-is-angular)
#### 2. [Why Angular?](#2-why-angular)
#### 3. [Explain Angular component/directive lifecycle hooks?](#3-explain-angular-componentdirective-lifecycle-hooks)

#### 1. [What is Angular?]
Angular is an app-design framework and development platform for creating efficient and sophisticated single-page apps.

#### 2. [Why Angular?]
Angular is an open-source front-end framework developed by Google for creating dynamic, modern web apps. First introduced in 2009, the framework has gained huge traction over the years for eliminating unnecessary code and ensuring lighter & faster apps.

Having rapidly evolved from AngularJS in 2010 to Angular 5 in 2017, the front-end framework is today used by more than 44.3% of software engineers for creating user interfaces (Stack Overflow Developer Survey 2017).
#### Some of the key points are 
- Easy Testing & Simplified Unit Testing
- Modular Structure
- Code Consistency
- Reusability
- Ease of maintainance & Improved readability

#### 3. Explain Angular component/directive lifecycle hooks?
- Directive and component instances have a lifecycle as Angular creates, updates, and destroys them. 
- Developers can tap into key moments in that lifecycle by implementing one or more of the lifecycle hook interfaces in the Angular core library.
- Each interface has a single hook method whose name is the interface name prefixed with ng. For example, the OnInit interface has a hook method named ngOnInit() that Angular calls shortly after creating the component:

#### NOTE: No directive or component will implement all of the lifecycle hooks. Angular only calls a directive/component hook method if it is defined.
