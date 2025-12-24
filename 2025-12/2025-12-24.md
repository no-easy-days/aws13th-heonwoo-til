# [2025-12-24] Git과 GitHub은 너무 어려워

## ☀️ 오늘의 목표 (Scrum)

>첫 날이라서 생략

## 📝 배운 내용 (Today I Learned)

### GIT이란?
> 분산을 통해 충돌을 방지하는 데이터 관리 방식 

> Working directory, Staging area, Repository로 구별함 
- Staging Area가 중요! 중간에 저장하는 공간

### Git활용
> Git을 통해 버전 저장 방법
1. git초기화
```
git init
```
2. 파일 추가
```
add {파일명}
```
3. commit을 통해 저장
```
git commit -m "{저장 내용을 알기 쉽게 ex: Add: 로그인}
```
- commit을 통해 저장한 경우 새로운 버전이 발생한 것
- log를 통해 이전에 저장한 commit 버전을 확인할 수 있고 로드할 수 있음
```
git log
git revert <commit_id>
```
- 주의사항 log가 많은 경우 귀찮아짐 뒤에 숫자 "-3"등을 붙여서 확인할 최소 범위를 지정하면 확인이 편함
- 근데 분산을 통해서 관리하는거라며? 분산이 아닌데? 그래서 등장했다 branch!!!

### branch란?
> main 개발 환경에 영향을 주지 않는 작업 공간

> branch를 만들때는 목적을 정확히 하는 이름으로 작성하는게 좋을 듯!!!

### branch 제작법
> branch 확인
```
git branch
# * main        ← * 표시가 현재 브랜치
#   feature
```
> branch 선언
```
# 새 브랜치 생성 (이동하지 않음)
git branch feature/login
# 생성과 동시에 이동
git switch -c feature/login
```
> branch 삭제
```
# 병합된 브랜치 삭제
git branch -d feature/login
# 강제 삭제 (병합 안 된 브랜치)
git branch -D feature/login
```
### GitHub란?
> Git을 통해 버전 저장을 관리하는 것을 할 수 있다. 그런데 다수의 사람과 협업을 하고 자료를 공유하려면?

> GitHub는 온라인 상에서 데이터를 공유하고 쉽게 접근하여 다수의 수정을 용이하게 함.
- Git과 GitHub의 연동 
1. git remote로 연결할 경로 지정
```
// 좀 더 쉽게 하는 방법이 있었는데 까먹음. 집 가서 차근차근 다시 해볼 예정
git remote add origin [https://사이트]
```
2. push를 통해 사이트에 올리기
```
git push origin main
```
3. pull을 통해 사이트에서 가져오기 
```
git pull origin main
```
- 근데 하나하나 보내고 가져오기 구찮지 않나? 그래서 등장했다! CLI!

### CLI란?
> Git과 GitHub 사이에 연결을 쉽게 해주는 프로그램?

## 🔥 도전 과제 & 해결 (Challenge & Solution)

> 수업 놓지지 않기...

## 💭 오늘의 회고 (Retrospective)

- **Keep (좋았던 점)**: 추상적인 큰 그림은 그릴 수 있었다.
- **Problem (아쉬웠던 점)**: 용어가 생소해서 일부 놓쳤다.
- **Try (시도할 점)**: 주말에 놓친 부분 쫓아가기
