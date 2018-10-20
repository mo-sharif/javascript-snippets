# What is this?

Snippets cheat sheet that I am putting together to help anyone that needs to learn important coding topic or just use it as a refresher ✌️  

enjoy!


# Table of content:

- [JavaScript](/JavaScript/js.md##javascript)
    - [Classes](/JavaScript/js.md###classes)
    - [Promises](/JavaScript/js.md###Promises)
- [Angular](#angular)
    - [Angular CLI](###angular-cli)
    - [Modules](###Modules)
    - [Components](###Components)
    - [Directives](#Directives)
    - [Services](#Services)
    - [Pipes](#Services)
    - [Observables](#Observables)
- [TypeScript](#typescript)

## Angular

- [ ] What is Angular ?
- [ ] Angular CLI ?

## Angular CLI

Angular Command line, helps automate some process like generating and building out app

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

## TypeScript

- [ ] What is typed?