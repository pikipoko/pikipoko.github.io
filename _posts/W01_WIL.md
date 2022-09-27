---
title: "W01_WIL"
date: 02/10/2022
categories: SWJG WIL Big-Oh
---
## 다짐
이론 > 문제 > 답지 > 문제       
문제를 30분동안 풀어본 다음 > 해당 파트를 책으로 읽고 > 30분동안 다시 풀어보기.

## python Big O
|함수|시간 복잡도|
|---|---|
len() | O(1)
append()|O(1)
insert() | O(N)
element in list | O(N)
sorted()|O(nlogn)
|enumerate()||

### [list comprehension](https://shoark7.github.io/programming/python/about-list-comprehension-python)
    [(변수를 활용한 값) for (사용할 변수 이름) in (순회할 수 있는 값)]

    arr = [i*2 for i in range(10)]
    arr = [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]

### 완전 탐색
가능한 모든 경우의 수를 다 체크해서 정답을 찾는 방법    
무식하게 한다는 의미로 "Brute Force"라고 부르기도 하며, 직관적이어서 이해하기 쉽고 문제의 정확한 결과값을 얻어낼 수 있는 가장 확실하며 기초적인 방법이다.       
완전탐색 문제는 완전탐색으로 풀어야 한다.


###  자료구조, 알고리즘 - 책 공부

#### 01-1 알고리즘이란?

|정리||
|---|---|
순차 구조 - sequential structure|한 문장씩 순서대로 처리되는 구조
선택 구조 - select structure|조건식으로 평가한 결과에 따라 프로그램의 실행 흐름이 변경되는 구조
결정 트리 - decision tree| 의사결정 과정과 연관된 이진 트리를 말하는 것으로, 내부 노드는 질문(예/아니오로 답할 수 있는), 외부 노드는 결정을 저장한다. (전공책 p.129)
pass|'아무것도 수행하지 말고 지나치세요'를 뜻하는 키워드. 반복문에서 사용 시 다음 행동으로 간다.
continue|
피연산자 - operand|연산 대상 ex) a>b --> a,b:피연산자/ >:연산자
a if b else c|b가 참이면 a, 거짓이면 c
a = x if x>y else y|x가 y보다 크면 x, 작거나 같으면 y를 a에 할당하겠다.
while|사전 판단 반복 구조
for|변수가 하나만 있을 때는 while문보다 for문을 사용하는 게 좋다. 코드가 직관적으로 짜이기 때문에.
이터러블 - iterable|반복할 수 있는 객체 - list, tuple, str
리터럴 - literal|데이터 그 자체, 메모리 위치안의 값
상수 - constant|변하지 않는 변수. 즉 값이면 다 넣을 수 있음.
집합 - set



값의 비교를 이미 마친 상태에서 다시 비교하는 것은 효율적이지 않다.      

    ex)
        if b >= a ...
        ...
        elif a > b ...

### expression과 statement [expression, statement 참고 링크1](https://shoark7.github.io/programming/knowledge/expression-vs-statement) [expression, statement 참고 링크2](https://gusdnd852.tistory.com/68)

#### expression
expression은 수식, 식, 표현식 등으로 불린다. expression은 하나 이상의 값으로 표현될 수 있는 코드를 말한다. expression은 평가가 가능해서 하나의 값으로 환원이 된다. 그 자체가 어떠한 값을 내포하고 있으면 그것은 식으로 불릴 수 있다.      
즉, 변수도 그 자체로 expression이라고 볼 수 있다.     
([변수-위 정의 파트](http://www.tcpschool.com/c/c_datatype_variable) - 데이터를 저장하기 위해 프로그램에 의해 이름을 할당받은 메모리 공간)        
expression들은 함수의 매개변수로 사용될 수 있고, 함수의 반환값으로도 사용될 수 있다.

---

#### statement
statement는 진술, 서술의 의미로 프로그래밍에서는 실행가능한(executable) 최소의 독립적인 코드 조각을 말한다. 우리가 프로그래밍하면서 컴파일러가 이해하고 실행할 수 있는 구문은 모두 statement라고 보면 된다. 문법적으로 해당 언어에 적합한 모든 코드 한 줄이나 블록은 statement라고 할 수 있다. statement는 흔히 한 개 이상의 expression과 프로그래밍 키워드를 포함하는 경우가 많다. 때로는 expression이 statement가 될 수 있다.     
* 따라서, expression은 statement에 포함된다고 볼 수 있다.       
변수에 할당하는 할당문은 expression처럼 평가되어 하나의 값을 반환하지 않는다.(대부분의 프로그래밍 언어에서)         

#### 정리
expression은 함수의 매개변수로 활용될 수 있지만, statement는 활용될 수 없다.        
변수는 expression으로 볼 수 있다.           
언어마다 expression과 statement가 좀 다르게 적용된다.