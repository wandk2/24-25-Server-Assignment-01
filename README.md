# GDG 서버 파트 1주차 과제

## 과제 설명
회원을 저장하고 관리할 수 있는 회원 관리 시스템을 만들어 봅시다.<br>
jun 패키지 안에 이미 구현되어 있는 ManagementSystem 인터페이스를 사용해 구현하면 됩니다.<br>
Main 클래스의 main() 메서드를 통해, 본인이 제대로 구현했는지를 테스트해볼 수 있습니다.<br>

## 구현해야 하는 기능 및 조건
1. addMember()
   - 파라미터로 받은 정보를 토대로 새로운 멤버 인스턴스를 생성해서 저장하는 메서드
   - 멤버는 반드시 컬렉션을 통해 저장해야 합니다
   - 저장된 모든 멤버의 id는 서로 달라야 합니다(중복될 수 없습니다)
   - 저장에 성공했다면 true를 반환하고, 실패했다면 false를 반환합니다
2. removeMember()
   - id를 토대로 멤버를 찾아 컬렉션에서 제거하는 메서드
   - 삭제에 성공했다면 true를 반환합니다
   - 삭제에 실패했다면(존재하지 않는 멤버를 삭제하려는 경우) false를 반환합니다
3. updateMember()
   - id를 토대로 멤버를 찾아 수정하는 메서드
   - 수정에 성공했다면 true를 반환합니다
   - 수정에 실패했다면(존재하지 않는 멤버를 수정하려는 경우) false를 반환합니다
   - 이름과 나이를 같이 수정하거나 각각 수정할 수 있도록 오버로딩 되어 있습니다
4. findById()
   - id를 토대로 멤버를 찾아 반환하는 메서드
5. findMembers()
   - 파라미터로 조건을 전달받아, 조건에 일치하는 멤버들을 List 형태로 반환하는 메서드
   - 메서드 내부에서 Stream을 사용해야 합니다
6. findMember()
   - 파라미터로 조건을 전달받아, 조건에 일치하는 멤버 하나를 반환하는 메서드
   - 메서드 내부에서 Stream을 사용해야 합니다
7. printMembers()
   - 컬렉션에 저장된 모든 멤버를 출력하는 메서드
   - 테스트용 메서드이기 때문에, 반드시 구현할 필요는 없습니다
8. getSize()
   - 컬렉션에 저장된 멤버의 수를 반환하는 메서드

## 주의사항
1. main() 메서드로 테스트해서 모든 기능이 정상적으로 동작하는지 확인해 볼 것을 권장합니다.
2. findMemberes()와 findMember()는 반드시 Stream을 사용해 구현해야 합니다.
3. 멤버에 대한 정보는 반드시 컬렉션을 통해 저장되어야 합니다.

## 과제 제출
본인 이름으로 src 디렉토리 안에 패키지를 하나 만들어서 구현하면 됩니다.<br>
과제를 성공적으로 구현하셨다면, AIOS 세션 때와 같이 PR을 통해 과제를 제출하시면 됩니다.
