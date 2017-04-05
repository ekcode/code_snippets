### git rm 되돌리기
```
git reset -- file
git checkout -- file
```

### .gitignore 적용
한번 커밋한 파일은 .gitignore에 설정하더라고 반영이 안된다.
```
git rm -r --cached .
git add .
git commit -m "fixed untracked files"
```
