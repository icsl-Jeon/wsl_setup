# wsl_setup 


## Intial setup ([ref](https://holeeman.github.io/windows/WSL-2%EC%97%90%EC%84%9C-%EB%A6%AC%EB%88%85%EC%8A%A4-GUI-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8-%EC%8B%A4%ED%96%89/))

### In window 
  * Install vcsrv
  * xLaunch `-ac` and uncheck Native Opengl 
  * [Register xlaunch startup program ](https://hoodiejun.tistory.com/13) 
  * Then, launch [Window Terminal](https://wslhub.com/wsl-firststep/devsetup/multiplexer/) 


### In WSL Ubuntu 
```
sudo apt-get update

# in ~/.bashrc 
export DISPLAY="`grep nameserver /etc/resolv.conf | sed 's/nameserver //'`:0"
export LIBGL_ALWAYS_INDIRECT=0 


echo 'set bell-style none' >> /etc/inputrc

```


## Using [wslg](https://docs.microsoft.com/ko-kr/windows/wsl/tutorials/gui-apps) (gui ) without x-forwarding 
* Register window insider program and update [window OS](http://blog.naver.com/PostView.nhn?blogId=dev4unet&logNo=222324541781&parentCategoryNo=&categoryNo=&viewDate=&isShowPopularPosts=true&from=search)
* Install vGPU of [nvidia](https://developer.nvidia.com/cuda/wsl/download)

