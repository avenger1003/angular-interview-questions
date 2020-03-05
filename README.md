<H1>Angular Interview Quick Book<H1>

#### 1. [What is Angular?](#1-what-is-angular-1)
#### 2. [Why Angular?](#2-why-angular-1)
#### 3. [Explain Angular component/directive lifecycle hooks?](#3-explain-angular-componentdirective-lifecycle-hooks-1)
#### 4. [What is Observable?](#4-what-is-observable-1)
#### 5. [What are the advantages of Observable?](#5-what-are-the-advantages-of-observable-1)
#### 6. [Observable Lifecycle](#6-observale-lifecycle-1)

#### 1. What is Angular?
Angular is an app-design framework and development platform for creating efficient and sophisticated single-page apps.

#### 2. Why Angular?
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

#### Lifecycle sequence
##### 1. ngOnChanges()
Respond when Angular (re)sets data-bound input properties. The method receives a SimpleChanges object of current and previous property values.
Called before ngOnInit() and whenever one or more data-bound input properties change.

##### 2. ngOnInit()
Initialize the directive/component after Angular first displays the data-bound properties and sets the directive/component's input properties.
Called once, after the first ngOnChanges().

##### 3. ngDoCheck()
Detect and act upon changes that Angular can't or won't detect on its own.
Called during every change detection run, immediately after ngOnChanges() and ngOnInit().

##### 4. ngAfterContentInit()
Respond after Angular projects external content into the component's view / the view that a directive is in.
Called once after the first ngDoCheck().

##### 5. ngAfterContentChecked()
Respond after Angular checks the content projected into the directive/component.
Called after the ngAfterContentInit() and every subsequent ngDoCheck().

##### 6. ngAfterViewInit()
Respond after Angular initializes the component's views and child views / the view that a directive is in.
Called once after the first ngAfterContentChecked().

##### 7. ngAfterViewChecked()
Respond after Angular checks the component's views and child views / the view that a directive is in.
Called after the ngAfterViewInit() and every subsequent ngAfterContentChecked().

##### 8. ngOnDestroy()
Cleanup just before Angular destroys the directive/component. Unsubscribe Observables and detach event handlers to avoid memory leaks.
Called just before Angular destroys the directive/component.

### 4. What is Observable?
An Observable is a function that can return a stream of values to an observer over time, this can either be synchronously or asynchronously. The data values returned can go from zero to an infinite range of values.

### 5. What are the advantages of Observable?
- Emitting multiple values asynchronously is very easily handled with Observables
- Error handlers can also easily be done inside Observables rather than a construct like promises
- Observables are considered lazy, so in case of no subscription there will be no emission of data values
- Observables can be resolved multiple times as opposed to functions or even promises

### 6. Observable Lifecyle!
There are 4 stages, with some help from observers and subscriptions the Observable instance passes through these four stages throughout its lifetime:
- Creation
- Subscription
- Execution
- Destruction
