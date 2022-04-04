# dockertraining
 8  sudo apt-get update
    9  sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release
   10  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
   11  sudo apt-get update
   12  sudo apt-get install docker-ce docker-ce-cli containerd.io
   13  sudo docker run hello-world
   14  sudo usermod -a -G docker ubuntu
   15  cd dockertraining/
   16  docker run hello-world
   17  docker container run -d ubuntu
   18  docker container  ls -a
   19  docker search nginx
   20  docker pull nginx
   21  docker image ls
   22  docker history nginx
   23  docker history nginx:1.20
   24  docker image ls
   25  docker container run -p 8080:80 nginx 
   26  docker container run -d -p 8080:80 nginx
   28  docker container ls
   29  docker container ls -a
   30  docker container ls
   31  docker container run -d -p 8081:80 nginx 
   32  docker container ls
   33  curl localhost:8081
   34  curl localhost:8080
   35  docker container --help
   36  docker container ls
   37  docker conatiner stop --help
   39  docker container stop 7d20c8e6a242
   40  docker container ls
   41  docker container ls -a
   42  docker container start 7d20c8e6a242
   43  docker container ls -a
   44  docker container ls 
   45  docker container rm -f 7d20c8e6a242
   46  docker container ls -a
   47  docker container rm -f 89c2b7f7748c
   48  docker container ls -a
   49  docker container rm -f c46182f97545
   50  docker container rm -f 69721fdb8250
   51  docker container rm -f 67f8dc1c6514
   52  docker container rm -f d47fc5e69231
   53  docker container ls -a
   54  domcker image ls
   55  docker image ls
   56  docker image rm nginx:latest 
   57  docker image ls 
   docker rm -f $(docker container ls -a)
   docker run --name some-mysql -e MYSQL_ROOT_PASSWORD=password -d mysql
   docker container run -d --name sonam-mongo mongo
   docker container run -it --name web nginx bash
   docker container exec -it web bash
docker commit --help
  128  docker container ls
  129  docker commit container eef0297ec72a sonamvashishth/k8training1
  130  clear
  131  docker container ls
  132  docker container commit --help
  133  docker commit eef0297ec72a sonamvashishth/k8training1
  134  docker image ls
  135  docker push sonamvashishth/k8training1:latest
  136  docker login
  137  docker push sonamvashishth/k8training1:latest

  39 docker container ls
140 docker run -it --name test1 ubuntu bash
141 docker container ls -a
142 docker container start 73
143 docker commit 7313bfc7a641 myimage
144 docker image ls
145 docker container run -it myimage bash
146 clear
147 docker container ls
148 docker container ls -a
149 docker container start 41f662b8e2c4

100  docker container logs ee
  101  docker container logs --help
  102  clear
  103  docker container inspect ee
  104  docker container stats ee
  105  history
  106  docker container top ee

