# Hanyang Univ. ERICA Software Department </br>[Software Development Practice] Git workflow team project

### 🏫 팀소개  
-----
1. 이용현 (팀장 / 소프트웨어학부 / 2019034684)
2. 김문주 (소프트웨어학부 / 2019038277)
3. 김종언 (소프트웨어학부 / )
4. 이승섭 (소프트웨어학부 / 2019033936)
5. 최진영 (소프트웨어학부 / 2019095905)
6. 황순태 (소프트웨어학부 / )
-----  
### 📜 팀 워크플로우 개요 (Forking flow)  
-----
1. 모든 프로젝트 참여자가 `개인적인 로컬 저장소`와 `공개된 자신의 원격 저장소(하나의 중앙 원격 저장소를 각자가 Fork한 것)`, 즉 `두 개씩의 Git 저장소`를 가지는 방식이다.
2. 모든 코드 기여자가 하나의 `중앙 저장소에 푸시하는 것이 아니라, 각자 자신의 원격 저장소에 푸시`하고, `프로젝트 관리자만 다른 개발자들의 기여분을 중앙 원격 저장소에 병합할 수 있다`는 점이 가장 큰 특장점이다.
+ 소규모의 팀에서는 팀원 모두가 프로젝트 관리자가 되어 중앙 원격 저장소를 관리할 수 있다.
3. `아주 큰 규모의 분산된 팀에서도 안전하게 협업하기에 좋은 협업 방법`이다.
4. `오픈소스 프로젝트에서 많이 사용하는 방식`이다.

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