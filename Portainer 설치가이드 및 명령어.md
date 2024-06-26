![image](https://github.com/welcomeglory/Docker/assets/153584777/c64cc9a3-00a1-44a8-8405-54aaf5f1bf45)<h1> Portainer 설치하기</h1>

<h3> 1. Portainer 디렉토리 파일 생성 </h3>

    mkdir -p /data/portainer

<h3> 2. Portainer 실행하기 </h3>

    docker run --name portainer -p 9000:9000 -d --restart always -v /data/portainer:/data -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ce

![image](https://github.com/welcomeglory/Docker/assets/153584777/bafc8a73-9eea-4c5e-a1f0-80d33c161b5b)

<h3> 3. vm virtualbox에서 포트 포워딩 </h3>

    - 실행 중인 ubuntu 설정에 접속
    - 네트워크 -> 고급 -> 포트 포워딩
    - 호스트 포트, 게스트 포트는 9000으로 입력하고 나머지는 동일

<h3> 4. Portainer 접속 </h3>

![image](https://github.com/welcomeglory/Docker/assets/153584777/43211f7b-ba9f-4022-86dd-532b851ee5a3)

<h3> 5. 컨테이너, 이미지 연결 상태확인 </h3>

![image](https://github.com/welcomeglory/Docker/assets/153584777/29f23acd-c9b3-4158-bc15-e18c8c7039c1)

<h3> 6. 이미지 검색 </h3>

    docker search tomcat

![image](https://github.com/welcomeglory/Docker/assets/153584777/9c7c4da9-0a6c-4fde-a0e2-45d2b103e9d5)

    https://hub.docker.com/
    에서 받아올수 있음

<h3> 7. 이미지 다운로드 </h3>

    docker pull nginx

![image](https://github.com/welcomeglory/Docker/assets/153584777/66f0b049-7884-4bb8-a92c-992f8d1471c5)
    
<h3> 7. 이미지 목록 출력 </h3>

    docker images

<h3> 8. 컨테이너 만들기 </h3>

    docker run -d --name {컨테이너 이름} -p : {이미지 명}

    run : 이미지를 가지고 컨테이너를 만들고 구동하는 명령어.
    -d : 컨테이너를 만들면 백그라운드에서 계속 구동하게 하는 옵션. ('데몬'이라고 읽는다.)
    --name : 컨테이너의 이름을 지정해주는 옵션. (따로 지정해주지 않으면 무작위로 이름이 생성된다.)
    -p : host port number와 conatiner의 port number를 연결해주는 옵션.

![image](https://github.com/welcomeglory/Docker/assets/153584777/0632f7f9-75b5-40a4-97f7-7688891b9f41)

    이미지명은 portainer에 이미지에 Tags 확인

 ![image](https://github.com/welcomeglory/Docker/assets/153584777/2aceb144-10c9-43a5-94af-ae71a31a38a2)


 ![image](https://github.com/welcomeglory/Docker/assets/153584777/8a5bac1f-3ba4-4980-a89b-8b43dc520b21)


    docker run -d -p 49161:1521 oracleinanutshell/oracle-xe-11g
![image](https://github.com/welcomeglory/Docker/assets/153584777/c05dc4df-c82a-4e11-9fb7-75df36ff7684)

https://hub.docker.com/r/oracleinanutshell/oracle-xe-11g

    docker hub(search) -> pull(image download) -> run(build container - create program) 

![image](https://github.com/welcomeglory/Docker/assets/153584777/e23ec8d1-f2ab-4ba1-b2c8-8618a7730f7c)


![image](https://github.com/welcomeglory/Docker/assets/153584777/ec54f2cb-c8d0-49c9-bd2c-378e5d69ee76)

    sqlplus

    user-name: system
    password: oracle


![image](https://github.com/welcomeglory/Docker/assets/153584777/bdf3070b-718f-4b17-afe8-58d09c40d1d5)

    docker exec -it 컨테이너이름 bash => 컨테이너 안에 BASH쉘을 실행시켜라.



    컨터이너 하나하나가 리눅스기반 OS를 가짐(ME는 우분투 사용)

    리눅스 위에 어플리케이션(예:오라클)이 돌아가는 구조임



    

    











    


    
