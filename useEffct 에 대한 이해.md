# useEffect Hook에 대한 이해

- 리액트 컴포넌트가 렌더링 될때 마다 특정 작업을 수행하도록 설정할 수 있는 Hook.
- Class형 컴포넌트의 componentDidMount, componentDidUpdate를 합친 형태라고 보면 이해하기 쉽다.


## 1. 컴포넌트가 최초 마운트되거나 업데이트 됐을때 모두 실행

`
useEffect(()=>{console.log('렌더링 되었습니다')})
`

## 2. 컴포넌트가 최초 마운트되었을때만 실행
- 함수의 두번째 파라미터로 빈 배열 전달

`
useEffect(()=>{console.log('마운트 되었습니다.')}, []);
`

## 3. 컴포넌트가 업데이트 되었을때만 실행
- 함수의 두번째 파라미터로 검사하고 싶은 값 전달하고 해당 상태가 변했을때만 실행됨  

`
useEffect(()=>{console.log("업데이트 되었을때만 실행"), [name]})
`
