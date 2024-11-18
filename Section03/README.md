# 배열과 객체 성능 평가 

> Understand how objects and arrays work, through the lens of Big O
Explain why adding elements to the beginning of an array is costly
Compare and contrast the runtime for arrays and objects, as well as built-in methods

#### Objects를 사용할 때 
+ **정렬(Order)**이 필요하지 않을 때
+ 빠른 접근, 삽입, 삭제가 필요할 때


|연산|빅오 성능|
|---|------|
|키-값 추가	|O(1)|
|키 제거	|O(1)|
|키에 접근|O(1)|


#### Arrays 사용할 때 
+ **정렬(Order)**이 필요할 때
+ 빠른 접근, 삽입, 삭제가 필요할 때 (부분적으로)

|작업	|빅오 성능|
|------|------|
|삽입 (Insertion)|상황에 따라 다름|
|제거 (Removal)	|상황에 따라 다름|
|탐색 (Searching)|	O(N)|
|접근 (Access)	|O(1)|

#### Array 연산의 Big O

|메서드	|빅오 성능|
|-----|------|
|push	|O(1)|
|pop	|O(1)|
|shift	|O(N)|
|unshift|	O(N)|
|concat	|O(N)|
|slice	|O(N)|
|splice	|O(N) (삽입 및 제거)|
|sort	|O(N*logN)|
|forEach/map/filter/reduce	|O(N)|
