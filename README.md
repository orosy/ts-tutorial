# TypeScript 간단 예제
1. Counter 만들기
- `useState`를 사용할 때에는 `useState<string>` 과 같이 Generics 를 사용합니다.
- `useState`의 Generics 는 상황에 따라 생략할 수도 있는데, 상태가 `null` 인 상황이 발생할 수 있거나, 배열 또는 까다로운 객체를 다루는 경우 Generics 를 명시해야 합니다.
- 예시 코드
```jsx
type Information = { name: string; description: string };
const [info, setInformation] = useState<Information | null>(null);
```

2. Input 상태 관리하기
3. Counter를 `useReducer`로 다시 구현하기
- `useReducer`를 사용할 때에는 액션에 대한 타입스크립트 타입들을 모두 준비해서 `|` 문자를 사용하여 결합시켜야합니다.`

<br />

---
참고 사이트: [타입스크립트로 리액트 Hooks 사용하기 (useState, useReducer, useRef)](https://velog.io/@velopert/using-hooks-with-typescript)
