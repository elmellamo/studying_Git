# vscode에서 깃 commit 날짜 변경하기

이미, 깃에 어떤 파일을 업로드했다는 전제 하에, 
1. 깃 bash 열기
2. 아래 코드 쓰기
```
git commit --amend --no-edit --date "$(date)"
git commit --amend --no-edit --date "Thur 16 Mar 2023 20:19:19 KST"
git rebase --continue
git push -f origin master
```

![image](https://user-images.githubusercontent.com/90952132/225848392-65467d6a-599f-4b10-9b36-ac6fdd733cba.png)
![image](https://user-images.githubusercontent.com/90952132/225848452-c499ab60-d7a0-4de5-b28f-e6b77275ceb7.png)
![image](https://user-images.githubusercontent.com/90952132/225848465-0c0830be-5b05-4ebf-b116-b0425965840f.png)


---
<참고링크>   
<https://deeprun.tistory.com/221>
