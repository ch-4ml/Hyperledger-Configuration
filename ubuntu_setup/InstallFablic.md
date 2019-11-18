# Fablic-Samples 설치

## Fabric-Sample 설치
### 아래 링크의 원본 링크 : https://raw.githubusercontent.com/hyperledger/fabric/master/scripts/bootstrap.sh
```cmd
$ sudo curl -sSL http://bit.ly/2ysbOFE | bash -s
$ vi ~/.profile
```
```vim
# 기존의 내용에서 추가되는 내용 ...:~/fabric-samples/bin;
export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin:~/fabric-samples/bin;
```
```cmd
$ source ~/.profile
``` 

## 설치 완료후 Fabric Sample 디렉토리 구조 탐색
``` cmd
tree 패키지가 설치 안되어있어 설치
$ sudo apt install tree
$ Tree -L 1 fabric-samples/
결과는 images 폴더의 Fabric-Samples 사진 참고
```

