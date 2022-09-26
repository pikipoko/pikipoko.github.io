---
title: "W01_WIL"
date: 02/10/2022
categories: SWJG WIL Big-Oh
---

문제를 30분동안 풀어본다음 > 해당 파트를 책으로 읽고 > 30분동안 다시 풀어보기.

## python
### list
|함수|시간 복잡도|
|---|---|
len() | O(1)
append()|O(1)
insert() | O(N)
element in list | O(N)

### 문자열
|||
|---|---|
sorted()|O(nlogn)

### 
|||
|---|---|
|enumerate()||


### for 문



### [list comprehension](https://shoark7.github.io/programming/python/about-list-comprehension-python)
    [(변수를 활용한 값) for (사용할 변수 이름) in (순회할 수 있는 값)]

    arr = [i*2 for i in range(10)]
    arr = [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]

### 완전 탐색
가능한 모든 경우의 수를 다 체크해서 정답을 찾는 방법    
무식하게 한다는 의미로 "Brute Force"라고 부르기도 하며, 직관적이어서 이해하기 쉽고 문제의 정확한 결과값을 얻어낼 수 있는 가장 확실하며 기초적인 방법이다.

|||
|---|---|
git branch --set-upstream-to origin/main|깃 홈페이지랑 로컬에서 만든 브랜치랑 연결 명령어


--------------------------
사장
1. 깃헙 페이지에서 리포지토리 생성 (main)
2. ex) vs code로 app.py 작업파일생성 푸쉬해서 리포지토리에 업로드 까지완료

---
신입
1. 사장의 리포지토리안에 내용을 복사
git clone (사장 url)
2. 신입의 브랜치생성 
3. 사장 파일을 수정 작성 
4. 업데이트를 하는데 master에 하면 좆댐 / 신입의 브랜치에 업로드 
5. 신입 깃헙페이지에 가면 풀 리퀘스트 도착
6. 확인 후 편지써서 사장한테 보고

------
사장
1. 신입의 풀 리퀘스트 도착
2. 코드 확인 (오류나 수정사장 코드 다보임)
3. 이상없으면 승낙
4. master 즉 우리 회사의 완성품이 수정 완료됨

-----

if 사장이 master 완성품에 변화가 생겼는데 그 도중 코드 수정을 하고 있었다면!

1. git add (해당파일)
2. git commit -m "comment"
3. ****** 절대 푸쉬 하면 안됨
4. master 완성품의 pull 먼저 >> 사장이 수정중이던 코드에 완성품 코드가 복사대체가 아닌 추가가 됨
5. 이후에 사장이 코드 수정 및 완료하면 push
---------------------------------------------------------------------


1. 깃 ~ 프로그램 연결
코드복제
git clone https://github.com/Gi-Youn-Oh/project1.git

2. 폴더이동 명령어
cd project1 ( 깃허브 리포지터리 이름)
cd .. 상위폴더 이동
cd ~ home 폴더

3. 코드 가져오기 (새로운 협업자가 클론 후 코드 받을때 / 보통자동으로 가져와짐)
code .

4. 파일 추가 명령어
git add . (전체)
git add index.html (index.html 만 전송)

5. 커밋하기
git commit -m "first commit"

6. 푸쉬하기
git push origin 브랜치명 / * master는 완성품

7. 브랜치 생성
git checkout -b (브랜치명)

8. 브랜치로 이동
git checkout (브랜치명)

9. 풀 하기
git pull origin master

10. 상태확인
ls (list directory contents)
git status

11. 리포지 토리 생성 후 첫 연결 ***
git init
==========
기타 개인
우선 git 클론을 통해서 연결
해당 파일을 업로드 하고자하는 폴더가 있는 곳으로 이동
change directory  / cd 폴더이름= 해당폴더로 이동 / cd .. 상위폴더이동 / cd~ 홈폴더로 이동

git add 파일명  > 파일 업로드
git commit -m(message) " 커밋 참고 이름 "
git push origin master > 전송