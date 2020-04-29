# origin 과 master

* __origin__ 은 우리가 연결한 __GitHub 원격저장소의 닉네임__ 이다.

ex. git remote add origin https://njfhkjshgkas.com.git

* 위의 예시는 origin이란 닉네임으로 원격저장소를 추가하라는 뜻

* __origin__꼬리표는 __원격저장소의 현재 버전상태__를 가리키는 커밋에 붙어있음

* __master__는 우리가 커밋을 올리는 __'줄기'__의 이름
* 따로 줄기를 생성하지 않으면 git은 master라는 기본줄기에 커밋을 올림

```markdown
종합해보면 아무것도 붙지 않은 __[master]는 내 컴퓨터 로컬저장소의 버전__을, 앞에 origin이 붙은 __[origin/master]는 GitHub의 원격저장소의 버전__을 가리키는 것
```

