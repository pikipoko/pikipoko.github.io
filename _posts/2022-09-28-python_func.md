---
title: "파이썬 내장함수"
date: 28/09/2022
categories: python function
---
- [리스트 sort()](#리스트-sort)

- [문자열 strip()](#문자열-strip)

### 리스트 sort()
    sort(*, key: None = ..., reverse: bool = ...) -> None
    sort(*, key: (str) -> SupportsRichComparison, reverse: bool = ...) -> None
        Sort the list in ascending order and return None.
        The sort is in-place (i.e. the list itself is modified) and stable (i.e. the order of two equal elements is maintained).
        If a key function is given, apply it once to each list item and sort them, ascending or descending, according to their function values.
        The reverse flag can be set to sort in descending order.
    key는 함수명.
    key가 매개변수로 주어지지 않으면

    문자열은 알파벳 오름차순 정렬
    정수는 크기 오름차순 정렬

    key가 주어지면
    각 리스트 요소를, key를 적용한 결과값으로 오름차순 정렬

### 문자열 strip()
    strip: (__chars: str | None = ..., /) -> str
        Return a copy of the string with leading and trailing whitespace removed.
        If chars is given and not None, remove characters in chars instead.
    문자열의 양쪽 공백을 없애준다.

### 키보드 stdout.write()
    