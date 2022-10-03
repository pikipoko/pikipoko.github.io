---
title: "W02_4_TIL"
date: 03/10/2022
categories: SWJG TIL
---

### TP
- 푼 문제를 정리해서 남한테 설명할 수 있어야 함.
- 문제 풀이가 아니라, 문제를 보고 어떻게 접근할 것인지
- 물 많이 마시기

### eval(expression) 함수

매개변수로 받은 expression(=식)을 문자열로 받아서, 실행하는 함수.
<hr/>

| expression | 하나 이상의 값으로 표현 될 수 있는 코드. |
| ---------- | -------------------------------------- |



### heap 정렬
heap : 완전 이진 트리         

    원소 a[i]에서
        부모 : a[(i-1)//2]
        왼쪽 자식 : a[i*2 + 1]
        오른쪽 자식 : a[i*2 + 2]

                부모 - a[i]
    왼쪽 자식 - a[i*2 + 1]      오른쪽 자식 - a[i*2 + 2]

<hr/>

    1. 힙에서 최댓값인 루트를 꺼낸다.
    2. 루트 이외의 부분을 힙으로 만든다.
    
    1, 2번을 반복하여 정렬한다.

### heapq 모듈

    Heap queue algorithm (a.k.a. priority queue).

    Heaps are arrays for which a[k] <= a[2*k+1] and a[k] <= a[2*k+2] for all k, counting elements from 0. For the sake of comparison, non-existing elements are considered to be infinite. The interesting property of a heap is that a[0] is always its smallest element.

    Our API differs from textbook heap algorithms as follows:

    We use 0-based indexing. 
    This makes the relationship between the index for a node and the indexes for its children slightly less obvious, but is more suitable since Python uses 0-based indexing.

    Our heappop() method returns the smallest item, not the largest.

    These two make it possible to view the heap as a regular Python list
    without surprises: heap[0] is the smallest item, and heap.sort() maintains the heap invariant!
<hr/>

| ------------------------- | ------------------------------------------------------------------------- |
| heap = []                 | creates an empty heap                                                     |
| heappush(heap, item)      | pushes a new item on the heap item                                        |
| heappop(heap)             | pops the smallest item from the heap item                                 |
| heap[0]                   | smallest item on the heap without popping it                              |
| heapify(x)                | transforms list into a heap, in-place, in linear time item                |
| heaprelace(heap, item)    | pops and returns smallest item, and adds new item; heap size unchanged    |

### 참고 링크

[expression 참고 링크](https://www.hackerearth.com/practice/python/working-with-data/expressions/tutorial/)