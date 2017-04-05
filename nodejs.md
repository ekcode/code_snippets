### package.json
패키지 설치하고 package.json에도 dependency를 추가한다.

```
npm install moment --save
```

yarn은 --global 옵션을 붙히지 않으면 기본적으로 local repository 에 의존성이 추가됨

```
yarn add moment
```

### yarn build
파일 수정되면 자동으로 빌드하기

https://github.com/joh/when-changed
```
when-changed -v1 public/javascripts/chat-core.ts yarn build
```

