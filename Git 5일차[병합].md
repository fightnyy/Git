# 깃정리 5일차

### 브랜치와 브랜치를 합치기

* 병합: 간단히 두 버전의 합집합을 구하는 것 

  - 꽃을 든 문어 + 모자를 쓴 문어를 합치면 => 꽃과 모자를 든 문어 

    => 각 문어가 커밋이라면 새로운 커밋인 __병합 커밋__이 생김

  - 그냥 문어+ 모자를 쓴 문어를 합치면 => 모자를 쓴 문어  

    => 합친 결과물이 뒷 문어와 동일 즉, 새로 상태를 만들어 줄 필요 없이 뒷문어로 상태를 바꿈 __빨리감기 병합__

  - 꽃을 들고 털모자를 쓴 문어 + 다른 모자를 쓴 문어를 합치면 => 꽃은 겹치지 않으니까 괜찮은데 모자는 어떤 모자를 써야할 지 모르겠음 

    => __충돌(Conflict)__ 상태=>충돌이 난 부분을 확인하고 무엇을 남길지 수동으로 선택하면 됨



* 병합 과정
  * Git에서 브랜치와 브랜치를 합치는 명령어는 __merge__ 이다. 저번시간에 했던 예시로 들어보면 저번에 [feature/detail]의 작업이 끝났다. 따라서 [master]브랜치와 합쳐야 한다. 만약 [feature/detail]의 단순 수정본이라면 빨리감기 병합처럼 진행 될것이다. 예를들어 [feature/detail]이 커밋4를 가르킨다면 master도 커밋4를 가르키고 있는것이다. 
  * 병합을 하면 [feature/detail]브랜치의 모든 내용이 [master]부랜치에 반영되었으니 [feature/detail-page]브랜치는 지워도 된다.
  * 다른 팀원도 [feature/cart]브랜치에서의 개발을 끝내고 [master]브랜치에 합치려고 한다고 가정해보자. 이때 보통 [master]는 최종용이니까 우선 [feature/cart]에 먼저 merge를 하고 그다음 아무 이상이 없으면 [master]로 최종 병합을 진행한다.
  * 이때 __빨리감기 병합__이 되면 좋지만 세상이 그렇게 호락호락 하지 않다. 예를 들어 [master]에 어떤 줄과 [feature-cart]어떤 줄이 같다고 해보자 이럴경우엔 __충돌__ 상태가 일어나게 되는데 이때는 소스트리에서 경고창을 내주고 고치라고 사용자에게 알려준다. 이때 사용자는 어떤걸 쓸 건지 판단하고 고치면 된다.

