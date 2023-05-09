# Docker
- 컨테이너 기반 오픈소스 가상화 플랫폼
- 파이콘 US 2013 '리눅스 컨테이너의 미래' 솔로몬 하이크(dotCloud→Docker Inc.)

**컨테이너 Container**
- 격리된 공간에서 프로세스가 동작하는 기술(가상화)
- 호스트 운영 체제에서 애플리케이션을 실행하기 위해 격리된 경량 사일로

**기존 가상화**
- OS 가상화, CPU 가상화(HVM) 이용(KVM), 반가상화(Xen) 
- → 클라우드 서비스 (OpenStack, AWS, Rackspace) 가상 컴퓨팅 기술의 기반 → 성능 문제

**리눅스 컨테이너 Linux Container**
- 프로세스 격리 (가볍고 빠르게 동작)
- CPU, 메모리 : 프로세스가 필요한 만큼만 추가 사용 → 성능 손실 ↓
- 새로운 컨테이너를 만드는데 걸리는 시간 : 1-2초(가상머신보다 빠름)

**기존 컨테이너(프로세스 격리)**
- Linux : cgroups(control groups), LCX(Linux Container / namespace 이용)
- FreeBSD : Jail
- Solaris : Solaris Zones
- Google : lmctfy (Let Me Contain That For You / 오픈 소스 컨테이너 기술)

**Docker**
- LXC 기반 → 자체적인 libcontainer(0.9ver) 기술 사용 → runC기술에 합쳐짐

**Docker와 VM(가상머신) 차이**

|기능|Docker|VM|
|:---:|:---:|:---:|
|구현 방식|하드웨어를 에뮬레이션하지 않고 독립된 환경에서 실행된 것처럼 보이는 특별한 제약이 가해진 프로세스 실행(컨테이너가 OS위에서 실행되는 다른 프로세스들과 정확히 같은 계층에서 실행)|OS나 하이퍼바이저 위에서 하드웨어를 소프트웨어로 에뮬레이션하고 그 위에 OS를 실행하고 그 위에 프로세스 실행|
