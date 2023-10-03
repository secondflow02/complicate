
# 프로젝트명 : Git Confilct Test

## 프로젝트 개요 및 설명

- README.md 파일 작성을 통해 conflict 유도하기
- 해당 레퍼지토리는 conflict를 유도하여 해결하는 연습을 진행한다.

## 배포 링크 및 시연 영상 : URL

## 팀원 소개

- 조장 : 영록
- 조원 : 선아
- 조원 : 지영
- 조원 : 진욱
- 조원 : 필우

## 사용 기술 스택

- HTML
- JS

---

## Code Convention

1. 명명 규칙

- 변수명, 함수명 : 카멜 케이스를 사용한다.
- 생성자 함수, 클래스 : 파스칼 케이스를 사용한다.
- 그 외(ex. 상수) : 스네이크 케이스를 사용한다.

- 배열 : 복수형으로 이름을 생성한다.

2. 블록 구문

- 한 줄 짜리 블록일 경우라도 { }를 생략하지 않고 명확히 줄 바꿈 하여 사용한다.

3. 문장 종료

- 문장 종료 시에는 반드시 세미콜론(;)을 사용한다.

4. 함수

- return : 바로 return 하는 경우에도 return을 사용한다.
- 불린 반환 함수 : 반환 값이 불린인 함수는 ‘is’로 시작한다.

5. 이벤트 핸들러

- 이벤트 핸들러는 ‘on’으로 시작한다.

6. 주석

- 작성자, 작성한 내용을 함께 작성한다.

---

## Git Commit Convention

- TYPE : 어떤 의도로 커밋했는지 명시한다.

  - feat : 새로운 기능 추가
  - fix : 버그 수정
  - docs : 문서 수정 (ex. README.md 수정 등)
  - style : 코드 포맷 변경, 세미콜론 누락 등 코드 수정이 없는 경우 (ex. 오타 수정, 탭 사이즈 변경, 변수명 변경 등)
  - test : 테스트 추가, 테스트 리팩토링 (프로덕션 코드 수정 X)
  - chore : 빌드 테스크 업데이트, 패키지 매니저를 설정하는 경우 등 (프로덕션 코드 수정 X) (ex. package.json의 변경이나 dotenv의 요소 변경 등, 모듈의 변경)
  - Design : CSS 등 사용자 UI 디자인 변경
  - !BREAKING CHANGE : API 변경의 경우 (ex. API의 arguments, return 값의 변경, DB 테이블 변경, 급하게 치명적인 버그를 수정할 경우)
  - !HOTFIX : 긴급하게 치명적인 버그를 고쳐야 하는 경우
  - Comment : 필요한 주석 추가 및 변경
  - Rename : 파일 혹은 폴더명을 수정하거나 옮기는 작업인 경우
  - Remove : 파일을 삭제하는 작업만 수행한 경우

- SUBJECT

  - 제목은 최대 50글자가 넘지 않도록 하고, 마침표 및 특수기호는 사용하지 않는다.
  - 영문으로 표기하는 경우 동사 원형을 가장 앞에 두고, 첫 글자는 대문자로 표기한다. (과거시제 X)
  - 제목은 서술형 문장이 아닌 간결하고 요점적인 서술을 한다. (ex. Fixed → Fix | Added → Add | Modified → Modify)
  - 한글로 제목을 작성할 경우 ⇒ 고침, 추가, 변경 으로 시작

- BODY : 상세 설명 작성

  - 한 줄 당 72자 내로 작성한다.
  - 양에 구애받지 않고 최대한 상세히 작성한다.
  - 어떻게 변경했는지보다 무엇을 변경했는지 또는 왜 변경했는지를 설명한다.

- FOOTER : 선택적이며, 이슈 트래커 ID 작성
  - **"유형: #이슈 번호"** 형식으로 사용
  - 여러 개의 이슈 번호를 적을 때는 쉼표(,)로 구분
  - 이슈 트래커 유형은 다음 중 하나를 사용한다.
    - Fixed : 이슈 수정 중 (아직 해결되지 않은 경우)
    - Resolves : 이슈를 해결했을 때 사용
    - Ref : 참고할 이슈가 있을 때 사용
    - Related to : 해당 커밋에 관련된 이슈 번호 (아직 해결되지 않은 경우)
// 여기까지가 지영님 내용입니다.

# 프론트엔드 2조 convention 20231003

## Index
1. [Javascript Code Convetion](#javascript-code-convention)
2. [Git Commit Convention](#git-commit-convention)

# Javascript Code Convention

1. 명명 규칙
    * 변수명, 함수명
        카멜 케이스를 사용한다.
        ```javascript
            var firstName;
        ```    
    * 생성자 함수, 클래스
        파스칼 케이스를 사용한다.
        ```javascript
            var FirstName;
        ```
    * 그 외 (ex.상수)
        스네이크 케이스를 사용한다.
        ```javascript
            var first_name;
        ```
    * 배열
        복수형 이름을 생성한다.
        ```javascript
            var arrays;
        ```
2. 블록 구문
    * 한 줄 짜리 블록일 경우라도 {}를 생략하지 않고 명확히 줄 바꿈하여 사용한다.

3. 문장 종료
    * 문장 종료 시에는 반드시 세미콜론(;)을 사용한다.
        ```javascript
            // x
            function semicolon(){
                return x
            }
            // o
            function semicolon(){
                return x;
            }
        ```
4. 함수
    * return
        바로 return하는 경우에도 return을 사용한다.
        ```javascript
            // X
            var return = (func)=> {func+1;};
            // o
            var return = (func)=>{return func+1};
        ```
    * boolean 반환 함수
        반환 값이 불린인 함수는 'is'시작 한다.
        ```javascript
            function isBoolean() {
                
            }   
        ```
5. 이벤트 핸들러
    * 이벤트 핸들러는 'on'으로 시작한다.
6. 주석
    * 작성자, 날짜 및 작성한 내용을 함께 작성한다.
        ```javascript
            // 홍길동, 20231001 코드를 수정하였습니다.
        ```

# Git Commit Convention

