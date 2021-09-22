# Git-101

깃 사용에 대한 내용 정리입니다.

## Git 초기 설정

- 해당 프로젝트 폴더내의 .git 폴더를 생성하며 버전 관리를 시작합니다.  

```
git init
```
- OS별 개행 문자 설정
  - 윈도우 설정  
  ```
  git config --global core.autocrlf true
  ```
  - 맥OS 설정
  ```
  git config --global core.autocrlf input
  ```
◆ Windows 에선 line ending 처리를 CR(Carriage-Return, '\r')과 LF(Line Feed, \n)을 사용하고 Unix 나 Mac OS 는 LF 만 사용하기 때문이다.  

- 사용자 설정
```
git config --global user.name '이름'
git config --global user.email '이메일주소'
```

- Git 설정 확인
```
git config --global --list
```

```
git status
git add .
git commit -m 'Study Markdown'
git log
git remote add origin 'url'
git push origin master

```
