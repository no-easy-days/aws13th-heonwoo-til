## git 활용
> 3가지 영역

|영역|설명|비유|
|----------|---|---|
|Working Directory|실제로 파일을 편집하는 공간|책상 위|
|Staging Area|커밋할 파일을 준비하는 공간|택배 박스|
|Local Repository|현재 저장소|창고|

> git 상태 확인 및 세팅

- git 저장소 만들기
```
git init
```

- git 저장소 상태 확인
```
git status
```

- git 이력 확인하기
```
# 전체 로그 확인
git log
# 한 줄씩 간단히
git log --oneline
# 3줄 출력
git log -3
```

> Staging Area 활용

- git에 파일 올리는 방법
```
# 특정 파일
add {파일명}
# 여러 파일
add {파일명} {파일명}
# 전체 파일
add .
```

- commit에 저장하는 법
```
# 메세지와 함께 커밋
git commit -m "{저장 내용을 알기 쉽게 ex: Add: 로그인}
# 에디터에서 상세 메시지 작성
git commit
# 에디터 없이 메시지 작성
git commit -m '{저장할 메시지}"
```



## 기타 git bash 코드
> 폴더 생성 및 이동

- 폴더 생성
```
mkdir <폴더명>
```
- 폴더 이동
```
cd <폴더 명>
```
- 폴더 나가기
```
cd ..
```
> 파일 생성

- 파일 생성
```
vim <파일 명>
```
1. 파일 작성: i 버튼
2. 저장: esc -> :w 입력
3. 나가기: esc -> :q 입력

## git 브랜치


## git 설치
> 설치 방법 
- Window: git-scm.com에서 설치
- macOS:
1. Homebrew 사용 $$(권장)$$
```
brew install git
```
2. Xcode Command Line Tools
```
xcode-select --install
```
- Linux (Ubuntu/Debian)
```
sudo apt update
sudo apt install git
```
> 설치 확인
```
git --version
```
> 환경 설정
```
git config --global user.name "추헌우"
git config --global user.email "example@gmail.com"
```
- github 이름, 이메일을 일치시키는게 좋음
> 설정 확인
- 개별 설정 확인
```
git config user.name 
git config user.email
```
- 전체 설정 확인
```
git config --list
```
> 설정 범위


|옵션|범위|설정 파일 위치|
|----------|---|---|
|--system|시스템 전체|/etc/gitconfig|
|--global|현재 사용자|~/.gitconfig|
|--local|현재 저장소|.git/config|
