### 아래 함수에 대한 시간 복잡도를 구하세요.

1. 

```js

function logUpTo(n){
    for(var i=1; i <= n ; i++){
        console.log(i); 
    }
}
```

> O(n)


2. 
```js
function logAtMost10(n){
    for(var i=1; i<=Math.min(n, 10); i++){
        console.log(i); 
    }
}
```
> O(1)
> n이 10 이상의 숫자일 때 값은 10(상수)으로 고정됨


3. 
```js
function logAtLeast10(n){
    for(var i=1; i<=Math.max(n, 10); i++){
        console.log(i); 
    }
}
```
>O(n)


4.
```js
function onlyElementsAtEvenIndex(array){
    var newArray = Array(Math.ceil(array.length / 2);) // O(1)
    for(var i = 0; i < array.length ; i++){ // O(n)
        if(i%2===0){
            newArray[i / 2] = array[i];  // O(1)
        }
    }
    return newArray ; 
}
```
> O(n)
> 코드 주석 참고 

5. 
```js
function subtotals(array){ 
    var subtotalArray = Array(array.length);  
    for(var i = 0; i<array.length; i++){
        var subtotal = 0 ;
        for(var j = 0; j <= i ; j++){
            subtotal += array[j]; 
        }
        subtotalArray[i] = subtotal ; 
    }
    return subtotalArray ; 
}
```
>O(n^2) 
> 선형으로 올라가는 그래프.. i에 따라 j도 함께 늘어난다. 

