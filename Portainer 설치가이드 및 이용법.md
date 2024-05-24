<h1> Portainer 설치하기</h1>

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


    


    


    
