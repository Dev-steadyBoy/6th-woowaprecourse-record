# <🥳프리코스에 관하여🥳>

## 🍏프로그래밍 요구사항

### 1. 공통 요구사항

- Node.js 14버전에서 실행 가능해야 한다. **Node.js 14에서 정상적으로 동작하지 않을 경우 0점 처리한다.**
- <span style = "background-color : lightgray">package.json</span>을 변경할 수 없고 외부 라이브러리(jQuery, Lodash등)를 사용하지 않는다. 순수 Vanila JS로만 구현한다.
- [JavaScript 코드 컨벤션](https://github.com/woowacourse/woowacourse-docs/tree/main/styleguide/javascript)을 지키면서 프로그래밍 한다.

  - <a href='https://velog.io/@cada/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-%EC%BD%94%EB%94%A9-%EB%B0%8F-%EB%84%A4%EC%9D%B4%EB%B0%8D-%EC%BB%A8%EB%B2%A4%EC%85%98-1%ED%8E%B8'>자바스크립트 코딩 컨벤션에 대한 글</a>
  - <a href='https://velog.io/@cada/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-%EC%8A%A4%ED%83%80%EC%9D%BC-%EA%B0%80%EC%9D%B4%EB%93%9C-%EB%84%A4%EC%9D%B4%EB%B0%8D-%EC%BB%A8%EB%B2%A4%EC%85%98-%ED%8E%B8'>자바스크립트 네이밍 컨벤션에 대한 글</a>
  - <a href='https://standardjs.com/'>JavaScript Standard Style</a>
  - <a href='https://google.github.io/styleguide/jsguide.html'>Google JavaScript Style Guide</a>
  - <a href='https://ui.toast.com/fe-guide/ko_CODING-CONVENTION'>NHN FE개발랩</a>
  - <a href='https://github.com/airbnb/javascript'>airbnb JavaScript Style Guide</a>
  - <a href='https://github.com/parksb/javascript-style-guide'>airbnb JavaScript Style Guide(한글 버전)</a>

- 프로그램 종료 시 <span style = "background-color : lightgray">process.exit()</span>를 호출하지 않는다.
- 프로그램 구현이 완료되면 <span style = "background-color : lightgray">ApplicationTest</span>의 모든 테스트가 성공해야 한다. **테스트가 실패할 경우 0점 처리한다.**
- 프로그래밍 요구 사항에서 달리 명시하지 않는 한 파일, 패키지 이름을 수정하거나 이동하지 않는다.
- indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.
  - 예를 들어 while문 안에 if문이 있으면 들여쓰기는 2이다.
  - 힌트: indent(들여쓰기) depth를 줄이는 좋은 방법은 함수(또는 메서드)를 분리하면 된다.
- 함수(또는 메서드)가 한 가지 일만 하도록 최대한 작게 만들어라.
- Jest를 이용하여 본인이 정리한 기능 목록이 정상 동작함을 테스트 코드로 확인한다.

#### 1.1 추가된 요구 사항

- 함수(또는 메서드)의 길이가 15라인을 넘어가지 않도록 구현한다.
  - 함수(또는 메서드)가 한 가지 일만 잘 하도록 구현한다.
- else를 지양한다.
  - 힌트: if 조건절에서 값을 return하는 방식으로 구현하면 else를 사용하지 않아도 된다.
  - 때로는 if/else, switch문을 사용하는 것이 더 깔끔해 보일 수 있다. 어느 경우에 쓰는 것이 적절할지 스스로 고민해 본다.
- 도미엔 로직에 단위 테스트를 구현해야 한다. 단 UI(Console.readLine, Console.print) 로직에 대한 단위 테스트는 제외한다.
  - 핵심 로직을 구현하는 코드와 UI를 담당하는 로직을 구분한다.
  - 단위 테스트 작성이 익숙하지 않다면 <span style = "background-color : lightgray">tests/~~~.js</span>를 참고하여 학습한 후 테스트를 구현한다.

---

<br>

### 2. 🍏과제 진행 요구사항

- 미션은 미션repository에서 Fork/Clone해 시작한다.
- **기능을 구현하기 전 <span style = "background-color : lightgray">docs/README.md</span>에 구현할 기능 목록을 정리**해 추가한다.
- **Git의 커밋 단위는 앞 단계에서 <span style = "background-color : lightgray">docs/README.md</span>에 정리한 기능 목록 단위**로 추가한다.
  - [커밋 메시지 컨벤션 가이드](https://gist.github.com/stephenparish/9941e89d80e2bc58a153)를 참고해 커밋 메시지를 작성한다. [번역된 페이지](https://www.conventionalcommits.org/ko/v1.0.0/)
- 과제 진행 및 제출 방법은 [프리코스 과제 제출 문서](https://github.com/woowacourse/woowacourse-docs/tree/main/precourse)를 참고한다.

> 1. fork하기
> 2. fork한 저장소 clone하기
> 3. 기능 구현을 위한 브랜치 생성
> 4. IDE로 가져오기
> 5. 기능 구현
> 6. 그 후 add, commit
> 7. 내 원격 저장소에도 올리기
> 8. Pull Request 보내기

---

<br>

### 3. ⛑️과제 제출 전 체크 리스트 - 0점 방지

- 기능 구현을 모두 정상적으로 했더라도 **요구 사항에 명시된 출력값 형식을 지키지 않을 경우 0점으로 처리**한다.
- 기능 구현을 완료한 뒤 아래 가이드에 따라 테스트를 실행했을 때 모든 테스트가 성공하는지 확인한다.
- **테스트가 실패할 경우 0점으로 처리**되므로, 반드시 확인 후 제출한다.

<br>

#### 3.1 테스트 실행 가이드

- 테스트 패키지 설치를 위해 Node.js 버전 14이상이 필요하다.
- 다음 명령어를 입력해 패키지를 설치한다.
  > npm install
- 설치가 완료되었다면, 다음 명령어를 입력해 테스트를 실행한다.
  > npm test

<br>

#### 3.2 미션 제출 방법

- 미션 구현을 완료한 후 Github을 통해 제출해야 한다.
  - Github를 활용한 제출 방법은 [프리코스 과제 제출](https://github.com/woowacourse/woowacourse-docs/tree/main/precourse)문서를 참고해 제출한다.
- Github에 미션을 제출한 후 [우아한테크코스 지원](https://apply.techcourse.co.kr/)사이트에 접속하여 프리코스 과제를 제출한다.
  - 자세한 방법은 [제출 가이드](https://github.com/woowacourse/woowacourse-docs/tree/main/precourse#%EC%A0%9C%EC%B6%9C-%EA%B0%80%EC%9D%B4%EB%93%9C) 참고
  - **PR(Pull Request)만 보내고 지원 플랫폼에서 과제를 제출하지 않으면 최종 제출하지 않은 것으로 처리되니 주의하자.**
