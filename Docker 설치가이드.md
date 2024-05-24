<h1>Docker 설치가이드</h1>

<h3>1. putty에서 root권한으로 접속</h3>

    sudo - root

![image](https://github.com/welcomeglory/Docker/assets/153584777/26fe0271-affb-4096-806f-f902aa09aa1c)
    

<h3>2. root 권한인지 확인</h3>

![image](https://github.com/welcomeglory/Docker/assets/153584777/f2a8a0b0-2fc3-4ca3-a55b-e5f2d68c4ee8)


<h3>3. 우분투 시스템 패키지 업데이트</h3>

    sudo apt-get update

![image](https://github.com/welcomeglory/Docker/assets/153584777/f4881ffe-c319-4cd4-b93b-a0374a3f9e96)


<h3>4. 필요한 패키지 설치</h3>

     sudo apt-get install apt-transport-https ca-certificates curl gnupg-agent software-properties-common

![image](https://github.com/welcomeglory/Docker/assets/153584777/1b5d532e-3399-4d8f-8491-54d9540b66ff)

    
<h3>5. Docker의 공식 GPG키를 추가</h3>

     curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

![image](https://github.com/welcomeglory/Docker/assets/153584777/f4fda724-bbf8-4a2a-b2b1-2a6590cb54ba)


<h3>6. Docker의 공식 apt 저장소를 추가</h3>    

     sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
    
![image](https://github.com/welcomeglory/Docker/assets/153584777/7becb15a-69cf-4a0e-a1c3-34b200d7ef75)


<h3>7. 시스템 패키지 업데이트</h3>

     sudo apt-get update
     
![image](https://github.com/welcomeglory/Docker/assets/153584777/4e58c3f1-cb96-4b89-bee7-f5622c38f749)


<h3>8. Docker 설치</h3>

     sudo apt-get install docker-ce docker-ce-cli containerd.io

![image](https://github.com/welcomeglory/Docker/assets/153584777/cc48ccb8-0093-4f2d-98d0-487b11980a44)

![image](https://github.com/welcomeglory/Docker/assets/153584777/b621283d-4158-4b3b-84a1-fbeb78484b75)



<h3>9. 도커 실행상태 확인</h3>

     sudo systemctl status docker
 
![image](https://github.com/welcomeglory/Docker/assets/153584777/9eee13be-1331-42f9-a390-5cbce991f749)

     active(running)이라고 나오면 docker가 돌아가고 있다는 뜻, 해당 명령어에서 빠져나올때는 q 나 ctrl+c

<h3>10. 도커 실행</h3>

    docker run hello-world
  
![image](https://github.com/welcomeglory/Docker/assets/153584777/6479856c-9181-44a3-86d7-f911b6e288ca)

<h3>11. 설치된 도커버전확인</h3>

     docker -v 

![image](https://github.com/welcomeglory/Docker/assets/153584777/d264c11f-b0b1-48b9-90ac-eeeecbf5ea81)

     
