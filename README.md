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
when the user want to bind the value from partucular HTML input, so the value will be extracted when the input is changed.


