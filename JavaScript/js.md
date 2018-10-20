
## Javascript

- [ ] What is JavaScript ?

### Classes 

- [ ] JavaScript Class ?

```

class Tesla{

constructor(){


}



}

```


### Map function 

```
const cars = [
  { name:'BMW', id:1 },
  { name:'Tesla', id:2 },
  { name:'Audi', id:3 }
];
```
```
const carNames = cars.map(car => car.name);
console.log(carNames); //["BMW", "Tesla", "Audi"]
```

### Filter

```
const electricCar = carNames.filter(car => car !== "Tesla")
console.log(electricCar)//["BMW", "Audi"]
```

### For in loop

```
let array = [1,2,3];

for ( let i in array){
  
  console.log(array[i]);
  
}
```

### Promises

Callbacks alternatives

```
function delay(ms) {
  return new Promise(resolve => setTimeout( resolve, ms));
}
```

```
delay(3000).then(() => alert('runs after 3 seconds'));
```

### Await/Async

Promises alternative

```
const asyncRequest = async () => {

    const val1 = await promise(val1)
    const val1 = await promise(val1)
    return promise(request1, request2)

}

```