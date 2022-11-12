GitHub과 같은 Git 원격 저장소가 무엇인지,

그리고 개발자들이 협업에 일반 클라우드 서비스 대신
이들을 사용하는 이유가 무엇인지 알아봅니다.

📖 Lesson 2. **GitHub** 시작하기

1. github.com 살펴보기\!

- Git으로 관리되는 프로젝트의 원격 저장소

https://techrecipe.co.kr/wp-content/uploads/2021/06/210630_GitHub-Copilot-_001.png

📝 협업에 필요한 인원 추가

GitHub에 새 Repository 생성

**Public**: 모두에게 보일 수 있는 프로젝트
**Private**: 허용된 인원만 볼 수 있는 프로젝트
협업할 팀원 추가

레포지토리의 Settings - Collaborators

![](https://velog.velcdn.com/images/anstmdgus473/post/76ccd3f1-d19f-48d5-bf62-23e09396deaa/image.png)

📖 Lesson 3. **원격 저장소!**

📖1. 로컬에 원격 저장소 추가 후 푸시

⭐️ 이번 강에서는 HTTPS 프로토콜 사용

![](https://velog.velcdn.com/images/anstmdgus473/post/62d15fb8-b054-4124-9bb9-0ed159efd533/image.png)

GitHub 레포지토리 생성 후 복붙 명령어

```
git remote add origin (원격 저장소 주소)
```

- 로컬의 Git 저장소에 원격 저장소로의 연결 추가
  - 원격 저장소 이름에 흔히 origin 사용. 다른 것으로 수정 가능
  ````
  git branch -M main```
  코드를 입력하세요
  ````

```

```

GitHub 권장 - 기본 브랜치명을 main으로

```
git push -u origin main
```

로컬 저장소의 커밋 내역들 원격으로 push(업로드)

-u 또는 --set-upstream : 현재 브랜치와 명시된 원격 브랜치 기본 연결

⭐️ GitHub의 해당 레포지토리 페이지 새로고침하여 살펴보기

- 파일들 내용
- 커밋 내역들

```
git remote
```

- 자세히 보기: git remote -v

💡추가사항
원격 지우기 (로컬 프로젝트와의 연결만 없애는 것. GitHub의 레포지토리는 지워지지 않음)

```
git remote remove (origin 등 원격 이름)
```

📖 2. GitHub에서 프로젝트 다운받기

```
git clone (원격 저장소 주소)
```

- 이번 강에서는 HTTPS 프로토콜 사용
- VS Code로 해당 폴더 열어보기
