# 1~3장 정리

## 01장 <프로그래밍>

### 1) 프로그래밍이란?

- 문제를 명확히 이해하고 분해한 후, 구분하여 순서에 맞게 배열해야 하는 작업.

### 2) 프로그래밍 언어

- 사람과 컴퓨터(컴파일러 또는 인터프리터)가 이해할 수 있는 인공어.
    
    ![**사람** -프로그래밍언어→ **컴파일러** -기계어→ **컴퓨터**](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled.png)
    
    **사람** -프로그래밍언어→ **컴파일러** -기계어→ **컴퓨터**
    

### 3) 구문과 의미

- js 변수엔 어떤 타입의 값도 할당할 수 있지만, 의미적으로 옳아야 함.
- 요구사항이 실현(해결)되어야 의미가 있음.

## 02장 <자바스크립트란?>

### 1) 자바스크립트의 탄생

- 웹페이지의 보조적인 기능을 수행하기 위해 탄생한 경량 프로그래밍 언어.
- 현재는 모든 브라우저의 표준 프로그래밍 언어로 자리잡음.

### 2) 자바스크립트의 표준화

- 마이크로소프트사의 js파생버전인 “JScript” 탄생. 크로스 브라우징 이슈가 발생하면서 모든 브라우저에서 정상적으로 동작하는 표준화된 js의 필요성이 대두됨.

### 3) 자바스크립트 성장의 역사

- 초창기 js는 한정적인 용도. 대부분의 로직은 주로 웹 서버에서 실행되고, 브라우저는 서버로부터 전달받은 html, css를 단순히 시각적으로 출력하는 수준이었음.

3-1) Ajex

- js 이용해 서버와 브라우저가 비동기 방식으로 데이터 교환할 수 있는 통신기능임.

3-2) jQuery

- 제이쿼리 등장으로 번거롭고 논란있던 DOM을 쉽게 제어할 수 있게 되고 크로스 브라우징 이슈도 어느정도 해결됨. 다소 까다로운 js 보다 배우기 쉽고 직관적임.

3-3) V8 자바스크립트 엔진

- js로 웹 애플리케이션을 구축하려는 시도가 늘면서 더 빠르게 동작하는 js 엔진. 이것의 등장으로 js는 데스크톱 애플리케이션과 유사한 사용자경험(UX)을 제공할 수 있는 웹 애플리케이션 프로그래밍 언어로 정착함.

3-4) Node.js

- 구글 V8 자스 엔진으로 빌드된 js 런타임 환경임. 브라우저의 js 엔진에서만 동작하던 js를 브라우저 이외의 환경에서도 동작할 수 있도록 js엔진을 브라우저에서 독립시킨 js 실행환경임. 다양한 플랫폼에 적용할 수 있지만, 서버 사이드 애플리케이션 개발에 주로 쓰이며, 이에 필요한 빌트인 API 제공함.
- 언어가 아니고 환경 WHR

3-5) SPA 프레임워크

- 개발규모와 복잡도의 상승에 필연적으로 등장한 프레임워크.

### 4) 자바스크립트와 ECMAScript (에크마) es6는 리액트

- ECMAScript는 js의 표준사양인 ECMA-262. 핵심문법을 규정함.
- JavaScript는 (프로그래밍 언어로서)기본 뼈대를 이루는 **ECMAScript**와 브라우저가 별도지원하는 **클라이언트 사이드 Web API**를 아우름.
    
    ![Untitled](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%201.png)
    

### 5) 자바스크립트의 특징

- js는 html, css와 함께 웹을 구성하는 요소 중 하나. **웹 브라우저에서 동작하는 유일한 프로그래밍 언어**.
- 개발자가 별도의 컴파일작업 수행하지 않는 **인터프리터 언어(한줄씩 읽어들임)**.
    
    ![참고](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%202.png)
    
    참고
    
- 명령형, 함수형, 프로토타입 기반 객체지향 프로그래밍 지원하는 멀티 패러다임 프로그래밍 언어.
- 클래스 기반 객체지향 언어보다 효율적이면서 강력한 프로토타입 기반의 객체지향 언어.

ES6 브라우저 지원 현황

- 구형 브라우저, 인터넷 익스플로러를 제외한 모던 브라우저의 ES6 지원률은 거의 100%에 육박.

## 03장 <자바스크립트 개발 환경과 실행 방법>

### 1) 자바스크립트 실행 환경

- 모든 브라우저, Node.js 환경에서 js를 실행할 수 있음. (ex.크롬 개발자도구의 console)
- 브라우저와 Node.js의 용도가 다름. 브라우저는 웹페이지를 브라우저 화면에 렌더링하는게 목적, Node.js는 브라우저 외부에서 js실행 환경을 제공하는 것이 주 목적. (Node.js는 DOM API를 제공하지 않음, 반대로 Node.js는 파일 시스템을 기본 제공함)
- 브라우저는 클라이언트 사이드 Web API를 지원하지만, Node.js는 지원하지 않고 ECMAScript와 Node.js 고유의 API 지원함.

![Untitled](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%203.png)

- 앞으로 js를 각각 **브라우저**, **Node.js**, **Visual Studio code**를 사용해 브라우저나 Node.js 환경에서 실행하는 방법을 살펴보자.

### 2) 웹 브라우저

- 구글 **크롬** 브라우저 사용.
- 크롬 브라우저의 V8 js 엔진은 Node.js에서도 사용.

2-1) 개발자 도구

- 크롬 브라우저가 제공하는 개발자 도구는 웹 애플리케이션 개발에 필수 도구. (단축키 F12)

![참고](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%204.png)

참고

2-2) 콘솔

- Console 패널은 js 코드에서 에러가 발생해 애플리케이션이 작동하지 않을 때 우선적으로 살펴봐야 함.
- 구현 단계에서는 에러가 빈번히 발생하므로 상시 콘솔을 열어둬야 함.
- 구현 단계에서 디버깅 실행하는 것보다 console.log 메서드를 사용하는게 나음. console.log(…)는 소괄호 안의 코드를 평가해서 결과를 콘솔에 출력하는 함수.
- 콘솔은 js코드 입력해 결과 확인할 수 있는 REPL(입력 수행 출력 반복) 환경으로 사용할 수도 있음.
- 코드에 줄바꿈이 필요할 땐, Shift 키를 누른 상태에서 엔터키를 누름.

2-3) 브라우저에서 자바스크립트 실행

- 브라우저는 html 파일 로드하면 script 태그에 포함된 js코드 실행함. 만약 js코드 내에서 console.log 메서드가 호출됐다면, 콘솔에 실행결과가 출력됨.

2-4) 디버깅

- 정상적으로 코드가 실행되지 않으면 **Console창 들어가, 에러 발생 위치 클릭**.
    
    ![dsd.jpg](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/dsd.jpg)
    

- 코드를 실행하는 도중에 일시정지하고 해당 시점의 변수값을 확인하기 위해 **브레이크포인트(중단점)를 걸음. 어떤 함수가 문제인지 안다면 바로 해당 라인에 중단점을 걸면 되지만, 모른다면 글로벌한 이벤트에 대해 중단점을 걸어보자.**
    
    ![왼쪽의 라인 번호 ‘13’은 브레이크포인트(중단점).](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%205.png)
    
    왼쪽의 라인 번호 ‘13’은 브레이크포인트(중단점).
    
- **마우스 커서를 올리면 변수의 값 확인할 수 있음**.
- **브레이크포인트 누르고 출력창의 ‘+’버튼 클릭하면 디버깅 모드**로 들어감.
    
    ![Untitled](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%206.png)
    
- -$counter의 변수의 값은 null임. 그 원인은 13번째 줄에서 $counter변수에 값을 할당할 때 html 요소의 아이디 ‘counter-x’로 잘못 지정한 탓임. ‘counter’로 수정하면 에러 제거됨.

### 3) Node.js

- 프로젝트 규모가 커짐에 따라 React, Angular, Lodash같은 프레임워크 또는 라이브러리 도입하거나 Bable, Webpack, ESLint 등 여러 도구 사용할 땐, Node.js와 npm이 필요함.

3-1) Node.js와 npm 소개

- Node.js는 크롬 V8 자바스크립트 엔진으로 빌드된 자바스크립트 런타임 환경임. 브라우저에서만 동작하던 **js를 브라우저 이외의 환경에서 동작시킬 수 있음**.
- npm은 자바스크립트 패키지 매니저임. Node.js에서 사용할 수 있는 모듈들을 패키지화해 모아둔 저장소 역할, 패키지 설치 및 관리 위한 CLI 제공함. 자신이 작성한 패키지 공개할 수 있고, 필요한 패키지 검색해 재사용할 수 있음.

3-2) Node.js 설치

- 다운로드 페이지에서 LTS버전은 장기적으로 안정된 지원이 보장됨. 반면 Current버전은 최신 기능 제공하지만, 업데이트가 발생하는 버전으로 안정적이지 않을 수 있음.
- 설치 후 터미널(명령 프롬포트)에서 버전 출력해 정상적으로 설치됐는지 확인함.
    
    ![npm도 함께 설치됨.](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%207.png)
    
    npm도 함께 설치됨.
    

3-3) Node.js REPL

- Node.js가 제공하는 REPL(Read Ebal Print Loop)를 사용하면 간단한 js 코드를 실행해 결과를 확인할 수 있음.
    
    ![프롬포트가 >로 변경되면 js코드 실행해 볼 수 있음.](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%208.png)
    
    프롬포트가 >로 변경되면 js코드 실행해 볼 수 있음.
    
- js 파일을 실행하려면 node 명령어 뒤에 파일 이름 입력함. 파일 확장자 .js는 생략가능.
- Ctrl+C키를 두 번 누르면 Node.js REPL이 종료됨.

### 4) 비주얼 스튜디오 코드

4-1) 비주얼 스튜디오 코드 설치

- 이미 설치돼있으므로 생략.

4-2) 내장 터미널

- 바탕화면에 myapp이라는 폴더 생성 후, index.js 파일 생성함. VS Code에는 명령 프롬포트(터미널)이 내장돼있음(단축키 Ctrl+`)
    
    ![내장된 프롬포트가 나타나면 다음과 같은 Node.js 명령어로 js 파일 실행할 수 있음.](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%209.png)
    
    내장된 프롬포트가 나타나면 다음과 같은 Node.js 명령어로 js 파일 실행할 수 있음.
    

4-3) Code Runner 확장 플러그인

- VS Code에서 Code Runner 확장 플러그인을 사용하면 내장 터미널에 단축키 사용해 ㅡjs 비롯한ㅡ 다양한 프로그래밍 언어로 구현된 소스코드 간단히 실행할 수 있음. (설치 방법은 pdf확인)
    
    ![Code Runner 단축키](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%2010.png)
    
    Code Runner 단축키
    
- 아래의 소스코드를 프롬포트에서 실행하면 에러가 발생함. 브라우저에서 알림을 띄우는 alert 함수는 브라우저에서만 동작하고 유효하기 때문. 근데 Code Runner는 Node.js 환경 사용해 js 실행함. 따라서 클라이언트 사이드 Web API가 포함된 소스코드는 Code Runner 통해 실행하지 말고 브라우저 환경에서 실행해야 함.
    
    ![Untitled](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%2011.png)
    
- 지금은 ‘브라우저 환경, Node.js 환경 모두에서 실행 가능한 **ECMAScript 표준 빌트인 함수**’와 ‘브라우저 환경에서만 실행 가능한 **클라이언트 사이드 Web API’**를 구분하기 어려울 것. 지금은 클라이언트 사이트 Web API는 Node.js 환경에서 실행할 수 없다는 것에 주목해야 함.

4-4) Live Server 확장 플러그인

- 클라이언트 사이드 Web API가 포함된 js 코드 실행하려면 Node.js환경이 아닌, 브라우저에서 실행해야 함. 밑의 예제를 실행하려면 개발자 도구의 콘솔이나, js 코드를 HTML에 삽입한 다음 HTML 파일을 브라우저에서 열어야 함.
    
    ![이 HTML 파일을 브라우저에서 직접 열어도 되지만! 파일 경로 문제 발생할수도 있고, 소스코드 수정할 때마다 매번 새로고침해야 하므로 번거로움.](%E1%84%8C%E1%85%A6%E1%84%86%E1%85%A9%E1%86%A8%20%E1%84%8B%E1%85%A5%E1%86%B9%E1%84%8B%E1%85%B3%E1%86%B7%2014db91e8639c4134b4c5ed60f021c923/Untitled%2012.png)
    
    이 HTML 파일을 브라우저에서 직접 열어도 되지만! 파일 경로 문제 발생할수도 있고, 소스코드 수정할 때마다 매번 새로고침해야 하므로 번거로움.
    
- Live Server 확장 플러그인 사용하면 소스코드 수정할 때마다 수정사항을 브라우저에 반영해주므로 편리함. 설치 후, “Go Live”버튼 누르면 가상서버가 기동되어 브라우저에 HTML 파일이 자동 로딩됨. 이후 소스코드 수정하면 자동으로 가상서버에 반영됨!





# 4~6장 정리

## 04장 <변수> (면접질문… 나중에 더 자세히 다룸)

### 1) 변수란 무엇인가? 왜 필요한가?

- 컴퓨터는 CPU를 사용해 연산하고, 메모리를 사용해 데이터를 기억함.
- 메모리는 데이터 저장하는 메모리 셀의 집합체임. 메모리 셀 하나의 크기는 1Byte(8Bits), 컴퓨터는 메모리 셀의 크기(1Byte)단위로 데이터 저장 또는 읽음.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/11db3890-d933-4252-b5d8-9aa196566149/Untitled.png)

- 각 셀마다 고유의 메모리 주소 가짐. 0부터 시작해 메모리 크기만큼 정수로 표현됨. ex) 4GB 메모리는 0부터 4,294,967,295(0x00000000~ 0xFFFFFFFF)까지의 메모리 주소 가짐.
- 컴퓨터는 모든 데이터를 2진수 처리함. 메모리에 저장되는 데이터는 종류에 상관없이(숫자, 텍스트, 동영상 등) 모두 2진수로 저장됨.
- 밑 예제의 숫자값 10, 20은 메모리 상의 임의의 위치에 저장되고 CPU는 그 값을 읽어들여 연산 수행함. 연산결과인 30도 메모리 상 임의의 위치에 저장됨. 그림에선 편의상 저장된 숫자값을 10진수로 표현했지만, 메모리에 저장되는 모든 값은 2진수임을 기억.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f8d0ef1d-0dd8-4868-a73e-870c9a33836d/Untitled.png)
    
- 성공적으로 연산이 끝났지만, CPU가 연산해 만들어낸 숫자값 30은 재사용할 수 없다는 문제가 있음. 재사용하고 싶다면 메모리주소를 통해 메모리공간에 직접 접근하는 방법밖에 없음. 하지만 직접접근은 실수로 운영체제가 사용중인 값을 변경하면 시스템을 멈추게하는 치명적 오류가 발생할 수 있음. 따라서 js는 개발자의 직접적 메모리제어 허용하지 않음.
- 만약 js가 개발자의 직접적 메모리제어 허용하더라도, 값이 저장될 메모리주소는 코드가 실행될 때 메모리상황에 따라 임의로 결정됨. 따라서 동일한컴터가 동일한코드 실행해도 코드가 실행될 때마다 메모리 주소는 변경됨. 한 마디로, 메모리주소 통해 값에 직접접근하는 방법은 올바르지 않음.
- 프로그래밍언어는 기억하고 싶은 값을 메모리에 저장하고, 저장된 값을 읽어들여 재사용하기 위해 변수라는 메커니즘 제공함. 변수는 하나의 값 저장하기 위해 확보한 공간자체 또는 메모리공간 식별하기 위해 붙인 이름임. 간단히 말하면, 값의 위치를 가리키는 상징적인 이름임. 변수는 프로그래밍언어의 컴파일러 또는 인터프리터에 의해 값이 저장된 메모리공간의 주소로 치환되어 실행됨. 따라서 개발자가 직접 메모리주소 통해 값 저장 또는 참조할 필요없고, 변수 통해 안전히 값에 접근할 수 있음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/31ef0de2-50de-4dbd-9906-beca72637baf/Untitled.png)
    
- 연산을 통해 생성된 새로운값 30은 메모리공간에 저장됨. 30을 다시 읽어들여 재사용할 수 있도록 메모리공간에 상징적인 이름 붙인 것이 **변수**임.
    
    ![값 저장=할당, 저장된 값 읽어들임=참조](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/df5e8db6-82c1-4704-b698-d3ea656f5b3e/Untitled.png)
    
    값 저장=할당, 저장된 값 읽어들임=참조
    
- 명확한 네이밍은 코드를 이해하기 쉬우며, 협업과 품질향상에 도움됨. 변수명은 첫아이 이름 짓듯, 심사숙고해서 지어야 함.

### 2) 식별자

- 변수 이름을 식별자라고도 함. 식별자는 어떤값을 구별해 식별할 수 있는 고유한 이름을 말함.
- 식별자는 메모리공간에 저장돼 있는 어떤값을 구별해 식별해낼 수 있어야 함. 이를 위해 식별자는 어떤 값이 저장돼있는 메모리주소를 기억해야 함. 식별자 result는 값 30을 식별할 수 있었음. 식별자 result는 값 30이 저장돼있는 메모리주소 0x0669F913을 기억해야 함. 즉, 식별자는 값이 저장돼있는 메모리주소와 매핑관계를 맺으며, 이 매핑정보도 메모리에 저장되어야 함.
- 이처럼 식별자는 값이 아니라 메모리주소를 기억하고 있음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bc7c60ed-7c84-4078-b292-fc414d54168a/Untitled.png)
    
- 식별자는 변수이름에만 국한되지 않고 함수, 클래스 등의 이름도 모두 식별자임. 즉, 메모리상에 존재하는 어떤값을 식별하는 이름을 모두 식별자라고 함.

### 3) 변수 선언

- 변수를 생성하는 것을 말함. 변수를 사용하려면 반드시 선언해야 함. **변수 선언시에는 var, let, const 키워드**를 사용함.
    
    **var score; // 변수 선언(변수 선언문)**
    
    변수 선언 후, 변수값을 할당하지 않았으므로 undefined값이 할당되어 초기화 됨. (선언과 초기화가 동시에 진행되기 때문.)
    

### 4) 변수 선언의 실행 시점과 변수 호이스팅

- js코드는 인터프리터에 의해 한 줄씩 순차적으로 실행되므로 밑의 예제는 참조에러가 발생할까? 하지만 **변수선언이 런타임(소스코드가 한 줄씩 실행되는 시점)이 아니라 그 이전 단계에서 먼저 실행되기 때문**에 참조에러는 발생하지 않고, undefined가 출력됨.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/08d19b1b-d7d3-4f48-befd-631d420b68e2/Untitled.png)
    
    변수 선언문보다 변수 참조하는 코드가 앞에 있음.
    
- js 엔진은 소스코드를 한 줄씩 실행하기 전, 먼저 소스코드의 평가과정을 거치면서 준비한다. 이때 소스코드 실행을 위한 준비단계인 평가과정에서 js 엔진은 변수선언을 포함한 모든 선언문을 소스코드에서 찾아내 먼저 실행함. 그리고 평가과정이 끝나면 비로소 변수선언 포함한 모든 선언문을 제외하고 소스코드를 한 줄씩 순차적으로 실행함. 즉, **js 엔진은 변수선언이 어디에 있든, 다른 코드보다 먼저 실행된다는 것**. 따라서 변수선언이 어디에 있든, 어디서든지 변수를 참조할 수 있음.
- 이처럼 변수선언문이 코드의 선두로 끌어 올려진 것처럼 동작하는 js 고유의 특징을 **변수 호이스팅**이라고 함. 변수선언뿐만 아니라 var, let, const, function, funtion*, class 키워드 사용해 선언하는 모든 식별자는 호이스팅 됨.

### 5) 값의 할당

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/be20d6a9-19fe-47ec-b480-c447bb1ea8aa/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4dbf6640-dcd3-45ad-bb88-edcc3354256a/Untitled.png)

두 개의 코드는 정확히 동일하게 동작함. 즉, js 엔진은 2번 예제처럼 코드를 단축해도 변수선언과 값의할당을 나누어 각각 실행한다는 것. 이때 주의할 점은 변수선언과 값의할당의 시점이 다르다는 것. 변수선언은 소스코드가 순차적으로 실행되기 전, 즉 런타임 이전에 먼저 실행되지만 값의할당은 런타임에 실행된다.

- 1번은 런타임 이전에 먼저 실행되고, 2번은 런타임에 실행된다. 따라서 런타임에서 score변수는 이미 undefined로 초기화돼있는 시점에서 새롭게 숫자값 80으로 변경된다.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d4b5b916-d0ec-4c06-bf96-418270294c58/Untitled.png)
    

### 6) 값의 재할당

- 이미 값이 할당돼있는 변수에 새 값을 할당해보자.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a7488045-d790-4010-b8b9-a1eb10c1c7f7/Untitled.png)
    
    var키워드로 선언한 변수는 선언과 동시에 undefined로 초기화되기 때문에 엄밀히 말하면 첨으로 값을 할당하는 것도 재할당임. 
    
- 만약 **값을 재할당할 수 없어서 변수에 저장된 값을 변경할 수 없다면 변수가 아니라 상수**라 함. 상수는 한 번 정해지면 변하지 않는 값. 다시 말해 단 한 번만 할당할 수 있는 변수.
    
    ![더이상 필요하지 않은 undefined, 80같은 불필요한 값들은 가비지 콜렉터에 의해 메모리에서 불시에 자동해제됨.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5f0990c2-1eb7-417c-a99a-c784a222a5ea/Untitled.png)
    
    더이상 필요하지 않은 undefined, 80같은 불필요한 값들은 가비지 콜렉터에 의해 메모리에서 불시에 자동해제됨.
    
    이전 값이 저장돼있던 메모리공간을 지우고 그 공간에 재할당값을 새롭게 저장하는게 아니라, 새로운 메모리공간을 확보하고 그 공간에 새 값 저장함.
    

### 7) 식별자 네이밍 규칙

- 식별자는 특수문자를 제외한 문자, 숫자, 언더스코어, 달러 기호 포함 가능. (abc,123,_,$ 가능)
- 단, 식별자는 숫자로 시작 할 수 없음.
- 예약어는 식별자로 사용할 수 없음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/768bc820-b7ce-4461-9e37-e542bf7ac188/Untitled.png)
    
- 변수는 쉼표(,)로 구분해 여러 개를 한 번에 선언할 수 있으나, 가독성이 나빠짐.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/085607a6-b536-48a0-ac3e-180a68518bbc/Untitled.png)
    
    한글이나 일본어 식별자도 사용할 수 있으나, 알파벳 외의 유니코드 문자로 명명된 식별자를 사용하는 것은 바람직하지 않음.
    
- 대소문자를 구분하므로 밑의 변수는 각각 별개임.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3b7d1cb9-6c50-4ff5-82ab-61f80571ec1b/Untitled.png)
    
- 4가지 유형의 네이밍 컨벤션. 일관성을 유지한다면 좋지만, 일반적으로 변수, 함수 이름에는 카멜케이스를 사용하고 생성자함수, 클래스 이름에는 파스칼케이스사용함. 코드 전체의 가독성 높이려면 카멜과 파스칼을 따르는게 유리함. (팀바팀!! 카멜이 제일 좋음) (데이터처리를 직렬적으로 할 수 있을 때 RxJs 공부)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0f4d5a8f-57db-48fc-9d87-a680b7b7e1a9/Untitled.png)
    
    카멜(변수, 함수)=firstName, 파스칼(생성자함수, 클래스이름)=FirstName
    

## 05장 <표현식과 문>

### 1) 값

- 식이 **평가**되어 생성된 결과.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4884bf62-ebaf-4cd9-abe7-e06fa1114cbc/Untitled.png)
    
- 모든 **값**은 데이터타입 가짐. 메모리에 2진수, 즉 Bit의 나열로 저장됨. 메모리에 저장된 값은 데이터타입에 따라 다르게 해석될 수 있음. (ex.메모리에 저장된값 0100 0001을 숫자로 해석=65, 문자로 해석=’A’)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f4b3f88c-7210-400b-bd21-628204c46767/Untitled.png)
    
    **10+20은 할당 이전에 평가되어 값을 생성해야 함.**
    

### 2) 리터럴 

- 사람이 이해할 수 있는 문자 또는 약속된 기호를 사용해 값 생성하는 표기법.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/18defcda-b131-4cc1-93db-1d1eaa259b97/Untitled.png)
    
    위 예제의 3은 **단순한 아라비아숫자가 아니라 ‘숫자 리터럴’**임. 사람이 이해가능한 아라비아숫자 사용해 숫자 리터럴 3을 코드에 기술하면 js엔진은 이를 평가해 숫자값 3 생성함.
    
- 리터럴은 사람이 이해가능한 문자(아라비아숫자, 알파벳, 한글 등) 또는 미리 약속된 기호(’’, ””, ., [], {}, // 등)로 표기한 코드. js엔진은 **런타임에 리터럴을 평가해 값 생성**함. 즉, 리터럴은 값을 생성하기 위해 미리 약속한 표기법임.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6116a45b-943e-4fb9-96c6-23dfbbddb697/Untitled.png)
    

### 3) 표현식

- 값으로 평가될 수 있는 문. 즉, 표현식이 평가되면 **새값 생성 또는 기존값 참고**함.
- 리터럴은 값으로 평가되므로 표현식이라고 할 수 있음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fea067fd-74ee-4047-aa70-1fe75e267e22/Untitled.png)
    
    위 예제의 **100은 리터럴**임. 리터럴 100은 js 엔진에 의해 평가돼 값생성하므로, 리터럴 그 자체로 **표현식**임.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2e2ad924-8e2d-4ab4-8f55-51faace5c301/Untitled.png)
    
    **50+50은 리터럴(50)과 연산자(+)**로 이뤄짐. 50+50도 **평가되어** **숫자값 100생성하므로 표현식**임.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8cb421b9-db51-4dee-9a8a-191b207c9698/Untitled.png)
    
    변수 **식별자를 참조**하면 변수값으로 평가됨. 식별자 참조는 **값생성하지 않지만**, **값으로 평가되므로 표현식**. (선언이 이미 존재한다고 가정.)
    
- 이처럼 표현식은 리터럴, 식별자, 연산자, 함수호출 등으로 이뤄짐. 즉, **값으로 평가될 수 있는 문은 모두 표현식**.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/017d5691-e099-42ca-9c12-e8d57fd64c1e/Untitled.png)
    
- **표현식**과 **표현식이 평가된 값**은 **동등한 관계**, 즉 **동치**임. (1+2와 3은 동치.) 따라서 표현식은 값처럼 사용할 수 있음. 문법적으로 **값이 위치할 수 있는 자리엔, 표현식도 위치할 수 있다는 걸 의미함.**
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/58a6babe-9bb1-4373-ade8-c0b6f71dfb28/Untitled.png)
    
    X는 이미 할당돼 있는 숫자값 3으로 평가됨. 따라서 숫자값 위치할 자리에 표현식 X를 쓸 수 있음.
    
- “표현식은 값이다”

### 4) 문

- ‘문’과 ‘표현식’을 구별, 해석할 줄 알면 js엔진 입장에서 코드 읽을 수 있고, 실행결과 예측할 수 있음.
- ‘문’은 프로그램을 구성하는 기본단위이자, 최소 실행 단위임. 문의 집합으로 이뤄진게 프로그램, 문을 작성하고 순서맞게 나열하는 게 프로그래밍. 컴퓨터에게 명령 내리므로 명령문이라고도 부름.
    
    ![4가지의 문으로 구분할 수 있음](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/28fcbdac-5397-42ca-bc94-8412808998a1/Untitled.png)
    
    4가지의 문으로 구분할 수 있음
    
- 문은 여러 토큰으로 구성됨.
- ‘토큰’은 문법적인 이미 지니며, 문법적으로 더 이상 나눌 수 없는 코드의 기본요소.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6eeecea3-8448-4075-beae-920ec0a1414a/Untitled.png)
    

### 5) 세미콜론과 세미콜론 자동 삽입 기능

- 문의 종료를 나타냄.
- 0개 이상의 문을 중괄호로 묶은 코드블록({…}) 뒤에는 세미콜론 붙이지 않음. 예를 들어 if문, for문, 함수 등. 이런 코드블록은 자체종결성을 가짐.
- ‘세미콜론 자동 삽입기능(ASI)’이 암묵적으로 수행되기에, 세미콜론은 생략 가능함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d7a708d3-c9b1-4a45-8b58-591324788fdc/Untitled.png)
    
    위의 예제처럼 간혹 ASI와 개발자의 예측이 맞지 않을 때가 있음. 세미콜론 사용을 권장하는 분위기이므로 붙이기.
    
- 실무에선 대부분 ; 씀 (팀바팀)

### 6) 표현식인 문과 표현식이 아닌 문

- 표현식=문의 일부일 수도, 그 자체로 문일 수도 있음.
    
    ![x = 1 + 2는 표현식이면서 완전한 문이기도 하다.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d421e6c8-92e6-471b-aaf4-468e170b5359/Untitled.png)
    
    x = 1 + 2는 표현식이면서 완전한 문이기도 하다.
    
- 문에는 표현식인 문과 표현식이 아닌 문이 있음. (표현식은 값으로 평가되며, 아닌 문은 값을 평가될 수 없음) (예를 들어 변수선언문은 값으로 평가될 수 없으므로, 표현식이 아닌 문임. 할당문은 값으로 평가되므로 표현식임)
- 표현식인 문과 표현식이 아닌 문을 구별하려면! **변수에 할당**해보자. 표현식은 변수에 할당할 수 있으나,  표현식이 아닌 문은 변수에 할당하면 에러발생함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/312b51da-b2a6-4831-99e8-e2e6a76be7ec/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f778d0f8-0abd-42cd-b956-10f1dbc04ff7/Untitled.png)
    
    할당문을 값처럼 변수에 할당함.  할당문(표현식인 문)은 할당한 값으로 평가됨. 즉, x=100은 100으로 평가됨. 따라서 foo변수에는 100이 할당됨.
    
- 크롬 개발자도구에서 표현식이 아닌 문을 실행하면 undefined를 출력하는 것을 **완료값**이라 함. 완료값은 표현식의 평가결과가 아님. 따라서 변수에 할당 또는 참조 불가능함.
    
    ![표현식인 문은 평가된값 반환](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/84650302-0d01-465b-af81-56fc4e67bbca/Untitled.png)
    
    표현식인 문은 평가된값 반환
    

## 06장 <데이터 타입>

### 0) 데이터 타입이란?

- 데이터 타입은 값의 종류임. 모든 값은 데이터 타입을 가짐.
- js(ES6)는 7개를 제공함. 원시 타입과 객체 타입으로 분류됨.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c7bc57e8-f1b3-4c83-8292-3e702cbb8fa7/Untitled.png)
    
    (숫자 타입의 값 1과 문자열 타입의 값 ‘1’은 전혀 다름. 값을 생성한 목적, 용도가 다름. 숫자는 산술연산을 위해, 문자열은 텍스트를 화면에 출력하기 위해서임. 또한 확보해야 할 메모리공간의 크기, 메모리에 저장되는 2진수, 읽어들여 해석하는 방식이 다름.)
    

### 1) 숫자 타입

- 하나의 숫자 타입 존재함. 모든 수를 실수(정수 사이를 촘촘히 채운)로 처리하고 정수만 표현하는 별도의 데이터타입 존재하지 않음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2c114738-3e76-43a4-bf84-4a7ca67cd9ac/Untitled.png)
    
     정수로 표시되어도 사실은 실수라는 것.
    
- 모든 숫자 리터럴은 메모리에 배정밀도 64비트 부동소수점 형식의 2진수로 저장됨.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8d010df4-ba1e-4f72-b7c3-2b1c6312a143/Untitled.png)
    
    2진수, 16진수 등을 표현하는 데이터 타입 제공하지 않기에, 참조하면 모두 10진수로 해석됨. 
    
- Infinity, -Infinity, NaN 세가지 특별한 값 표현할 수 있음.
    
    ![1. 양의 무한대 2. 음의 무한대 3. 산술연산불가(not-a-number, 대소문자 구별 주의!)](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d011712d-885a-431f-bf2a-f2715d4e39dc/Untitled.png)
    
    1. 양의 무한대 2. 음의 무한대 3. 산술연산불가(not-a-number, 대소문자 구별 주의!)
    

### 2) 문자열 타입

- 텍스트 데이터 나타냄. 0개 이상의 16비트 유니코드 문자(UTF-16)**3의 집합.
- ‘’, “”, ``으로 텍스트를 감쌈. 일반적인 건 ''
- ''안에 "", ""안에 '' 쓸 수 있음
- 원시타입이며, 변경 불가능한 값임. 문자열이 생성된 후, 그 문자열을 변경할 수 없음.

### 3) 템플릿 리터럴

- ES6부터 도입된 새 문자열 표기법임.
- 런타임에 일반 문자열로 변환돼 처리됨.
- 백틱(``)사용해 표현함.
- 3-1) 멀티라인 문자열
    - 일반 문자열은 줄바꿈이 허용되지 않음. 줄바꿈 등의 공백을 표현하려면 백슬래시(\)로 시작하는 이스케이프 시퀀스를 사용해야 함.
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6d2a0eb4-c78f-4bf0-8c34-d527e6ed3eff/Untitled.png)
        
        ![이스케이프 시퀀스 사용해 작성한 html 코드](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0ec8e7f4-6609-456b-9a8e-be2bbf3769c3/Untitled.png)
        
        이스케이프 시퀀스 사용해 작성한 html 코드
        
    - 이런 일반 문자열과 달리 템플릿 리터럴 내에선 이스케이스 시퀀스 사용하지 않고도 줄바꿈이 허용되고, 공백이 있는 그대로 적용됨.
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6c8eed37-e27e-437a-a7d2-d95195342fc1/Untitled.png)
        
- 3-2) 표현식 삽입
    - 문자열은 문자열 연산자 +를 사용해 연결함.
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/90c011c7-b1f5-4c1d-9c20-cd938260842d/Untitled.png)
        
    - 하지만 템플릿 리터럴 내에선 표현식 삽입 통해 간단히 문자열 삽입할 수 있음. ${표현식}으로 표현식을 감쌈. 이때 표현식 평가결과가 문자열이 아니더라도 문자열로 강제 타입 변화돼 삽입됨.
        
        ![표현식삽입을 템플릿리터럴이 아닌 일반 문자열에서 사용하면 문자열로 취급되므로 주의할 것.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2b2497c7-1cdf-4769-a95f-c2272ba9f63f/Untitled.png)
        
        표현식삽입을 템플릿리터럴이 아닌 일반 문자열에서 사용하면 문자열로 취급되므로 주의할 것.
        

### 4) 불리언 타입

- 값이 true, false뿐임.
- 조건문에서 자주 사용함.

### 5) undefined 타입

- var로 선언한 변수는 **암묵적으로 undefined로 초기화**됨. 즉, 첫 할당이 이뤄질 때까지 변수선언에 의해 확보된 메모리공간을 쓰레기값(빈상태)로 내버려두지 않고, undefined로 초기화함. 따라서 변수선언 이후 값 할당않고 변수 참조하면 undefined가 반환됨.
- undefined가 반환된다면 초기화되지 않은 변수라는 걸 알 수 있음.
- 하지만 개발자가 직접 변수에 값이 없다는 걸 명시하고 싶을 땐? undefined 말고 null을 할당하자.

### 6) null 타입

- null, Null, NULL은 다 다르니 주의.
- 변수에 값이 없다는 걸 의도적으로 명시할 때 사용함.
- 즉, 변수가 이전에 참조하던 값을 더 이상 참조하지 않겠다는 뜻. 이전에 할당됐던 값에 대한 참조를 명시적으로 제거하며, js엔진은 아무도 참조않는 메모리 공간에 대해 가비지 콜렉션 수행할 것임.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ca49f9a1-3005-4924-9111-750cd5be9937/Untitled.png)
    
- 함수가 유효한 값을 반환할 수 없을 때 명시적으로 null 반환하기도 함.
    
    ![document.querySelector 메서드가 조건에 맞는 html 요소 검색할 수 없을 때 에러대신 null 반환함.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c64db275-5d58-4fb5-8084-24835ea90a28/Untitled.png)
    
    document.querySelector 메서드가 조건에 맞는 html 요소 검색할 수 없을 때 에러대신 null 반환함.
    

### 7) 심벌 타입

- ES6에 추가된 7번째 타입, 변경 불가능한 원시 타입의 값임.
- 심벌값은 다른 값과 중복되지 않는 유일무이한 값임. 따라서 이름이 충돌할 위험이 없는 객체의 유일한 프로퍼티 키 만들기 위해 사용함.
- 심벌 이외의 원시값은 리터럴 통해 생성하지만, 심벌은 Symbol함수 호출해 생성함. 이때 생성된 심벌값은 외부에 노출되지 않고, 다른 값과 절대 중복되지 않는 유일무이한 값임.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/be30cdd6-7f93-4045-ad36-bbe393378222/Untitled.png)
    

### 8) 객체 타입

- js의 데이터 타입은 크게 원시, 객체 타입으로 분류함. 그 이유는 원시와 객체가 근본적으로 다르다는 것임.
- 중요한 것은 js는 객체 기반의 언어이고, **js를 이루고 있는 거의 모든 것이 객체**라는 것임.

### 9) 데이터 타입의 필요성

- 그래서 데이터 타입이 왜 필요할까?

9-1) 데이터 타입에 의한 메모리 공간의 확보와 참고

- 메모리에 값 저장하려면 확보할 메모리공간의 크기 알아야 함. 몇 Byte 공간 사용해야 낭비없이 값 저장할지?
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/be029c57-32e4-4ebf-b966-73f4059882cf/Untitled.png)
    
    위 코드 실행되면 컴터는 100 저장하기 위해 메모리공간 확보 후, 메모리에 100을 2진수로 저장함. 이러한 처리 하려면 먼저 메모리공간의 크기를 알아야 함.
    
- js엔진은 데이터 타입에 따라 정해진 크기의 메모리공간 확보함. 위 예제의 경우, 리터럴 100을 숫자타입으로 해석하고 8바이트의 메모리공간 확보 후 2진수로 저장함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d796e169-c3ee-40ec-bc7b-1d737426d607/Untitled.png)
    
    (js는 숫자타입 값 생성할 떄 배정밀도 64비트 부동소수점 형식 사용하므로 실제 2진수 값은 위 그림과 다름)
    
- 값을 참조할 땐, 식별자 score 통해 100 저장돼있는 메모리공간의 주소(메모리 공간의 선두 메모리 셀의 주소) 찾아감.
- 만약 위의 score 변수를 8바이트 단위로 읽어들이지 않으면 값이 훼손됨. js엔진은 변수에 숫자타입의 값이 할당돼있으므로 숫자타입으로 인식하고 한 번에 그만큼의 메모리 세을 읽어들임.

9-2) 데이터 타입에 의한 값의 해석

- 그런데 메모리에서 읽어들인 2진수를 어떻게 해석해야 할까? 메모리에 저장된 값은 데이터 타입에 따라 다르게 해석될 수 있음.
- score변수에 할당된 값은 숫자타입의 값임. 따라서 참조하면 메모리공간의 주소에서 읽어들인 2진수를 숫자로 해석함.
- 데이터 타입이 필요한 이유 :
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3c4dee79-b702-4f2f-ba88-7f1877de5380/Untitled.png)
    

### 10) 동적 타이핑

10-1) 동적 타입 언어와 정적 타입 ㅜ 언어

- js의 모든 값은 데이터 타입을 갖는다고 했음. 그럼 변수는 데이터 타입을 가질까?
- 정적타입 언어(C, java)는 변수 선언할 때 데이터 타입을 사전에 선언해야 하는데, 이를 명시적 타입 선언이라고 함. 이는 변수의 타입을 변경할 수 없고, 타입에 맞는 값만 할당할 수 있음. 그리고 컴파일 시점에 타입체크(선언한 데이터타입에 맞는 값 할당했는지) 수행함으로써 에러 줄임.
- 반면 js는 변수를 선언할 때 타입을 선언하지 않음. var, let, const 키워드를 선언할 뿐. 정적타입 같이 미리 선언한 데이터타입의 값만 할당할 수 있는게 아니라, 어떠한 데이터타입의 값이라도 자유롭게 할당함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/377993a9-cd8e-4dcf-a382-b7f6c6867701/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8a582cc7-dd35-4aad-8a98-c2564701703d/Untitled.png)
    
    typeof 연산자로 변수연산하면 변수에 할당된 값의 데이터타입 반환함.
    
- 어떤 데이터타입의 값이라도 자유롭게 할당할 수 있으므로 정적타입언어에서 말하는 데이터타입과 개념이 다름. 정적타입언어는 변수선언 시점에 변수의 타입이 결정되고, 변수의 타입을 변경할 수 없음. 반면 js는 값을 할당하는 시점에 변수의 타입이 동적으로 결정되고 타입을 언제든지 자유롭게 변경할 수 있음.
- 결론은 js의 변수가 선언이 아닌 할당에 의해 타입이 결정(타입 추론)이 됨. 또한 재할당에 의해 변수타입이 언제든지 변할 수 있음. 이를 동적 타이핑이라고 하며, 동적 타입 언어(python,php,…)라고 한다.
- 변수는 타입을 가질까? 갖지 않는다. 하지만 값은 타입을 갖는다. 따라서 현재 할당돼있는 값에 의해 변수타입이 동적으로 결정된다.

10-2) 동적 타입 언어와 변수

- 동적 타입 언어는 변수에 어떤 데이터값도 할당할 수 있음. 따라서 편리함.
- 하지만 모든 소프트웨어 아키텍처엔 트레이드오프(trade-off)가 존재함. 따라서 js는 유연성이 높지만 신뢰성이 떨어진다는 단점이 있음.
    
    **밑의 동적타입언어의 변수를 사용할 때 주의할 사항을 기억하자.**
    
- 변수는 꼭 필요한 경우에 한해 제한적으로 사용해야 함. 변수값은 재할당에 의해 언제든 변경될 수 있으므로 동적타입언어는 타입 잘못 예측해 오류발생할 가능성이 높음. 변수 개수 많을수록 오류발생 확률이 높아지므로 변수를 무분별 남발하지 않고, 필요한만큼 최소한으로 유지해야 함.
- 변수 유효범위(스코프)는 최대한 좁게 만들어 부작용 억제 해야 함.
- 전역변수는 최대한 사용자제해야 함.
- 변수보단 상수를 사용해야 함. (값 변경 억제)
- 변수이름은 목적, 의미 파악할 수 있게 네이킹해야 함. 모든 식별자(변수, 함수, 클래스 이름 등)는 존재이유 파악할 수 있게 짓기.
- 가독성이 좋은 코드가 좋은 코드임을 잊지말 것.



# 7~9장 정리

## 07장 <연산자>

### 0) 연산자란?

- 연산자는 하나 이상의 표현식을 대상으로 계산을 수행해 하나의 값을 만듦. 이때 연산의 대상은 피연산자임. 피연산자는 값으로 평가될 수 있는 표현식이어야 함. 또한 피연산자와 연산자의 조합으로 이뤄진 연산자 표현식도 값으로 평가되는 표현식이어야 함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/63e80dbc-9535-43d0-ac13-5eccf8dec533/Untitled.png)
    
- 피연산자는 ‘연산의 대상’이 되어야 하므로 ‘값’으로 평가할 수 있어야 함. 연산자는 (값으로 평가된)피연산자 연산해 새값 만듦.

### 1) 산술 연산자

- 수학적 계산을 수행해 새 숫자값 만듦.  산술 연산이 불가하면, NaN을 반환함.

1-1) 이항 산술 연산자

- **+   -    *    /      %**
- 2개의 피연산자를 산술연산해 숫자값을 만듦.
- 부수효과(피연산자 값 변경)가 없고, 언제나 새 값 만듦.

1-2) 단항 산술 연산자

- **++    - -      +     -**
- 1개의 피연산자를 산술연산해 숫자값 만듦.
- 증가/감소(++/- -)연산자는 부수효과가 있음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7b42ba2d-70b0-441d-abc6-fd730db3b13c/Untitled.png)
    
- 숫자타입이 아닌 피연산자에 +단항 연산자를 사용하면 피연산자를 숫자타입으로 변환해 반환함. 이때 피연산자를 변경하진 않음. 따라서 부수효과 X.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f74159ec-4165-4d9e-b08b-1c9bfc50141b/Untitled.png)
    
- - 단항 연산자는 **+ → -, - → +**로 피연산자의 부호를 반전한 값 반환함. 숫자타입 아닌 피연산자에 사용하면 숫자타입으로 변환해 반환함. 이때 피연산자를 변경하진 않음.따라서 부수효과 X.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f2f5b6a3-73b1-4e7c-bf45-610f96a2a8e4/Untitled.png)
    

1-3) 문자열 연결 연산자

- + 연산자는 피연산자 중 하나 이상이 문자열일 때 문자열 연결 연산자로 동작함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/40ed8738-4716-4e57-888f-d8a7677fe2ed/Untitled.png)
    
    true, false, null은 각각 1,0,0으로 타입 변환됨. 이를 암묵적타입변환(타입강제변환)이라고 함. undefined는 숫자로 타입변환되지 않음. 
    

### 2) 할당 연산자

- **=    +=    -=    *=    /=    %=**
- 우항에 있는 피연산자의 평가결과를 좌항의 변수에 할당함. 따라서 부수효과 O
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d649b18b-65df-440a-91a9-9a6590be0fd8/Untitled.png)
    
- 할당문은 값으로 평가되는 표현식이고, 할당된 값으로 평가됨. (var x;  console.log(x=10); //10, x=10은 x에 할당된 10으로 평가됨)
- 할당문은 표현식인 문이므로 여러 변수에 동일한 값 연쇄 할당할 수 있음. (var a,b,c;   a=b=c=0;  //모두 0으로 초기화됨)

### 3) 비교 연산자

- 좌항과 우항의 피연산자 비교 후 결과를 불리언 값(true, false)으로 변환함. if, for문 같은 제어문에서 주로 사용함.

3-1) 동등/일치 비교 연산자

- **==(동등비교)    ===(일치비교)    ! =    ! ==**
- 좌항과 우항의 피연산자가 같은 값으로 평가되는지 비교해 불리언값 반환함.
- ==(동등비교)는 느슨, ===(일치비교)는 엄격함.
- ==(동등비교)는 비교할 때 암묵적타입변환 통해 타입 일치 시킨 후 같은 값인지 비교함. 따라서 타입이 다르더라도 같은 값이면 true임. (5==’5’ //true) 결과 예측이 어렵고, 사용자제 해야 함.
- ===(일치비교)는 타입,  값이 같을 때 true 반환함. 따라서 암묵적타입변환 하지 않음. (5===’5’ //false)
- NaN은 자신과 일치하지 않는 유일한 값임 따라서 숫자가 NaN인지 조사하려면 isNaN 사용함.(isNaN(NaN); 과 isNaN(1+undefined);는 모두 true 반환함)
- js에는 양과 음의 0이 있는데 이들을 일치/동등 비교하면 true 반환하므로 주의!!
- ! =(부동등비교)와 ! ==(불일치비교)는 각각 동등, 일치 연산자의 반대 개념. (5 != 5; //false) (5 !== ’5’; //true)

3-2) 대소 관계 비교 연산자

- **> < ≥ ≤**
- 피연산자 크기 비교해 불리언값 반환함.

### 4) 삼항 조건 연산자

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6e91f1e8-2038-4d34-83b6-6db0c959d12f/Untitled.png)

## 08장 <제어문>

- 조건에 따라 코드블록실행(조건문)하거나 반복실행(반복문)할 때 사용함.
- 제어문 사용하면 코드 실행 순서가 변경되므로 가독성 해침. forEach, map, filter, reduce 같은 고차함수는 제어문 사용 억제해 복잡성 해결함.

1) 블록문 (=코드블록)

- 0개 이상의 문을 중괄호로 묶음.
- 블록문을 하나의 실행단위로 취급함.
- 단독으로 쓸 수 있으나 일반적으로 제어문, 함수 정의할 때 사용.
- 블록문은 언제나 자체 종결성 갖기 때문에 세미콜론 붙이지 않음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ea3ab428-a014-46f2-9219-65f5be604860/Untitled.png)
    

2) 조건문

- 조건식은 불리언값으로 평가되는 표현식임.

2-1) if … else문

- if 문의 조건식은 불리언값으로 평가되어야 함. 만약 불리언이 아닌 값으로 평가되면 js 엔진에 의해 암묵적 타입 변환됨.
    
    ![코드 블럭 내의 내용이 한 줄이면 중괄호 생략가능.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/60a04f81-26dd-49b8-b40d-bbbb30c74d63/Untitled.png)
    
    코드 블럭 내의 내용이 한 줄이면 중괄호 생략가능.
    
- 대부분의 if 문은 삼항 조건 연산자로 바꿔쓸 수 있음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/88660abe-c4cd-497f-9f92-d539c540745f/Untitled.png)
    
    ![조건식의 값이 0이어서 불리언 값인 false로 변환됨](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5f9efb5f-d510-4368-bb8e-5f2af5096479/Untitled.png)
    
    조건식의 값이 0이어서 불리언 값인 false로 변환됨
    
- 경우가 세 가지일때도 삼항 조건 연산자로 표현할 수 있음
    
    ![왼쪽 num의 값이 0이므로 false로 변환돼 ‘영’이 반환됨.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/60430b8f-fb36-44a2-a62e-ed40ea03b293/Untitled.png)
    
    왼쪽 num의 값이 0이므로 false로 변환돼 ‘영’이 반환됨.
    
- num>0 ? ‘양’ : ‘음’은 값으로 표현되기에 표현식임. 따라서 삼항 조건 연산자는 값처럼 사용할 수 있어서 변수에 할당할 수 있음. 하지만! if … else문은 표현식이 아닌 문임. 따라서 변수에 할당할 수 없음.

2-2) switch문

- 주어진 표현식 평가하여 그 값과 일치하는 표현식 갖는 case문으로 실행흐름 옮기.
- 표현식과 일치하는 case문이 없으면 default문으로 이동함. default문은 옵션.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/22071c20-3338-41d9-94d8-460552a539ae/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/56903a6d-8abd-454a-9f3e-0e6149dc3dfb/Untitled.png)
    
- 문의 마지막에 break문을 사용하지 않으면 해당하는 문에서 탈출하지 않고 맨 마지막 문으로 할당되는 걸 폴스루라고 함. (유용할 때도 있음)
- default문은 break문 생략이 일반적임.(switch문의 맨 마지막에 위치하므로 자동으로 switch문을 빠져나오기 때문에)

3) 반복문

- 조건식이 거짓일 때까지 평가해 코드블록 반복함.

3-1) for문

- 반복횟수가 명확할 때 주로 사용함.
- 밑 예제는 i 변수가 0으로 초기화된 상태에서 시작함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/294e1c84-69c0-4ca9-a14a-dbb78d08364f/Untitled.png)
    
- 무한루프
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a313c16f-1a5d-4e7f-94d3-4fb3ff7497f0/Untitled.png)
    

3-2) while문

- 반복횟수가 불명확할 때 주로 사용함.
- 조건식의 평가 결과가 참이면 코드 블록을 계속해서 반복실행함.
- 조건식의 결과가 불리언값이 아니면 암묵적 타입 변환해 논리적 참, 거짓 구별함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6c906692-ca26-40d6-8091-daa3afc0b323/Untitled.png)
    
- 무한루프에서 탈출하려면 if문으로 탈출조건 만들고 break문으로 탈출함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/15297e32-f3a8-44c3-afd3-40e493478af8/Untitled.png)
    

3-3) do … while문

- 무조건 한 번 이상 실행 후 조건식 평가함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7ff57dd7-d805-4ffe-b92a-664503f7579a/Untitled.png)
    

4) break문

- 반복문, switch문 외 레이블문에서도 코드 블록을 탈출함.
- 이 외에 break문 사용하면 SyntaxError(문법오류) 발생함.
- 레이블문은 식별자가 붙은 문으로 프로그램의 실행순서를 제어함. (switch문의 case, default도 레이블문임) 레이블문 탈출하려면 break문에 레이블 식별자 지정해야 함.
    
    ![하지만 중첩된 for문 외부로 탈출할 때만 사용하길 권장함.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6c431a1b-da1c-4c51-b88d-a1a253f4eab4/Untitled.png)
    
    하지만 중첩된 for문 외부로 탈출할 때만 사용하길 권장함.
    
- 문자열에서 특정 문자의 인덱스(위치)를 검색하는 예제임.
    
    ![문자열 세번째 ‘l’에 도착하면 for문을 탈출해버림.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a11f3371-e425-4274-915a-02538a4da718/Untitled.png)
    
    문자열 세번째 ‘l’에 도착하면 for문을 탈출해버림.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b1f1680b-8e88-4834-a721-a5aabdfafc59/Untitled.png)
    

### 5) continue문

- 반복문의 코드블록실행을 현 지점에서 중단하고 증감식(맨 위)로 실행흐름 이동함.
    
    ![문자열에서 특정 문자 개수 세는 예제.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4a4fde89-91b9-423e-a94f-7312a4e603ef/Untitled.png)
    
    문자열에서 특정 문자 개수 세는 예제.
    
    ![위 예제의 for문과 동일하게 작동함.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9b79e02d-682f-4678-840b-5003ed4048e8/Untitled.png)
    
    위 예제의 for문과 동일하게 작동함.
    
    if문 내에 실행해야 할 코드가 한 줄이면 위와 같이, 코드가 길다면 continue문을 사용하는게 가독성이 좋음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f0f4151b-e048-4d1f-951b-f78c30698e70/Untitled.png)
    

## 09장 <타입 변환과 단축 평가>

### 1) 타입 변환이란?

- js의 모든 값은 타입이 있음. 이를 개발자 의도에 따라 변환할 수 있음. 이것을 **명시적 타입 변환(타입 캐스팅)**이라고 함. 반대로, 개발자 의도완 달리 표현식 평가 중 js엔진에 의해 변환되는 건 **암묵적 타입 변환(타입 강제 변환)**이라고 함.
    
    ![명시적 타입 변환](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/aeb6d51c-e64b-492c-ba43-ab7d29dfa9e2/Untitled.png)
    
    명시적 타입 변환
    
- 둘 다 원래의 값을 변경하지 않음. 타입 변환은 기존 원시값 사용해 다른 타입의 새 원시값 생성하는 것임.
    
    ![암묵적 타입 변환](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/607e3480-2ff3-480e-a4e6-9e3797f946a5/Untitled.png)
    
    암묵적 타입 변환
    
    js엔진은 표현식 x + ‘’ 평가하기 위해 x 변수의 숫자값(10)을 바탕으로 새 문자열 값 ‘10’ 생성하고 이것으로 ‘10’=’’ 평가함. 이때 암묵적으로 생성된 ‘10’은 x에 재할당되지 않고 표현식 평가가 끝나면 아무도 참조 않으므로 가비지 콜렉터에 의해 메모리에서 해제됨. 즉, js엔진은 피연산자값을 암묵적으로 타입변환해 새 타입 값 만들어내고 단한 번 쓰고 버림.
    
- **중요한 건 코드를 예측할 수 있어야 함.**

### 2) 암묵적 타입 변환

- js엔진은 코드의 문맥을 고려해 암묵적 타입 변환함.

2-1) 문자열 타입으로 변환

- **1 + ‘2’ // 102** 에서 +연산자는 피연산자 중 하나 이상이 문자열이므로 문자열 연결 연산자로 동작함. 따라서 +연산자의 모든 피연산자는 문맥상 문자열 타입이어야 함.
- 피연산자만이 암묵적 타입 변환이 되는 건 아님. 템플릿 리터럴의 표현식 삽입은 표현식의 평가 결과를 암타변함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d30bf3a7-0d96-4e7a-8d6b-ec53211c0505/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cd4e6f11-95b1-4941-bbc0-4c306e8b7453/Untitled.png)
    

2-2) 숫자 타입으로 변환

- -, *, / 연산자는 숫자값을 만드는 게 목적이기 때무에 문맥상 피연산자가 모두 숫자타입이어야 함. 이때 피연산자를 숫자타입으로 반환할 수 없다면, 평가결과로 NaN을 반환함.
- 불리언 값을 만들어내는게 목적인 비교 연산자(>, <) 역시, 피연산자의 크기를 비교해야 하므로 문맥상 모두 숫자타입이어야 함. 따라서 문맥에 따라 암타변함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8ed37e8a-c299-4761-977e-879023ec908e/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d2c8a3d9-d4d6-4b46-b661-c67684b4babe/Untitled.png)
    
    빈 ‘’, 빈 [], null, false는 0으로, true는 1로 변환됨.(객체, 비지 않은 배열, undefined는 변환되지 않아 NaN이 됨)
    

2-3) 불리언 타입으로 변환

- if, for문 같은 제어문 또는 상항 조건 연산자의 조건식은 불리언(true, false)값으로 평가되는 표현식임.
- 이때 js엔진은 불리언 타입이 아닌 값인 Truthy(참으로 평가되는 값)는 true로, Falsy는 False로 암타변함. false로 평가되는 Falsy값은 false, undefined, null, 0, -0, NaN, ‘’(빈 문자열)이 있음. 이외의 모든 값은 ture로 평가되는 Truthy값임.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5a06ce28-e8ae-42a7-92e7-cb2307383897/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d2ad6cc3-51f7-46b3-be82-bb6690eb9b70/Untitled.png)
    

### 3) 명시적 타입 변환

- 표준 비트인 생성자함수(string, AQNumber, Boolean)를 new 연산자 없이 호출하는 방법, 빌트인 메서드 사용하는 방법, 앞서 본 암묵적 타입 변환 이용하는 방법이 있음.
- 3-1) 문자열 타입으로 변환
    1. String 생성자 함수를 new 연산자 없이 호출하는 방법
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/59a0c3fb-b540-4ce2-b2da-c477381f9f01/Untitled.png)
        
    2. Object.prototype.toStirng 메서드를 사용하는 방법
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/29fe9d40-f09f-4196-aad7-5dd0e8c8e0ad/Untitled.png)
        
    3. 문자열 연결 연산자를 이용하는 방법
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6588180d-f856-4d32-b9c6-5368fa8745df/Untitled.png)
        
- 3-2) 숫자 타입으로 변환
    1. Number 생성자 함수를 new 연산자 없이 호출하는 방법
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9f89d75c-207a-4b56-99c0-6336efb4bfaf/Untitled.png)
        
    2. parseInt. parseFloat 함수를 사용하는 방법(문자열만 숫자로 타입변환가능)
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fe5894a2-bca8-4e70-a975-c45f73c5b23b/Untitled.png)
        
    3. + 단항 산술 연산자 이용하는 방법
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9a09c369-bb7e-4d8e-a52b-433ccb71fb42/Untitled.png)
        
    4. * 산술 연산자 이용하는 방법
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7006ea07-1d6b-44d4-9e4d-814c7c2d5c55/Untitled.png)
        
- 3-3) 불리언 타입으로 변환
    1. Boolean 생성자 함수를 new 연산자 없이 호출하는 방법
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/608e8cd7-6bf6-4a56-a75b-d93661b4f7a3/Untitled.png)
        
    2. ! 부정 논리 연산자를 두 번 사용하는 방법 
        
        ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2106105c-1102-4601-b3e1-dfba2be1b867/Untitled.png)
        

### *4) 단축 평가*

4-1) 논리 연산자를 사용한 단축 평가

- “논리합(::) 또는 논리곱(&&) 연산자 표현식의 평가결과는 불리언 값이 아닐 수 있음. 이들은 언제나 2개의 피연산자 중 어느 한 쪽으로 평가됨.”
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bec55747-79a1-4817-a431-05c4588788bc/Untitled.png)
    
    논리곱 연산자는 2개의 피연산자가 모두 true로 평가될 때 true 반환함. 또한 좌항에서 우항으로 평가됨. 여기서 ‘Cat’이 Truethy값이라서 true로 평가되는 시점까진 위 표현식을 평가할 수 없음. 두번째 피연산자까지 평가해봐야 위 표현식 평가 가능함. 다시 말해, “두번째 피연산자가 논리곱 연산자 표현식의 평가결과를 결정(좌우)함. 그리고 논리연산의 결과 결정하는 두번째 피연산자, ‘Dog’를 그대로 반환함. 
    
- 논리합(::) 연산자도 위와 동일히 동작함. 논리합은 2개의 피연산자 중 하나만 true로 평가되도 true 반환함. 그럼 이때, Truthy값이므로 true로 평가되는 ‘Cat’이 그대로 반환됨. “두번째 피연산자까지 평가해보지 않아도 표현식 평가할 수 있기 때문”
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5c6669eb-6da6-433f-ac75-3e73f0f9bea3/Untitled.png)
    
    이처럼 &&, :: 연산자는 논리연산의 결과를 결정하는 피연산자를 타입 변환 없이, 그대로 반환함. 이를 단축 평가라고 함. 표현식 평가 도중 평가결과가 확정된 경우, 나머지 평가과정 생략하는 것임.
    
- 단축 평가로 if문 대체할 수 있음. 어떤 조건이 Truthy값일때 무언가 해야한다면, 논리곱(&&)연산자 표현식으로 대체함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a5ee6c70-b7fc-47fb-8555-f67536cebad2/Untitled.png)
    
    조건이 Falsy값일땐 논리합(::)으로 대체가능
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/28cc19b1-e52e-4070-b594-c0c8d9c42f24/Untitled.png)
    
- 참고로 삼항 조건 연산자는 if…else문 대체가능함.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cf190621-d5fc-4fb2-be15-2087cb8a4db6/Untitled.png)
    
- 단축평가에는 유용한 패턴이 있음.

4-2) 옵셔널 체이닝 연산자

- ES11에서 도입된 옵셔널 체이닝 연산자(?.)는 좌항의 피연산자가 null, undefined인 경우 undefined를 반환하고, 그렇지 않으면 우항의 프로퍼티 참조 이어감.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7d7dfcd1-9635-48ee-95f3-0f7e7e30fead/Untitled.png)
    
    ?.는 객체를 가리키기 기대하는 변수가 null, defined가 아닌지 확인하고 프로퍼티 참조할 때 유용함. 도입되기 전에는 논리연산자 && 사용한 단축평가 통해 변수가 null, defined인지 확인했음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/da1de528-8da5-444d-b60b-0d55319ad098/Untitled.png)
    
    &&는 좌항 피연산자가 falsy값(false, undefined, null, 0, -0, NaN, ‘’)이면 좌항 피연산자를 그대로 반환함. 하지만 0, ‘’은 객체로 평가될 때도 있음.
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a8d0107d-b3b2-4b25-ba21-8da008ae885c/Untitled.png)
    
    155p확인
