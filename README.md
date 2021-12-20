# Cloud-Basic

## 클라우드 컴퓨팅
클라우드 컴퓨팅 개념

대형 전력회사에서 전기를 받아쓰듯이 중앙집중화 된 대형 데이터센터에서 서비스를 받고, 소프트웨어 프로그램들도 인터넷 망을 통해서 자유롭게 빌려 쓴다. IT 자원을 구매하거나 소유할 필요 없이, 필요한 만큼 사용료를 주고 쓰는 개념이 바로 "클라우드컴퓨팅" 이다. -니컬러스  카-

배경 및 필요성

새로운 디지털 시대는 클라우드컴퓨팅이 중심이 될 것이다. -빌 게이츠

미래 인터넷 경제의 최대 화두는 클라우드컴퓨팅의 가속화에 있다. -에릭 슈미츠

사용자 편의성, 서비스 연계성, 자원의 공동활용

경제성

- 실제 자원 활용률 : 5~20%
- 특정 시점에서만 활용률이 높음
    - 스포츠 시즌 : 영상 스트리밍
    - 쇼핑 시즌 : 초콜릿 쇼핑몰(예: 발렌타인데이/빼빼로데이)

오버 프로비저닝 - 서버 활용률이 낮은 경우

언더프로비저닝 - 서버 활용률을 넘어서 사용할 경우

클라우드 컴퓨팅을 이용해서 서버활용률을 적절하게 조정한다

데이터 센터

- 수만개의 서버를 묶어둔 것
- 자원의 활용이 적절한지 감시하고 문제가 생겼을 시 대응한다
- 데이터센터의 온도가 올라갈 경우 기능저하, 장애가 나올 수 있기 때문에 적정온도 유지

제공 유형에 따른 분류

IaaS - 인프라 제공 서비스 : 프로세싱 파워, 서버, 네트워크, 가상화 및 OS와 같은 기본적인 컴퓨팅 자원을 제공하는 클라우드 서비스

PaaS - 플랫폼 제공 서비스 : 클라우드 컴퓨팅 환경을 통해 어플리케이션 개발 플랫폼을 제공하는 서비스. 단말을 위한 API를 제공하거나 다양한 이기종 간의 단말에서의 개발 환경을 제공

SaaS - 소프트웨어 제공 서비스 : 별도의 전용 소프트웨어를 제공하여 소비자가 단지 어플리케이션만을 사용하고 어플리케이션이 실행되는 운영체제, 하드웨어 또는 네트워크 인프라는 제어하지 않는 클라우드 서비스

사용 유형에 따른 분류

Public 공용클라우드 : 제3의 회사 (예 : Amazon AWS, Microsoft Azure, Google Cloud, KT uCloud, NAVER Cloud, TOAST) 에서 제공되는 클라우드를 인터넷으로 접속해 사용

Private 사설 클라우드 : 인터넷을 통하지 않고 사내 등에 직접 하드웨어 구입 후 클라우드를 구축, 네트워크 속도, 보안 및 법적인 문제에 따라 사용하는 경우가 많음

Hybrid 하이브리드 클라우드 : 공용 클라우드와 사설 클라우드의 적절한 조합

공용 클라우드 예

Amazon EC2

- 자사 컴퓨팅 자원을 인터넷을 통해 제공하여 초기 시장 선도
- '06년 EC2(Elastic Computer Cloud)를 출시
- 전 세계 대상 온라인 서점 서비스에 사용되는 유휴 서버 자원들을 가상화시켜 서비스를 제공

Microsoft Azure

- 2009년 PaaS를 중심으로 정식 서비스를 시작, 현재는 2018년 기준, 54개 데이터센터를 기반으로 IaaS, PaaS, SaaS 모두를 제공

Google Cloud

- 1992년 시작된 검색 엔진을 기반으로 다양한 분산, 클라우드 컴퓨팅 기술을 개발 및 선도

사설 클라우드 예

- 기업/회사 내 데이터센터를 구축하여 직접 클라우드를 관리
- 사내 클라우드 구축 + 공용 서비스 인프라를 위해 사용

클라우드 컴퓨팅 : 클라우드 가상화

가상 자원은 클라우드 컴퓨팅을 탄생하는 데 있어 핵심 기술에 해당합니다

컨테이너 & 베어베탈

- 가상 머신은 하이퍼바이저 위에서 별도의 운영체제와 함께 동작합니다
- 컨테이너는 공통된 운영체제(커널)를 기반으로 독립적으로 응용프로그램을 실행합니다
- 베어메탈은 가상화/컨테이너 기반이 준비되어 있지 않은 물리 서버로, 베어메탈에 가상화/컨테이너 서비스를 구축하여 클라우드 컴퓨팅 서비스를 만듭니다

프로그래머블 / 소프트웨어 정의 인프라

- 원하는 때 원하는 만큼 자원을 확장하거나 줄이는 과정을 수동이 아닌 프로그래밍 가능한 인프라 환경을 통해 자동으로 이뤄집니다
- 인프라 전체를 소프트웨어 기반으로 제어하는 환경을 소프트웨어 정의 인프라/소프트웨어 정의 데이터센터 등 용어로 이야기하기도 합니다

## 가상화
가상화란

- 가상화란 컴퓨터 자원의 추상화(abstract)를 일컫는 광범위한 용어
- 간단하게는 어떤 사물을 물리적인 것이 아닌 가상으로서 생성하는 과정으로, 컴퓨터, 운영체제, 스토리지, 어플리케이션, 네트워크 등에 적용이 가능함
- 그렇다 하더라도, 가상화의 핵심은 서버 가상화

가상화의 기원

- 가상화의 기원은 최초 1960년대 IBM 메인 프레임에서 파티셔닝을 통해 서로 다른 업무를 동시에 실행하여 대용량 컴퓨팅 자원을 효율적으로 활용한 것이 그 효시로써, 컴퓨팅 기술의 발전에 따라 이를 x86 플랫폼 상에서 구현할 수 있게 된 것이 현재의 x86 서버 가상화
- 단순히 서버 자원 만을 공유하던 기존의 가상화는 데이터 센터 인프라 자원(스토리지, 네트워크, 보안, 재해복구)으로 그 범위를 넓혀 이제는 데이터 센터 자체에 대한 가상화(SDDC)가 진행중
- 과거 가상화되지 않은 서비스를 도입하는데 걸리는 시간은 현재 가상화를 통해 큰폭으로 단축됨

하이퍼바이저 - Native & Hosted

- 서버 가상화에서 가상 머신의 생성 및 관리를 가능케하는 소프트웨어

Native(bare metal)

하드웨어에 직접 설치되어 호스트에서 발생하는 오버헤드를 감소시킴

Hosted

기존 운영체제에서 동작하는 일반 프로그램과 같은 레벨에서 실행 게스트 OS의 종류에 제약이 적음

TYPE 1

물리 서버 위에 하이퍼바이저를 구동시켜 여러개의 가상 서버를 만드는 타입

TYPE 2

물리 서버 위에 운영체제를 구동시키고 그 위에 여러 개의 하이퍼바이저를 실행시켜 여러 가상서버를 만드는 타입

전가상화

하드웨어를 모두 가상화 한 것

Guest OS를 아무런 수정 없이 이용이 가능

반가상화

하드웨어를 완전하게 가상화하지 않음

Guest OS가 직접적으로 하드웨어를 제어할 수 없음. OS 코드 수정 필요

서버 가상화를 위한 하드웨어 지원

하드웨어 지원 가상화

- 가상화 솔루션의 VMM(Virtualization Machine Monitor = Hypervisor)의 구동에서 CPU overhead를 줄이기 위한 기술
- 인텔/AMD는 VMM 기술에서 사용되는 가상화 구현 관련 명령어 패턴을 하드웨어 기술로 구현함

참고 : CPU Ring 구조

- 전통적으로 Ring 0번에서 3번까지 총 4개가 잇는데, 0을 관리자 모드, 3을 일반 모드로 사용
- 가상화를 위해서는 물리 CPU에서 추가적인 Ring 계층 사용이 필요한데, 소프트웨어적으로 Ring 1을 하나 더 사용하면 성능이 저하됨
- CPU 하드웨어 내부적으로 계층을 처리해주면 속도가 빨라짐

인텔 CPU : Intel VT

- Intel VT-x, VT-l

: CPU 단에서 제공되는 기술이며, 인텔의 가상화 기술 중 x86서버에 탑재되는 Xeon processor에 대한 기술을 VT-x라고 하며, 유닉스 서버용 프로세서인 Itanium processor에 대한 기술을 Vt-i라 부름

- Intel VT-d

: Virtualization Technology for Directed I/O 를 의미하며, I/O가 사용하는 DMA 주소를 물리 서버와 VM에 매핑하는 것을 하드웨어로 구현한 것

- Intel VT-c

: Virtualization Technology for Connectivity를 의미하며, 가상화 환경에서 네트워크 카드의 성능을 향상시킴

AMD CPU : AMD-V

- 64bit x86-architecture에 대한 AMD의 가상화 기술을 AMD-V라 부름
- AMD-V는 애슬론 64 및 튜리온 64 X2, 옵테론 2세대 및 페넘 이후의 프로세서에 존재함
- AMD는 입출력 메모리 관리 장치(IOMMU) 기술을 AMD-V에 추가함

하이퍼바이저 종류

- 상용 : VMWare Workstation, ESXi, Microsoft Hyper-V, Citrix XenServer 등
- 오픈소스 : VirtualBox, Xen, KVM 등

서버 가상화와 클라우드

- 서버 가상화는 클라우드 인프라를 만드는 기반 기술
- 클라우드 인프라를 실제 만들려면, "네트워크"도 필요합니다
- 네트워크 가상화는 가상 머신들이 사용하는 네트워크 대역을 직접 만드는 것을 가능하게 하는 기술입니다

## 네트워크 가상화
서버 가상화 & 네트워크 가상화

- 클라우드 인프라를 실제 만들려면, "네트워크"도 필요합니다.
- 네트워크 가상화는 가상 머신들이 사용하는 네트워크 대역을 직접 만드는 것을 가능하게 하는 기술입니다
- 다양한 기술이 있는데 (VLAN, VXLAN, GRE, NVGRE, STT ...) 여기서는 VLAN을 살펴볼 예정입니다.

서버 가상화는 가상서버를 실제 물리서버처럼 가상화 시키는 것

네트워크 가상화는 하나의 물리네트워크가 있는데 여러 개의 가상 네트워크를 만들어서 독립적으로 사용할 수 있도록 만드는 것

네트워크 가상화 환경에서의 IP 대역

- 한 물리 네트워크에서 두 가상 네트워크가 가상화가 되어 있는 상태
- 가상 네트워크 A 내에 있는 IP주소는 동일 가상 네트워크이므로 통신 가능
- 가상 네트워크 A와 B가 서로 통신하려고 하는 경우 다른 가상 네트워크 이므로 통신 불가능

네트워크 가상화 기술 : VLAN 소개

- 네트워크 데이터 링크 계층 내 특정 필드를 이용하여 물리 스위치 장비에서 서로 다른 "네트워크"처럼 분리하여 관리
- 공유기와 같은 장비는 스위치라고 할 수 있음
- 예를 들어서 VLAN10과 VLAN20과 통신을 할려 하면 차단할 수 있음 (학생과 선생님) 802.1Q
- VLAN이 적용되지 않은 스위치 (모든 포트들을 통해 서로 네트워크 통신 가능
- VLAN이 적용된 스위치 (VLAN 번호가 같은 것끼리 서로 네트워크 통신이 가능하다)

참고 : 물리 스위치 VLAN 설정

VLAN 설정 명령어 CLI (예 : Cisco 장비)

- VLAN 번호 생성 명령어
- VLAN에 이름 부여
- 스위치 포트를 VLAN 사용 가능한 모드 (access 모드)로 변경
- 해당 스위치에 VLAN 번호 부여

VLAN 설정 화면 GUI (예 : HP 장비)

VLAN : Trunk 모드에 대해 알아보자

- Trunk 모드 비활성화일 때 : 스위치3 입장에서 VLAN 번호마다 포트 번호를 필요로 함
- Trunk 모드 활성화일 때 : 스위치 1, 2에 해당하는 포트만 있으면 사용 가능 (VLAN 번호 그대로 전달)
- 하나만 설정해도 된다는 장점이 있지만 트래픽이 많아지면 많은 부하가 걸림 → 네트워크 설비를 어떻게 구성하느냐가 중요

OpenvSwitch

- Linux 환경에서 가상의 "네트워크 스위치" 장비를 구현

: VLAN 등 연결 가능한 포트 및 네트워크를 구성 가능한 스위치로 사용 가능

: 클라우드 환경에서 오픈 소스 기반으로 구축시 소프트웨어 기반 스위치로 주로 활용

## 오픈스택
OpenStack 이란?

- 클라우드 환경에서 컴퓨팅 자원과 스토리지 인프라를 셋업하고 구동하기 위해 사용하는 오픈 소스 소프트웨어 프로젝트의 집합

OpenStack에 대한 다른 정의들

- OpenStack은 공용(Public) 클라우드와 사설(Private) 클라우드 구축을 가능하게 하는 오픈소스 소프트웨어
- OpenStack은 서버, 스토리지, 네트워크들과 같은 자원들을 모두 모아, 이들을 제어하고 운영하기 위한 클라우드 Operating System
- OpenStack은 오픈 소스를 기반으로 클라우드를 구축하고 운용하고자 하는 오픈 소스 개발자, 회사, 사용자들이 주축이 되어 발전하는 커뮤니티
- IaaS 형태의 클라우드 컴퓨팅 오픈소스 프로젝트로 컴퓨팅, 스토리지, 네트워킹 자원을 관리하는 여러 개의 하위 프로젝트들로 이루어짐

OpenStack의 성장

- 빠른 글로벌 오픈소스 커뮤니티 성장세

OpenStack : Production 환경

- 코어 ≥ 5,000,000 개가 Production 환경에서 사용 중 (2017년 4월 통계)
- 전체 OpenStack 환경 중 2/3 (그 외 : 개발용, QA용, PoC...)

OpenStack을 사용하는 곳

- 국내 : KBS, 현대자동차, 넷마블, 카카오 등
- 월마트, 이베이, 페이팔, 하버드대학교, MIT

OpenStack 역사

- OpenStack 핵심 컨트리뷰터
- 초기 : Rackspace & NASA
- Rackspace : OpenStack의 Object Storage라고 하는 "Cloud Files" 부분 플랫폼을 개발하는데 기여하기 시작
- NASA : 기존 "Nebula" 플랫폼을 발전시켜 컴퓨팅 자원 플랫폼을 개발하는 데 기여
- 2012년 5월 : NASA와 OpenStack 관계 종료
- 2012년 9월 : VMWare사 가 OpenStack foundation에 가입
- 그리고, 많은 회원사 & 참여자들이 참여하고 있음

OpenStack 릴리즈

- 6개월 주기로 릴리즈 발표
- 릴리즈 : 개발자 서밋 & 미팅에 맞추어 계획됨
- 2016년까지 OpenStack Summit에서 개발자 회의가 진행됨 (OpenStack Design Summit)
- 2017년부터 PTG (Project Team Gathering)이라는 이름으로 별도 개발자 행사 개최
- 기본적으로 업그레이드 버전업 미지원 (최근부터 지원하기 시작)
- 새로운 특징 및 핵심 기능들은 보통 1년을 주기로 많은 변화가 생김

OpenStack 릴리즈 이름

- 차후 Summit이 개최되는 장소와 관련된 지명 등을 중심으로 설문 후 법적 이슈가 없는 이름을 선택
- N : Austin 서밋이 개최된 근처에 Newton House가 있음
- O : Olimpic이 설문 1위였으나, Olympic과의 유사성 등으로 3위로 선정된 Barcelona 근처 해변 이름인 Ocata가 선정

OpenStack 구성요소

자원 종류 → OpenStack 구성요소 이름

Compute (컴퓨팅) → Nova

Storage (스토리지) → Swift (Objects), Cinder (Block), Glance (Images)

Identity (인증) → Keystone

Network (네트워크) → (Quantum) Neutron

OpenStack 구성 요소 → (조금 더 쉽게 보면)

- Nova (VM 인스턴스 관리)
- Swift (Object 스토리지 관리)
- Glance (VM 이미지 관리)
- Keystone (통합 인증 관리)
- Horizon (웹 관리 포털)
- Neyutron (가상 네트워크 관리)
- Heat (템플릿 관리)
- Ceilometer (Metering 관리)

소프트웨어로 클라우드 인프라를 자동화하는 OpenStack

프로그래머블 인프라

- Compute, 네트워킹, 스토리지를 관리하는 API 공통 집합

단일 플랫폼

- 가상머신, 컨테이너, 베어메탈

→ "오픈" 소스, 디자인, 개발, 커뮤니티

Datacenter Cloud (Infrastructure)

Container (Infrastructure)

Edge (Infrastructure)

CI/CD (Continuous Integration & Continuous Delivery)

새로운 기술 : 커뮤니티 간 협력

Containers : 쿠버네티스, 도커, 메소스

PaaS : Cloud Foundry, OpenShift

NFV : OPNFV, Cloudify

Provisioning : Terraform, puppet, ANSIBL, SALTSTACK

테스트 : 커뮤니케이션 & 피드백

- OpenStack CI 테스트
- OpenStack 서밋 & 포럼
- PTG (Project Team Gathering)

OpenStack과 하이브리드 클라우드

Private Cloud

- openstack

Public Cloud

- 구글 클라우드 플랫폼, AWS, Azure

## 오픈스택과 비즈니스 에코시스템
OpenStack 생태계 : 업스트림과 다운스크림의 상호 교류

업스트림 활동

- 개발 : 코드 컨트리뷰션
- 문서화
- 번역
- 개발 항목 & 스펙 정의
- 버그 수정
- ...

다운스트림 활동

- 배포된 릴리즈 설치 & 사용
- 사용자 피드백
- 비즈니스 도입
- 유스케이스 & 이점 공유
- Marketing 메세지 & 전략
- ...

OpenStack 거버넌스

- OpenStack Foundation : OpenStack을 "개발, 지원, 보호, 홍보" 하기 위해 만들어진 비영리 재단
- 개인 멤버 : [www.openstack.org](http://www.openstack.org) 에 "Foundation Member"로 가입한 모두
- 기관 멤버 : 플래티넘과 골드 스폰서
- 뿐만 아니라 여러 지원을 하는 회사 및 기관이 많습니다.

- 여러 계층으로 구성된 리더쉽
- 이사회 (Board of Directors)
- 기술 위원회 (Technical Committee) : ATC (Active Project Contributor) 와 ATC (Active Technical Contributor)
- 사용자 위원회 (User Committee) : AUC (Active User Contributor)

OpenStack을 바라보는 기업의 관점

- OpenStack을 도입/사용하고자 하는 기업
- 자체 인프라 관리에 도입
- 새로운 인프라 구축에 OpenStack 활용

vs

- OpenStack 생태계에 합류하고자 하는 기업
- 기업 소프트웨어 개발에 있어 OpenStack 활용
- OpenStack 활성화가 기업 제품 판매 활성화에 영향
- OpenStack 방향에 따른 기업 수익성 영향 고려

OpenStack을 도입한 글로벌 기업

- OpenStack 도입 글로벌 기업
    - Best Buy
    - BMW
    - Comcast
    - Disney
    - WalMart
    - 카카오
    - 넷마블
    - ...

OpenStack 생태계에서의 글로벌 기업

- 배포판 제공 회사
    - Canonical
    - RedHat
    - HP (현재 HP Enterprise)
    - Oracle
    - ...
- x86 (서버) 제조사
    - Dell
    - HP
    - ...
- (소프트웨어 정의) 네트워킹
    - Cisco
    - Arista
    - ...

글로벌 기업들의 OpenStack 오픈소스 적극 참여

- OpenStack 코드 기여에 참여한 글로벌 기업
    - [https://www.stackalytics.com](https://www.stackalytics.com) 에서 확인 가능
- 주요회사
    - Red Hat
    - VMware
    - Cisco
    - Canonical
    - ...

- 참여 이점
    - 자사에서 제작하는 S/W code에도 연관
    - 일부 회사 소식 개발자 : 오픈 소스 기여가 회사 업무
    - 오픈소스를 통한 개발력 향상
    - 자사 방향과 오픈소스의 개발 방향을 일치시키기도 한다

OpenStack : Nova

- Nova
    - 가상 머신 자원을 관리하는 OpenStack의 구성 요소 중 하나입니다

OpenStack Nova의 발전

- 최초 릴리즈인 Austin에는 Nova와 Swift (오브젝트 스토리지 관리)만 존재
- 오픈 소스 하이퍼바이저 위주로 지원 시작
    - Xen+Libvirt
    - KVM
    - XenAPI (for XenServer)
    - QEMU
- 참고 : 네트워크 관리에 대해서는, 가상 인스턴스 관리와 동시에 관리되어야 한다고 생각하여 Nova-network 라는 하위 구성 요소를 두어 발전 → 후에 Quantum / Neutron으로 발전

OpenStack & (Vendor) 드라이버

- 다양한 상용 / 오픈 소스 하이퍼바이저, 스토리지, 네트워크 장비 등과 호환성이 높음

다양한 상용 하이퍼바이저 지원 시작

- 시작은 사실 XenServer 부터 ...
- (Xen 기반 상용 하이퍼바이저이기에 상대적으로 쉬웠을 듯)

Nova 지원 하이퍼바이저

- [https://docs.openstack.org/developer/nova/support-matrix.html](https://docs.openstack.org/developer/nova/support-matrix.html)
- (Note : 몇몇 정보는 업데이트되지 않았을 수 있습니다)

사실 Hyper-V도 초창기부터...

- Nova 소스 저장소 : [https://git.openstack.org/cgit/openstack/nova](https://git.openstack.org/cgit/openstack/nova)

2012년 10월, Folsom Summit에서 발표

OpenStack : not only Nova but also...

- 실제 고려시에는 네트워크, 스토리지 등 다방면 고려 필요
- Cloudbase

## 오픈스택 설치시스템 준비
가상 서버 준비하기 - Hypervisor 설치 전 준비

최소사양

- CPU : 4 core 이상
- Memory : 4GB 이상
- Disk : 500GB

권장사양

- Memory : 8GB 이상 (Single instance 이상의 경우 인스턴스 메모리 크기 * 인스턴스의 개수)

우분투 설치하기 - 우분투 DeskTop 설치 - VIrtualBox 에서 VM 생성

네트워크 테스트 베드 구성하기

- 유무선 네트워크 → 인터넷 공유기(라우터) → 모뎀 → 인터넷

네트워크 구성도

인터넷 → AP 192.168.0.1 → 192.168.0.101 → VirtualBox를 이용한 오픈스택 설치 → 우분투 서버

우분투 명령어

- nano → 편집기 명령어 + 경로
- ifconfig → 설정 되있는 네트워크 목록 확인

## DevStack
DevStack 이란?

- 복잡한 오픈스택 시스템을 자동으로 설치하여 어떻게 동작하는지 알기 위한 프로젝트
- 오픈스택을 처음 접하는 유저에게 추천
- 오픈스택의 프로젝트의 All-in-One 설치를 제공하며, 어떤 구성요소들이 있는지 확인할 수 있음
- [https://docs.openstack.org/devstack/latest/](https://docs.openstack.org/devstack/latest/)

DevStack 설치를 위한 사전 준비

- 최신 버전의 Virtualbox
- Intel : VT-d, VT-x / AMD : AMD-V를 지원하는 64비트 CPU
- 8GB이상의 RAM
- Ubuntu Server LTS 최신버전 VM에 설치
- DevStack 프로젝트 repository
- VM으로 DevStack Clone
- local.conf 설정

DevStack 설치

- 이전 영상에서 “stack” 사용자를 생성하지 않은 경우 : stack 유저 추가
    - $ sudo useradd -U -G sudo -s /bin/bash -m stack
    - $ echo “stack ALL=(ALL) NOPASSWD: ALL” | sudo tee /etc/sudoers.d/stack
    - $ sudo passwd stack
    - $ sudo su - stack

- Devstack 다운로드
    - $ git clone -b stable/pike [https://git.openstack.org/openstack-dev/devstack](https://git.openstack.org/openstack-dev/devstack)
    - $ cd devstack

주의사항

- Ubuntu 최신으로 업그레이드 할 것
    - 이전 영상에서 업그레이드 선택 안했을 때
    - $ sudo apt update && sudo apt dist-upgrade && sudo apt install git
- local.conf 파일 생성하기
- 설치 시작
    - ./stack.sh

설치 데모 : 네트워크 구성 한경

- 로컬 영역 연결 1 : 인터넷 연결
- VIrtualBox → 로컬 영역 연결 2 : 호스트 네트워크 192.168.56.1
- API request → Nova API → Compute → enp0s8 : 인터넷 연결
- 가상 머신 → Other components → enp0s3 : 호스트 네트워크 192.168.56.101

DevStack 설치 후 주의사항

- DevStack이 설치된 VM의 OS를 종료하지 말고 스탭샷을 만드시오
- DevStack이 VM 내에서 종료해야 할 경우 unstack.sh를 이용하시오
- github에서 DevStack을 Clone한 뒤 실행 전 branch를 버전에 맞게 checkout하여 주십시오
- Virtualbox에서 32bit 옵션만 있는 경우 BIOS에서 Virtualization Technology 활성화와 Hyper-V가 꺼져 있는지 확인하여 주십시오

## Horizon 대시보드
Horizon 대시보드란

- 웹 대시보드를 통해 OpenStack 자원을 관리하는 프로젝트
- Python Django + Angualr JS로 구현됬다

Horizon 대시보드 변천사

Essex

Havana

Queens

Horizon 대시보드 사용해보기 - 주요 용어

- 사용자 (User)와 프로젝트 (Projects)
- 한 사용자는 여러 프로젝트에 속할 수 있습니다
- 인스턴스 (Instance)
- OpenStack에서는 설치 환경 내에서 가상 머신이 실행 중인 대상을 이야기합니다.
- 인스턴스 유형 (Instance Type)
- OpenStack은 VirtualBox와 달리, 미리 인스턴스 유형을 지정하고 (CPU, 램, 디스크 용량 등), 해당 인스턴스 유형을 사용하도록 되어 있습니다.)
- OpenStack에 있는 2가지 유형의 IP주소
- Fixed IP : 인스턴스가 생성된 이후 종료될 때까지 변하지 않는 IP 주소 (관리용)
- Floating IP : 서비스를 위해 필요에 따라 인스턴스에 연결/해제하는 IP 주소 (서비스용)

Horizon 대시보드 사용해보기 - 살펴볼 과정

1. 내부 네트워크 생성 : 인스턴스가 사용할 가상 네트워크
2. 이미지 생성 : 사용할 인스턴스 이미지 직접 등록
3. Flavor 생성 : 인스턴스 유형을 미리 정하기
4. 인스턴스 생성 : 1~4를 기반으로 인스턴스를 생성
5. 블록 스토리지 생성 : 가상 디스크 추가 가능
6. ssh 접속과 볼륨 연결 확인 : 인스턴스 접속

네트워크

내부 네트워크 생성

demo 계정으로 접속

1. 프로젝트
2. 네트워크
3. 네트워크 생성
4. 라우터
5. 라우터 생성
6. 네트워크 토폴로지

이미지 올리기

순서

1. 관리자
2. 이미지
3. 이미지생성
4. 이미지 이름
5. 이미지 설명
6. 이미지 소스 유형 파일 검색
7. 포맷
8. 이미지 생성

Flavor

1. 관리자
2. Flavor
3. Flavor 생성

인스턴스 생성

1. Compute
2. 인스턴스
3. 인스턴스 시작
4. 인스턴스 이름
5. 이미지 선택
6. Flavor 선택
7. 네트워크 선택
8. 보안그룹 선택
9. 키페어 생성
10. 인스턴스 시작

블록 스토리지 사용

1. Compute
2. 볼륨
3. 볼륨생성
4. 볼륨이름
5. 크기
6. 볼륨생성

ssh 접속과 볼륨 연결 확인

## CLI로 오픈스택 사용하기
OpenStack CLI 소개

- CLI : Command-Line Interface
- OpenStack 각 구성 요소에 대한 API를 직접 호출하여 원하는 작업을 명령어로 수행
- 참고 : OpenStack은 각 구성요소별로 API 제공
- Nova (Compute API) : [https://developer.openstack.org/api-ref/compute](https://developer.openstack.org/api-ref/compute)
- Neutron (Networking API) : [https://developer.openstack.org/api-ref/networking](https://developer.openstack.org/api-ref/networking)
- Keystone (Identity API) : [https://developer.openstack.org/api-ref/identity](https://developer.openstack.org/api-ref/identity)
- ...
- 통합 CLI 툴 제작
- 이전에는 Nova / Neutron / Keystone 등 따로 CLI 명령어를 사용해야 했음
- 현재 통합 클라이언트 : openstackclient (명령어 : “openstack”)

OpenStack CLI 활용하기

- 참고 문서 : 한글 OpenStack 설치 가이드 (URL : [https://docs.openstack.org/ko_KR/install-guide](https://docs.openstack.org/ko_KR/install-guide) )
- 데모는 Ocata 버전을 기준으로 하나, 차후 버전에서도 동일 방식으로 사용 가능
- 클라이언트 환경 스크립트 : [https://docs.openstack.org/ocata/ko_KR/install-guide-ubuntu/keystone-openrc.html](https://docs.openstack.org/ocata/ko_KR/install-guide-ubuntu/keystone-openrc.html) (참고 : DevStack 환경에서는 “source openrc [사용자명] [프로젝트명]” 을 사용)
- 이미지 올리기 : [https://docs.openstack.org/ocata/ko_KR/install-guide-ubuntu/glance-verify.html](https://docs.openstack.org/ocata/ko_KR/install-guide-ubuntu/glance-verify.html)
- 인스턴스 생성 (네트워크, 볼륨 등 포함) : [https://docs.openstack.org/ocata/ko_KR/install-guide-ubuntu/launch-instance.html](https://docs.openstack.org/ocata/ko_KR/install-guide-ubuntu/launch-instance.html)

이미지 올리기 (Glance service)

```
. openrc admin
wget https://download.cirros-cloud.net/0.3.5/cirros-0.3.5-x86_64-disk.img

oepnstack image list // 현재 이미지 목록
openstack image create "cirros" \
> --file cirros-0.3.5-x86_64-disk.img \
> --disk-format qcow2 --container-format bare \
> --public
\ 을 사용하면 줄바꿔서 명령어를 사용할 수 있다
```

각종 OS 이미지 다운로드 URL : https//docs.openstack.org/image-guide/obtain-images.html 

이미지 업로드시 사용하는 CLI 명령어

```
openstack image create
옵션
--file cirros-0.3.5-x86_64-disk.img // 파일명을 지정
--container-format bare // 컨테이너 포맷 방식
--public 모든 프로젝트가 공유 허용할건지 정의
```

디스크 포맷 방식에 종류 URL : [https://docs.openstack.org/image-guide/image-formats.html](https://docs.openstack.org/image-guide/image-formats.html) 

프로젝트 네트워크 생성

1. 컨트롤러 노드에서 demo ccredential을 소스로 하여 사용자 전용 CLI 명령에 대한 엑세스를 갖습니다.
2. 네트워크 생성
3. 네트워크에 서브넷을 생성

```
source openrc demo
openstack network list

openstack network create selfservice
openstack subnet create --network selfservice --dns-nameserver 8.8.8.8 --gateway 172.16.1.1 --subnet-range 172.16.1.0/24 selfservice
```

라우터 생성

```
. openrc demo

openstack router list

라우터 생성
openstack router create router

셀프 서비스 네트워크 서브넷을 라우터에 인터페이스로 추가합니다
neutron router-interface-add router self-service

게이트웨이를 라우터에 대한 프로바이더 네트워크로 설정합니다
neutron router-gateway-set router provider

퍼블릭 네트워크로 설정합니다
neutron router-gateway-set router public
```

인스턴스 생성

flavor

```
openstack flavor list

openstack flavor create --id 0 --vcpus 1 --ram 64--disk 1 m0.nano

source openrc admin

. openrc demo

```

네트워크 생성한 NET ID와 인스턴스 연결 필요

```
openstack server create --flavor m0.nano --image cirros --nic net-id // copy 시키기

openstack network list

openstack server create --flavor m0.nano --image cirros --nic net-id 아이디 --security-group default selfservice-instance

```

블록 스토리지

```
.openrc demo
openstack volume create --size 1 volume1

openstack volume list

openstack server add volume selfservice-instance volume1

```

1. 볼륨을 인스턴스에 연결
2. 볼륨 목록
3. SSH 상용하여 인스턴스에 엑세스 하고 /dev/vdb 블록 스토리지 장치에 대한 볼륨 검증 fdisk 명령어 사용

## 오픈스택과 REST API
잠깐 : API에 관해서

- API (Application Programming Interface)
- 프로그램과 프로그램이 서로 명령을 주고 받기 위해 미리 약속해둔 일종의 규칙

API로 클라우드 인프라를 관리하려면

- API 파악시 장점
- 어떤 구성 요소가 있는지 파악 가능
- 추상화되어 있는 기능에 대한 자세한 이해
- 시스템  구축 표준화 방안 마련

- OpenStack : CLI와 API의 차이점
- CLI에서 수행하는 모든 명령어를 API 호출로 사용 가능
- API를 활용하면 다양한 아이디어를 붙여 클라우드 소프트웨어를 만들 수 있음
- 다른 클라우드와 상호 연동 가능
- OpenStack 일부 구성 요소만을 사용하여 클라우드 서비스를 구축 가능

OpenStack App Hackathon

- 2016년 Taiwan을 시작으로 Mexico, 호주 등 다양한 국가에서 개최
- 40여 시간동안 클라우드 API를 활용한 OpenStack App을 개발
- OpenStack App 개발을 위한 다양한 문서  [https://www.openstack.org/appdev/](https://www.openstack.org/appdev/)
- FirstApp 문서 : OpenStack App 첫 개발을 위한 내용을 문서로 정리

클라우드 인프라를 API로 다루기 위해 필요한 것들

1. API를 제공하는 주체 (서버 파트)
- “API 액세스” 메뉴에서 API 목록 확인
1. API를 사용하는 주체 (모바일 앱 with Fuse, CLI, ...)
- 먼저, curl로 간단히 테스트 하기 전에.. 문서를 봅시다
- 일단 인증 기본이 되는 토큰을 가져와야 API 사용이 가능)
- OpenStack Keystone : API v2와 v3가 있음
- API URL을 알아냄 → https://[server URL]/identity/v3/auth/toekns
- Postman : GUI 환경으로 API 테스트가 용이함
- 모바일 앱에서 테스트를 해 보려면? 일단 프로토타이핑이 필요한데...
- Fuse로 만드는 방법 : 자스크립트로 REST API 통신

Client (HTTP POST)

Server (REST Interface)

JSON/REST/HTTP

GET/POST 방식

```
bash
ssh stack@192.168.56.101
OS_TOKEN=[X-subject-Toekn]
OS_COMPUTE_API=https://[Server URL]/compute/v2.1
curl -s -H "X-Auth-Token: $OS_TOKEN" \
$OS_COMPUTE_API/flavor

```