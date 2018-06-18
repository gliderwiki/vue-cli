# vue-cli

> vue study sample

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build


# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test

```

For detailed explanation on how things work, consult the [docs for vue-loader](http://vuejs.github.io/vue-loader)


# Vue init project with cli 


``` bash
# 설치 : sudo npm install vue-cli -global

vue init webpack : 고급 웹팩 기능을 활용한 프포젝트 구성방식 
vue init webpack-simple : 웹팩 최소 기능 (빠른 프로토타이핑)
vue init simple : 최소 뷰 기능만 들어간 HTML 파일 1개 생성 
vue init pwa : 웹팩 기반의 프로그래시브 웹 앱  지원 
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


## VueJS 주요 개념 

#### 라이프사이클 

![VueJS 라이프 사이클](https://kr.vuejs.org/images/lifecycle.png)

1. 이벤트와 라이프 사이클 초기화 작업
1. 데이터를 감시할 수 있도록 변경 
1. 템플릿 마운트 
1. 데이터 변경시 템플릿 업데이트 
1. 데이터와 이벤트 감시 취소 
1. 라이프 사이클 종료 

### 인스턴스

`인스턴스 선언` 
```javascript
new Vue({
  // 옵션이나 컴포넌트 설정 
  // 루트 컴포넌트로 Vue 클래스를 초기화한 최상위 객체 
});
```
```javascript
var vm = new Vue({
  // 옵션이나 컴포넌트 설정 
});
```

### 컴포넌트 
개발자가 HTML 태그 방식으로 UI를 덧붙일 수 있게 기능을  제공.
  
`컴포넌트 선언`

```javascripto
Vue.component(<컴포넌트 이름>, {
  // 옵션
});
```

`지역 컴포넌트 선언`

```javascripto
new Vue({
  // 초기화 옵션 
  components : {
    <컴포넌트 이름> : <컴포넌트 옵션>
  }
});
```

- 지역 컴포넌트는 상위 컴포넌트의 템플릿에서만 사용 가능 
.
