
 # Angular Interview Questions & Answers.





### Table of Contents

| No. | Questions |
|-----| --------
|1  | [What is Angular ?](#What-is-angular?)|
|2  | [What are the key features of Angular ?](#What-are-the-key-features-of-angular?)|
|3  | [Command for Create new project , component ,service ?](#command-for-create-project-component-service?)|
|4  | [Explain two-way data binding in Angular ?](#explain-two-way-data-binding-in-angular?)|
|5  | [What is dependancy Injection in Angular?](#what-is-dependancy-injection-in-angular?)|
|6  | [Explain Angular modules](#explain-angular-modules)|
|7  | [What is an Angular directive?](#what-is-an-angular-directive?)|
|8  | [What is Angular component?](#what-is-angular-component?)|
|9  | [What are the key components of Angular?](#what-are-the-key-component-of-angular?)|





































1. ### What is angular?
 Angular is a popular open-source web application framework developed by Google.
 It is used for building dynamic and single-page web applications (SPAs) with enhanced user experiences.

2. ### What are the key features of Angular?
 key features of Angular include two-way data binding, dependency injection,
 modularity, templates ,directives, components, and a poweful CLI for scaffolding and 
 managing

3. ### Command for Create new project, component ,service?
  
   1. Create a New Angular Project 
        ```javascript
        ng new -your-project-name

        ```
   2. Create a New component 
      ```javascript
      ng generate component component-name
      ```
   3. Create new Service
      ```javascript
       ng generate service service-name
      ```
4. ### Explain two-way data binding in Angular?
  Two-way data binding in Angular means that any changes in the UI (User Interface) automatically update the application objects and vice versa.It simpllifies the synchronization between the model and view, providing a seamless user experience.

5. ### What is dependancy Injection in Angular?
  Dependency injection is a desgin pattern used in Angular to achive loosly
  coupled component and manage dependencies.It allows the componenet to recive the required dependencies from an external source,making the application more modular, maintainable and testable.

6. ### Explain Angular modules.
  Angular modules are containers for organizing and grouping reated components,
  directives,ppipe,and services. They help keep th application modular and maintainable by providing a way to organize the application into cohesive and reusable blocks.

7. ### What is an Angular directive?
   An Angular component is a reusable HTML element or attributes that adds behavior to the DOM.It can modify the structure,behavior,and appearance of the DOM elements.

    Directives add behaviour to an existing DOM element or an existing component instance.

    ```javascript
    import {Directive,ElementRef,Input} from '@angular/core';

    @Directive({selector:'[highLight]'});
    export class HighlightDirective{
        constructor(el:ElementRef){
            el.nativeElement.style.color = 'red'
        }
    }
    ```

8. ### What is Angular component?
  An Angular component is a building block of an application that encapsulates the logic, data,and user interface element.Component are reuseable,maintainable, and xcan be composed to form complex UIs.
   These component are a subset of directive,unllike directives,components always have a template and only one component can be instantiated per element in a template.
   Example:-
    ```javascript
    import {component} from '@angular/core';

    @component({
        selector:'my-app',
        template:`<div>
        <h2> {{title}}</h2>
        <p>Angular Interview Questions And Answer </p>
        </div>
        `
    })

    export class AppComponent {
        title:string = 'Welcome to Angular world';
    }
    ```

9. ### What are the key components of Angular?
    1. Component: These are the basic buiding blocks of an Angular application to control HTML views.
    2. modules: An Angular module is a set of angular basic building blocks like components,directive,services etc. An application is divided into logical pieces and each piece of code is called "module" which perform a single task.
    3. Template :These represent the views of an Angular application.
    4. Services:Are used to create components which can be shared across the entire application.
    5. Metadata: this can be used to add more data to an Angular class.


