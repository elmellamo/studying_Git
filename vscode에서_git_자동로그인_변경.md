# VS CODE에서 깃 자동로그인 변경하기
# VS CODE에서 깃 로그아웃하고 로그인 새로하기
# 에러 You do not have permission to push to on Github. Would you like to create a fork and push to it instead

stackoverflow에 보면
- In VScode sign out by clicking on the person icon on the left down on the screen and close VScode.
- After this go to your "Control Panel" in "Windows OS and search for " Credential Manager" and choose "Windows Credentials".
- Below you will see a list called "Generic Credentials", remove everything with the name "Git" and "Github". (this will remove your logins)

이렇게 하라고 하는데, 한국말로 도대체 무엇인지 모를 수 있다.

1. 제어판 > 자격증명관리자 검색 > Windows 자격 증명 > 일반 자격 증명
2. 일반자격증명에서 git이 들어간 거명 다 삭제한다.
3. VS CODE에 다시 들어가서 사람 모양 있는 '계정'에 들어간다.
4. 로그아웃한다
5. 로그인하여 설정 동기화 를 누른다.
6. 설정 동기화 맨 윗창에 Github로 로그인을 누른다.
7. 새롭게 로그인하려는 계정을 웹에서 입력하고 동기화 누른다.
8. 터미널 창에서 우선 현재 기존에 연결되어 있는 깃 계정이 무엇인지 확인한다.
'''
git config --list
'''
9. 그럼 여기서 user.name과 user.email을 살펴본다. 나올 때까지 엔터를 친다. 확인하였으면 q를 누른다.
10. 바꾸고픈 계정으로 다시 수정한다.
'''
git config --global user.name "닉네임"
git config --global user.email "이메일"
'''
11. 다시 현재 기존 연결되어 있는게 맞게 연결되어 있는지 확인한다.
'''
git config --list
'''


-Contrl Panel == 제어판
-Credential Manager == 자격증명관리자
-Generic Credentials == 일반 자격 증명

##참고링크
<https://stackoverflow.com/questions/68080637/you-do-not-have-permission-to-push-to-on-github-would-you-like-to-create-a-fork>
<http://conanoc.egloos.com/6345602>
