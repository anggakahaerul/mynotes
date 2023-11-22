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