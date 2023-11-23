# mynotes
Study Notes Angular

@Component({
  selector: 'app-root', //selector to show in the index html
  standalone: true,
  imports: [CommonModule, RouterOutlet],
  templateUrl: './app.component.html', //template url (render the content show whatever inside the content)
  styleUrl: './app.component.css' 
})
export class AppComponent { //it is a typescript class
  title = 'hello-world'; //this is just a property
}

one way binding

@Component({})
export class MyComponent {
    message = 'Hello World'
}

data binding 


{{message}}

to show it in our template


GENERATE OUR FIRST COMPONENT.

In our terminal we can run
new split terminal. left for server, right for personal terminal
,command is
example:
ng g component appointment-list

one component list can be placed in another component for example 

we have app component html. but if we want to insert appointment-list component we just have to import the component like

<app-appointment-list></app-appointment-list>

to the component html.

INTRODUCTION TO TYPE SCRIPT

if we have learned c# its an easy way to understand typescript cause its really close.

Typescript syntax

app.component.ts

app.component file name
.ts ext name

class AppComponent {//here we can save our code or etc}

if we want to be able to access this class from the other class we need to add "export"

Export class AppComponent {//here we can save our code or etc}


class AppComponent {
title = 'app'; 
items: string []= [
}

- Method
log (text:string):void{
var message = "Message" + text;
}
- Private Method
private log (text:string):void {
var message = "Message" + text;
}


another example
private log (text:string) {
sum (a: number, b: number){
return a+b;
}
}

CREATE AN INTERFACE
npm run ng generate interface folder/filename


ONE WAY DATA BINDING
when the user want to bind the value from particular html component {{data}}

TWO WAY DATA BINDING
when the user want to bind the value from particular HTML input field, so the value will be extracted when the input is changed.

Lifecycle Hooks
ngOnInit()
to load any data from local storage.

export class AppointmentListComponent implements OnInit {
  ngOnInit(): void {
    let savedAppointments = localStorage.getItem("appointments"); 
    this.appointments = savedAppointments ? JSON.parse(savedAppointments) : [];
    // if have value lets load it but if empty just use empty array
  }
}

the user should implements it from OnInit import.

The Most commonly used commands in angular
to create new project
ng new projectName

to run applications
ng serve

ng serve --open

ng serve -o
Same as ng serve, but also opens your default web browser to the application.

ng generate component componentName
or
ng g c componentName

Generates a new component with the specified name.


ng generate service serviceName
or
ng g s serviceName

Generates a new service with the specified name.
ng build

Builds your application for production, creating a dist/ folder with the output.
ng update

Checks your application for outdated dependencies, and can also update them.
Remember, these commands should be run in a terminal or command prompt from within your Angular project's root directory.
I hope you find this cheat sheet helpful as you navigate your Angular journey.
Happy coding!

FUNGSI DARI
Component
Service
Modul

Jannick & TutorialsEU



