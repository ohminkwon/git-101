# Git-101

깃 사용에 대한 내용 정리입니다.

## Git 초기 설정

- 해당 프로젝트 폴더내의 .git 폴더를 생성하며 버전 관리를 시작합니다.  

```
git init
```
- OS에 따라 개행문자 설정을 합니다.
  - 윈도우 설정  
  ```
  git config --global core.autocrlf true
  ```
  - 맥OS 설정
  ```
  git config --global core.autocrlf input
  ```
◆ Windows 에선 line ending 처리를 CR(Carriage-Return, '\r')과 LF(Line Feed, \n)을 사용하고 Unix 나 Mac OS 는 LF 만 사용하기 때문이다.  

- 해당 버전 관리 사용자를 설정합니다. (추후 변경 가능)
```
git config --global user.name '이름'
git config --global user.email '이메일주소'
```

- Git 설정 확인
```
git config --global --list
```

## Git & GitHub

- 버전 변경 여부, 변경점 등록, 변경내역추가, 기록을 확인합니다.
```
git status
git add .
git commit -m '변경 사항'
git log
```

- 이전 버전으로 되돌리기
```
$ git reset --hard HEAD~1
```

- 이전 버전으로 되돌리기를 취소
```
$ git reset --hard ORIG_HEAD
```

- 깃허브에 업로드
```
git remote add origin 'url'
git push origin master
```

- 깃 브랜치 설정
```
git branch
git branch -a
git branch '브랜치 버전 이름'
git checkout '브랜치 버전 이름'
```
