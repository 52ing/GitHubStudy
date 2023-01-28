

[git Error]
mashup-todolist % git push origin master
error: src refspec master does not match any
깃헙에서 pull 없이 push 할 경우 기존내용 삭제 문제가 생길 수 있음.

   1. git init
   2. git add . 
   3. git commit -m "message"
   4. git remote add origin 'git url'
   5. git push -u origin master

이 외에 Master Branch가 없엉서 발생하는 오류는?
   1. git checkout -b 'master'
   2. git push origin master

[VSCode 초기화 안나오는 현상]
   1. 소스 제어탭에 1k or 5k 뜨면서 너무 많은 변경이 감지.. 라고 뜸
        a. root repository > git rev-parse --showtoplevel
        b. 대부분 /Users/사용자이름 경로가 나옴
        c. 해당 경로로 이동 후 ls -a or ls 명령어를 사용하여 .git 폴더 있는지 확인.
        d. 폴더 있을 경우 rm -rf .git 명령어 사용 하여 삭제 하고 다시 접속하면 초기화 버튼 나오는것을 볼 수 있다.!
    2. git clean 도 가능하지만 파일, 폴더가 모두 날라 갈 수 있으니..ㅠ
