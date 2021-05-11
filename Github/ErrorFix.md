# Github Error 정리 & 해결 방법


## Push 관련 에러

### error: src refspec master does not match any.
- 다음과 같은 에러 메세지가 나온다.
```
error: failed to push some refs to 'https://github.com/repo~'
```

- 원인 : 깃허브에서 pull 과정 없이 push 하는 경우 원래 내용을 삭제 및 수정 할 위험성이 있기 때문에 에러를 발생시키는 것이다.

- **해결 방법** : 새로운 Git Repository를 Init후 Push 하면 된다.
```
git init
git add -all
git commit -m "Commit msg"
<이름 이메일 입력 뜨면 입력> # git remote add origin "repo-url"
git push -u origin master  # origin 원격 저장소 master 브랜치 푸시
```
