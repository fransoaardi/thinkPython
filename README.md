# thinkPython
thinkPython 정리 page입니다.

# fork
https://github.com/fransoaardi/thinkPython repo를 자신의 계정으로 fork합니다. 

# git 설치
git 을 사용하기 위해서는 설치가 필요하다.
* for windows
- https://git-scm.com/download/win

* 참고 
- http://freeprog.tistory.com/72 

# git bash
설치 후 git bash 프로그램을 실행하여 로컬에 저장할 경로를 생성한다.
```bash
 현재 C:\mygit 에 있다고 하면,
 $ mkdir test3
 C:\mygit\test3 디렉토리가 생성된다. 

 C:\mygit\test3 폴더로 이동시에, Git Bash 에서는 
 $ cd /c/mygit/test3   라고 입력해야함.
```

# git clone
본인의 로컬에 repo를 저장할 경로를 만들고 폴더를 우클릭하고 GitBash here 누른다
콘솔창에 다음과같이 입력합니다.
```bash
현재위치 C:\mygit 일때 (복사 붙여넣기는 shift insert 이용합니다)
$ git clone https://github.com/내id/thinkPython.git
하면 C:\mygit\thinkPython 디렉토리가 생성되고 내용이 다운받아져서 만들어진다.
``` 

# 본인의 차례때 내용 정리하기
- 본인의 repository ( github.com/내id/thinkPython ) 의 chapter로 들어갑니다.
- 파일을 생성하고 내용을 입력합니다. ( 주의 : .md 파일로 만들어야 markdown syntax가 적용됩니다 ) 
- 내용 정리 후에 아래의 Commit directly to the master branch. 와 commit changes 버튼을 클릭합니다.
- 회색글씨로 되어있는 제목과 설명 부분은 신경쓰지 않아도 됩니다.
- 작성 및 정리 완료 후, 첫 화면에 new pull request 버튼을 클릭합니다.
``` bash
base fork: fransoaardi/thinkPython base: master <- head fork: 내id/thinkPython compare: master 
```
아래의 file changed 내용을 비교하고, 변경 내용이 맞는지 확인하고, 
Create pull request 버튼을 클릭하고, 제목과 comment는 신경쓰지 않고 create pull request 버튼을 클릭합니다.

이로써 원본으로 merge가 완료되었습니다.

# 소스 pull, fetch upstream, merge upstream/master

* git pull
clone 해놓은 directory에 가서 git pull 하면 본인의 repository의 최신내용이 내려받아짐 
```bash
$ git pull
```
* git fetch upstream
```bash
$ git fetch upstream 
```
하면 upstream ( 함께 작업하고있는 페이지 ) 의 최신 내용이 내려받아짐

* git merge upstream/master
```bash
$ git merge upstream/master
하면 함께 작업하고 있는 페이지의 내용과 내가 작업하고 있는 내용이 합쳐짐(merge)
```
