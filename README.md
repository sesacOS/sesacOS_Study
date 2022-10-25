# 새싹 OS 스터디 방입니다.

<br>

## 상황: 공동작업 할 때 (※ $는 터미널이라는 의미입니다.)

### 깃 명령어

#### 깃허브 저장소를 내 컴퓨터에 가져오기

```
$ git clone (주소)
```

#### 저장소 확인하는 법

```
$ git remote -v
```

#### 브랜치 확인하는 법

```
$ git branch -v
```

#### 브랜치 바꾸는 법

```
$ git checkout (브랜치이름)
```

#### 저장소를 생성하는 법

```
$ git remote add (저장소 이름) (git 주소)
```

#### 원격 저장소에서 파일 내려받기

```
$ git pull origin(저장소) main(브랜치)
```

#### 깃 현재 상태 보기

```
$ git status
```

#### 깃 파일 스테이지에 등록하기

```
$ git add (파일명)
```

#### 깃 스테이지 상태 보기

```
$ git status
```

#### 깃 커밋하기

```
$ git commit -m (커밋명)
```

#### 깃 푸쉬하기 (main 브랜치에 푸쉬)

```
$ git push origin(저장소) main(브랜치)
```

#### 깃 푸쉬하기 (나의 브랜치에 푸쉬)

```
$ git push origin(저장소) seonghyeon(내 브랜치)
```

<br>

### 참고사항

1. main 권한을 가진 사람이 나의 브랜치에 올린 내용을 pull request로 승인하기를 하면,
   main 브랜치에 내용이 합쳐진다.

2. 같이 작업하는 파일이 있다면 무조건 push 말고 pull 먼저 해야한다!!

<br>
<hr>
<br>
### 터미널 명령어

#### 파일 목록 보기

```
$ ls
```

#### 폴더 이동하기

```
$ cd 폴더이름
```

#### 폴더 뒤로 이동하기

```
$ cd ..
```

#### 현재 폴더 위치 보기

```
$ pwd
```

#### 폴더 생성하기

```
$ mkdir (폴더명)
```

#### 파일 생성하기

```
$ touch (파일명)
```

<hr>

### 오류사항 해결방법

1. git push를 하니까 git pull해라는 오류가 뜬다?
   자격증명 삭제 후 깃허브 재연결하기
   https://stackoverflow.com/questions/37813568/git-remote-repository-not-found

2. The requested URL returned error: 403 오류가 뜬다?
   깃 토큰 새로 발급받기 & 자격증명에 추가하기
   https://ohrora-developer.tistory.com/m/16
