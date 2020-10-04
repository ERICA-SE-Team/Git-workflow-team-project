----
## 💻 Git 워크플로우 진행 방식 (Forking flow)
----

#### 1. 프로젝트 팀 전체가 사용하는 중앙 원격 repository, 개인이 사용하는 개인 원격 repository, 개인이 사용하는 개인 로컬 repository를 아래의 이미지와 같이 구성함.
![Alt text](http://alldpublic.kr/SDP_Team/1.jpeg)

#### 2. 중앙 원격 저장소를 포크(fork)해서 자신만의 원격 저장소를 만든다.
 •중앙 원격 저장소를 복제한 저장소는 개인의 공개 저장소(remote repository) 역할을 함.
 •다른 개발자는 자신의 원격 저장소에 푸시할 수 없음(내려 받는 것은 가능)
![Alt text](http://alldpublic.kr/SDP_Team/2.jpeg)

#### 3. 프로젝트 참여자는 git clone 명령으로 로컬 저장소를 만든다.
'''
git clone [개인 원격 remote 저장소 주소]
'''
![Alt text](http://alldpublic.kr/SDP_Team/3.jpeg)

#### 4. 로컬 저장소와 중앙 원격 저장소, 개인 원격 저장소를 연결한다.
[로컬 저장소 - 중앙 원격 저장소 연결]
'''
$ git remote add center [중앙 원격 remote 저장소 주소]
'''
[로컬 저장소 - 개인 원격 저장소 연결]
'''
$ git remote add origin [개인 원격 remote 저장소 주소]
'''
![Alt text](http://alldpublic.kr/SDP_Team/4.jpeg)
