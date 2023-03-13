# 디자인 시스템을 만들어보는 프로젝트

> 나만의 디자인 시스템을 만들어보는 두 번째 프로젝트입니다.

참고자료 : [creating your own react component library](https://blog.harveydelaney.com/creating-your-own-react-component-library/)

<br>

## What I Learned

### rollup plugin

- rollup plugin list site : https://github.com/rollup/plugins
- peerDepsExternal : 번들링하는 모듈의 peerDependencies를 자동으로 외부로 추출하여 번들링되지 않도록 한다. 즉, 플러그인을 사용하면 번들링 중에 peerDependencies를 자동으로 처리할 수 있으며, 이는 번들의 크기를 줄이고 종속성 관리를 개선하는 데 도움이 된다.
- resolve : 이 플러그인을 사용하면 Rollup은 모듈 번들링 시에 이러한 외부 종속성을 효율적으로 처리하여 번들의 크기를 최소화하고 실행 속도를 높일 수 있다. 이를 위해 @rollup/plugin-node-resolve 플러그인은 모듈 이름 해결을 통해 Node.js 모듈 시스템과 호환되도록 Rollup이 모듈을 가져오는 방법을 변경한다.
- rollup-plugin-terser : minify the Rollup bundle

<br>

### running rollup

- package.json에 rollup 실행에 대한 스크립트를 작성한다.

```js
"scripts": {
  "build" "rollup -c"
}
```

- `-c` flag는 rollup config 파일에 명시되어 있는 내용들을 수행하겠다는 의미가 된다.

<br>
