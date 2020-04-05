# 우분투 설정 추가 및 변경

## vim 업데이트
``` cmd
$ sudo apt-get install vim
```
## docker 설치
```cmd
$ sudo apt install docker.io
$ sudo apt install docker-compose
$ sudo apt install software-properties-common
현재 접속중인 사용자에게 권한 부여
$ sudo usermod -aG docker $USER
$ reboot
재부팅 이후
$ docker --version
Docker version 18.09.7, build 2d0083d
$ docker
```

## curl 설치
``` cmd
$ sudo apt-get install curl
```

## build-essential 설치 (윈도우 개발자 도구 개념)
``` cmd
$ sudo apt-get install build-essential libssl-dev
```
## nvm 파일 설치
``` cmd
$ curl -sL https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh -o install_nvm.sh 
$ bash install_nvm.sh
$ source ~/.profile
$ nvm install v8.11.1
$ node -v
v8.11.1
$ npm -v
v5.6.0
```

## GO 언어 설치
```cmd
go 언어 압축 파일 저장
$ curl -O https://storage.googleapis.com/golang/go1.11.2.linux-amd64.tar.gz
go 언어 압축 해제
$ tar -xvf go1.11.2.linux-amd64.tar.gz
go 언어 폴더 이동
$ sudo mv go /usr/local
링크 생성
$ sudo ln -s /usr/local/go/bin/go /usr/local/bin/go
환경변수 적용
$ vi ~/.profile
```
아래 내용 추가
``` vim
export GOPATH=$HOME/go
export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin
```
터미널에서 설정
``` cmd
$ source ~/.profile
```

## Python, GIT 설치
``` cmd
$ sudo apt install -y python
$ python --version
Python 2.7.15+
$ sudo apt install -y git
$ git --version
git version 2.17.1
```

## 최종 설치된 프로그램 확인
``` cmd
$ python --version
Python 2.7.15+
$ git --version
git versioon 2.17.1
$ docker --version
Docker version 18.09.7, build 2d0083d
$ docker-compose --version
docker-compose version 1.17.1, build unknown
$ go version
go version go1.11.2 linux/amd64
$ node -v
v8.11.1
$ npm -v
5.6.0
```
[다음 과정(패브릭 설치)](./InstallFabric.md)
