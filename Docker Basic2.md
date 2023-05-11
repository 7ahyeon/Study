# chroot(Chenge Root Directory)
- 루트 디렉터리 '/'를 변경
- 목적 : **디렉토리 경로를 격리**시킴으로써 데이터 유출 및 피해 최소화
- 이전 : chroot jail 환경 안에서 필요한 라이브러리 미리 준비해야함/복잡한 설정 방법/완벽한 가상환경X(많은 제약)
- **LXC(Linux Container) 등장** : 시스템 레벨의 가상화 : 리눅스 커널 레벨에서 제공되는 격리된 가상화 공간
- 가상머신VM과 달리 컴퓨터나 OS자체를 가상화하지 않음 : 컨테이너

# cgroups(Control Groups)
- CPU, 메모리, 보조기억장치, 네트워크 등의 자원을 할당하는 가상화 공간 제공
-  **namespaces** : process tree, 사용자 계정, file system, IPC 등을 격리 시켜서 Host OS와 완벽하게 격리된 공간 생성 


# LXC
- 리눅스 커널의 cgroups와 namespaces를 이용하여 격리된 공간
