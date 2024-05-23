<h1>Docker 설치가이드</h1>

1. putty에서 root권한으로 접속
https://velog.io/@osk3856/Docker-Ubuntu-22.04-Docker-Installation
참고

2. pwd, whoami 명령어로 root 권한인지 확인

3. 우분투 시스템 패키지 업데이트
    > sudo apt-get update

4. 필요한 패키지 설치
    > sudo apt-get install apt-transport-https ca-certificates curl gnupg-agent software-properties-common
    
5. Docker의 공식 GPG키를 추가
    > curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

6. Docker의 공식 apt 저장소를 추가    
    > sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

7. 시스템 패키지 업데이트
    > sudo apt-get update

8. Docker 설치
    > sudo apt-get install docker-ce docker-ce-cli containerd.io

9. 도커 실행상태 확인
    > sudo systemctl status docker
 
![image](https://github.com/welcomeglory/Docker/assets/153584777/9eee13be-1331-42f9-a390-5cbce991f749)

active(running)이라고 나오면 docker가 돌아가고 있다는 뜻

빠져나올때는 q 나 ctrl+c

- docker run hello-world
  
![image](https://github.com/welcomeglory/Docker/assets/153584777/6479856c-9181-44a3-86d7-f911b6e288ca)

- docker -v => 설치된 도커버전확인
 













