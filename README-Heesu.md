# 2020-03-26 JavaScript 스터디

## Javascript
프로그래밍 쪽으로 웹브라우저를 제어하는 역할을 하기 위한 도구 또는 언어.
웹서버를 동작하기 위한 도구.

브라우저에서 동작하는 자바스크립트는 클라이언트 사이드 스크립트 라고 함


### Node.js
웹브라우저를 제어 하기 위한 기술로써의 자바스크립트
웹서버를 제어하기 위한 기술로써의 자바스크립트  
# 

### 기본 자바스크립트 작성

    <!DOCTYPE html>
    <html>
        <head>
            <meta charset="utf-8"/>
        </head>
        <body>

            <script>
                alert('Hello world');  //자바 스크립트 코드
            </script>

        </body>
    </html>



### 크롬 개발자 도구 사용
* 단축키 : Ctrl + Shift + I  
# 


### javascript 사용시 실행 도구
* Visual Studio code  
# 


### 결과를 Chrome 브라우저로 띄우기
1. vs code의 확장(Extensions) 메뉴로 진입 한 후 "open in browser"를 다운로드 받는다.
2. 실행하고자 하는 파일에서 우클릭 후 사용자의 편의에 따라 "Open in Default Browser" 혹은 "Open In Other Browser"를 클릭하여 결과를 확인한다.
    - "Open in Default Browser" 단축키 : Alt + B
    - "Open In Other Browser" 단축키 : Shift + Alt + B
# 

### 숫자와 문자

"와 '가 붙지 않은 숫자는 숫자로 인식한다.

    document.write(1);                // 숫자 1
    document.write("1");              // 문자 1
    document.write('1');              // 문자 1
      

숫자 연산도 가능하다.

    document.writeln(1+1);          // 2
    document.writeln(2-1);          // 1
    document.writeln(4*2);          // 8

단 여기에서는 &는 나머지, /는 몫을 구하는 연산이다.

    document.writeln(15%8);         // 7
    document.writeln(15/8);         // 1


## Math 객체
* 수학에서 자주 사용하는 상수와 함수들을 미리 구현해 놓은 자바스크립트 표준 내장 객체
* 수학적인 상수와 함수를 위한 속성과 메서드를 가진 내장 객체

## Math 연산 이용

    document.writeln( Math.pow(3,2) );      // 9, 3의 2제곱
    document.writeln( Math.round(5.7) );    // 6, 5.7 반올림
    document.writeln( Math.ceil(14.2) );    // 15, 14.2 올림
    document.writeln( Math.floor(10.6) );   // 10, 10.6 내림
    document.writeln( Math.sqrt(25) );      // 5, 25의 제곱근 
    document.writeln( Math.random() );      // 0.0이상 1.0 미만인 값들 중 무작위로 뽑아 낸다.


## 1 ~ 100 랜덤 숫자 뽑아내기

1. 랜덤 숫자를 뽑아내는 것이 먼저다


    Math.random();


2. 0.xxxxx 형태가 되었으므로 100을 곱해준다.


    100 * Math.random();


3. 위 상태는 100을 곱해주어 범위를 0.0이상 100.0미만으로 확장 시켰다.  
*단*, 이렇게 되면 100은 나올수가 없으므로 +1을 추가해야 한다.


    (100 * Math.random()) + 1; //1.0 이상 101.0미만


4. 이 상태에서 Math.floor만 해주어 소수점만 버린다. **완성!**


    Math.floor((100 * Math.random()) + 1);






****************
~~사실 마크다운 문법도 공부했습니다 칭찬해주세요 ㅈㅅ~~
****************