# Build and Run

`docker build -t jenkins:Net7 . && docker run -d -v jenkins_home:/var/jenkins_home -p 8080:8080 -p 50000:50000 --restart=on-failure jenkins:Net7`
