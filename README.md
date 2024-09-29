## 처음 실행시 문제점 
### 해당 소스 받아 실행하면 DevopsStep1ApplicationTests 클래스의 test2() 메소드에서 오류 발생함 test2() 메서드 주석 처리해주세요. 그리고 gradlew build 실행하면 결과 파일(build/libs/*.jar) 생성됩니다 

## docker 이미지 파일생성 (Dockerfile이 있는 위치에서 아래 명령 실행) 
### docker build -t {본인의 docker hub 계정명}/devops_step1 .

##  Docker Hub 이미지 푸시
### docker push {본인의 docker hub 계정명}/devops_step1


## Docker hub에서 이미지 받아 실행 
 sudo docker run -d -p 80:8080 --name devops_step1 --restart always {본인의 docker hub 계정명}/devops_step1:latest
