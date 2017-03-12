### less 설정

```
npm install less-middleware --save
```

app.js에 아래 코드를 추가

```
app.use(lessMiddleware(__dirname + '/public'));  //[1]
app.use(express.static(path.join(__dirname, 'public'))); //[2]
```

[2]번 앞쪽에 [1]을 설정해야 auto compile 된다.


