
## Angular

- [ ] What is Angular ?
- [ ] Angular CLI ?

## Angular CLI

Angular Command line, helps automate some process like generating and building out app

### Routes
Sample routes snippet
```
const routes: Routes = [
  { path: '', loadChildren: './tabs/tabs.module#TabsPageModule' },
  { path: '**', loadChildren: './tabs/tabs.module#TabsPageModule' }

];
```
### Modules

### Components

### Directives

### Built Directives

```
*ngIf="(users$ | async).length"
*ngFor="(let user of users$ | async)"

```
### Services

- [ ] What are services used for?
 
### Pipes

- [ ] Async pipes
- [ ] Subscribe to an Observable
  
### Observables
- [ ] What is Observables
- [ ] Create Observable

Import Observable and HttpClient

```
import { Observable } from 'rxjs';
import { HttpClient } from '@angular/common/http';

```
Get http API resources

```
public posts$ :Observable<any>

constructor(public http:HttpClient){}

ngOnInit() {

    this.posts$ = this.getPosts();

}

getPosts(): Observable<any[]> {

    return this.get.http<any[]>('ENTER_API_URI', {
        params: {
          per_page: '12'
        }
      });
}


```


```
Subscribe to Pipe

```
```