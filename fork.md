# fork

* 기본적으로 원격저장소에 커밋을 직접 푸시할 수 있는 사람은 원격저장소를 만든 소유자 뿐이다.
* 다른 사람이 이곳에 푸시하려면 원격저장소의 소유자가 이 사람을 협력자로 등록을 해야한다. (등록안한사람이 푸시하면에러)
* 원격저장소 소유자가 협력자로 등록하려면 [Settings - Collaborators]에서 해당하는 유저를 찾고 [Add-collaborator]하면됨



***

오픈소스를 사용하다보면 여러사람의 아이디어를 담고 싶음. 그러나 원격저장소에는 뭔가 완전한 버전을 놓고 싶기 때문에 모든 사람을 다 기여자로 주기에는 부담이 너무 큼 이럴 때 대안이 될 수 있는 것이 __Pull request__ 이다. 개발자는 원본 저장소를 자신의 계정에 복사해서 원격저장소를 생성하고 이곳에 커밋을 올린 후 원본저장소의 소유자에게 병합을 요청하면 원본저장소의 소유자는 개발자의 병합 요청을 검토해 원본저장소에 반영시키는 것

__비교__

|        | 의의                                    | 편리한 점                                                    | 불편한 점                                               |
| ------ | --------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------- |
| 브랜치 | 하나의 원본저장소에서 분기를 나눈다.    | 하나의 원본저장소에서 코드 커밋 이력을 편한게 볼 수 있다.    | 다수의 사용자가 다수의 브랜치를 만들면 관리하기 힘들다. |
| 포크   | 여러 원격저장소를 만들어 분기를 나눈다. | 원본저장소에 영향을 미치지 않으므로 원격저장소에서 마음껏 코드를 수정 할 수 있다. | 원본저장소의 이력을 보려면 따로 주소를 추가해야 한다.   |

* Fork 하는법
  1. 해당 원본 저장소로 간다
  2. fork 버튼을 누른다
  3. 포크가 찍힌 책이 스캔되는 애니메이션이 나온뒤 포크가 되었다고 나온다.