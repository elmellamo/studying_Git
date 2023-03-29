# Pull is not possible because you have unmerged files 에러

평소대로 vscode에서 바로 master로 동기화하고 깃에서 pull request를 하다가 아래와 같은 에러가 났다.
아마 이전에 같은 파일을 main에 merge했는데 같은 파일을 수정하니 에러가 난 것!
이유 불문하고, 이럴 때 에러를 고치는 방법은 다음과 같다.

<에러 내용>    
![image](https://user-images.githubusercontent.com/90952132/228544528-6c2d4755-6484-4396-9a59-ed76720594f4.png)   
![image](https://user-images.githubusercontent.com/90952132/228544580-f01cbf08-ac5d-4561-8443-9bf4a0be2eff.png)   
- This branch has conflicts that must be resolved
- Use the command line to resolve conflicts before continuing.
- error: Merging is not possible because you have unmerged files. hint: Fix them up in the work tree, and then use 'git add/rm <file>' hint: as appropriate to mark resolution and make a commit. fatal: Exiting because of an unresolved conflict.
  
---
<에러를 수정할 수 있는 방법!>
위의 깃에서 하라는 대로 하면 아래와 같은 에러상황을 파악할 수 있고,   
![image](https://user-images.githubusercontent.com/90952132/228546322-32bd5601-ec34-4225-897d-d24c25a0fced.png)
```
  git status
  git commit -am '커밋할 메세지입력'
```
![image](https://user-images.githubusercontent.com/90952132/228546561-fea8d76a-44c3-4ac0-85aa-ada8aa7eeaa6.png)

이렇게 하면 vscode 소스제어에서 커밋 칸에 **'변경내용 동기화'**라고 뜨게 된다.
이후, 원래대로 깃에서 merge를 하려고 하면 성공적으로 업로드!

![image](https://user-images.githubusercontent.com/90952132/228547273-b051345a-7e29-4f1f-a713-ae6024a97ea9.png)
