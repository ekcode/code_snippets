### github의 내 repository 리스트 받아오기 및 clone
```
USER=ekcode; curl -s "https://api.github.com/users/$USER/repos?per_page=1000" | grep -o 'git@[^"]*'
USER=ekcode; curl -s "https://api.github.com/users/$USER/repos?per_page=1000" | grep -o 'git@[^"]*' | xargs -L1 git clone
```
### Changing author info
https://help.github.com/articles/changing-author-info/

### git config
git config user.name "Ickhyun Kwon"
git config user.email "ekcode@icloud.com"

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
