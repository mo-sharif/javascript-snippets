

## Map function 

```
const smartPhones = [
  { name:'iphone', price:649 },
  { name:'Galaxy S6', price:576 },
  { name:'Galaxy Note 5', price:489 }
];

```
const prices = smartPhones.map(smartPhone => smartPhone.price);
console.log(prices);


//Making a promise

function delay(ms) {
  return new Promise(resolve => setTimeout( resolve, ms));
}

delay(3000).then(() => alert('runs after 3 seconds'));


//For in loop

let array = [1,2,3];

for ( let i in array){
  
  console.log(array[i]);
  
}



//


// Angular loops
console.log(`*ngIf="(users$ | async).length"
*ngFor="(let user of users$ | async)"`);



//observables

//pipe

//subscribe

