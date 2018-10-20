# Table of content:

- [JavaScript](/JavaScript/js.md#javascript)
    - [Classes](/JavaScript/js.md#classes)
    - [Promises](/JavaScript/js.md#Promises)
- [Angular](/Angular/angular.md#angular)
    - [Angular CLI](/Angular/angular.md#angular-cli)
    - [Modules](/Angular/angular.md#Modules)
    - [Components](/Angular/angular.md#Components)
    - [Directives](/Angular/angular.md#Directives)
    - [Services](/Angular/angular.md#Services)
    - [Pipes](/Angular/angular.md#Services)
    - [Observables](/Angular/angular.md#Observables)
- [TypeScript](/TypeScript/ts.md#typescript)

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