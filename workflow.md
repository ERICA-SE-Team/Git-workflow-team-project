#### 5. 새로운 기능 개발을 위해 격리된 branch를 만든다.
```
$ git checkout -b [branch name]

# 위의 명령어는 아래의 두 명령어를 합한 것
$ git branch [branch name]
$ git checkout [branch name]
```
![Alt text](http://alldpublic.kr/SDP_Team/6.jpeg) 

#### 6. 로컬 저장소의 커밋 이력을 자신의 원격 저장소(remote repository)에 푸시한다.
```
$ git commit -a -m "Write commit message"

# 위의 명령어는 아래의 두 명령어를 합한 것
$ git add . # 변경된 모든 파일을 스테이징 영역에 추가
$ git add [some-file] # 스테이징 영역에 some-file 추가
$ git commit -m "Write commit message" # local 작업폴더에 history 하나를 쌓는 것
```  
![Alt text](http://alldpublic.kr/SDP_Team/7.jpeg) 

#### 7. 프로젝트 관리자(소규모 팀에서는 모두가 관리자가 될 수 있음)에게 자신의 기여분을 반영해 달라는 풀 리퀘스트를 던진다.
![Alt text](http://alldpublic.kr/SDP_Team/8.jpeg) 
