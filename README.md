
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
