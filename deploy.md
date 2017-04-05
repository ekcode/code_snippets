* https://zeit.co/

### deploy git sub directory to heroku
```
git subtree push --prefix vanilla-server heroku master
```

### deploy to heroku by force
아래 방법이 있긴 하지만 명령어가 너무 길다.
```
git push heroku `git subtree split --prefix vanilla-sockjs master`:master --force
```

##### repository를 삭제하고 다시 push 하는 방법
https://github.com/heroku/heroku-repo 설치
```
heroku repo:reset -a vanilla-sockjs
```
