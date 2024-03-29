# OS(Operating System)와 Computer Architecture
## 운영체제
- [운영체제란?]()
- [운영체제의 운용기법]() <!-- 일괄 작업, 대화형, 시분할, 분산 -->
- [소프트웨어와 하드웨어]()
- [시스템 소프트웨어와 응용 소프트웨어]()
- [제어, 처리 프로그램]()
- [컴퓨터 리소스]()
- [커널]()
- [커널 구조]() <!-- 단일형 구조, 계층형 구조, 마이크로 구조 -->
- [쉘]()
- [프로세스 관리]()
- [주소 공간, 물리적 주소, 논리적 주소, 주소 바인딩]() <!-- https://charles098.tistory.com/103?category=947356 -->
- [다중 처리]()
- [인터럽트]() <!-- 인터럽트 개념, 동기적 인터럽트, 비동기적 인터럽트, 인터럽트 처리 과정, 이중 모드, 내부 인터럽트, 외부 인터럽트, 시그널, IRQ, 인터럽트 벡터, 인터럽트 핸들러 -->
- [네트워크]() <!-- 포트와 소켓, 소켓 디스크립터 -->
- [보안]() <!-- https://brokenbot.tistory.com/68, https://peemangit.tistory.com/193 -->
- [펌웨어와 디바이스 드라이버]()
- [버퍼와 스트림]()
- [메시지 큐]()
- [핸들러]()
- [I/O Multiplexing]()
- [Programmed Input/Output]() <!-- https://ko.wikipedia.org/wiki/%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8_%EC%9E%85%EC%B6%9C%EB%A0%A5 -->
- [시스템 콜]()
- [캐시 매핑]() <!-- 직접 매핑, 연관 매핑, 집합-연관 매핑 -->
- [터미널 사용]()
- [기계 주기]()
- [가상 데스크톱]()
- [패리티 비트, 해밍 코드]()
- [컴퓨터의 기능]()
- [환경 변수]()
- [가상머신]()
- [코어 덤프(Core Dump)]() <!-- https://velog.io/@jsj3282/%ED%9E%99-%EB%8D%A4%ED%94%84%EC%99%80-%EC%93%B0%EB%A0%88%EB%93%9C-%EB%8D%A4%ED%94%84 -->
- [인터페이스]()
- [POSIX란?]()
- [CLI와 GUI란?]()
- [Unix CLI]()
- [Linux CLI]()
- [파이프]()
- [아카이브, 백업, 압축]() <!-- https://m.blog.naver.com/sosungkuk2/221543915990 참고 -->
- [공유 자원과 임계구역]() <!-- 공유 자원과 임계구역의 개념 및 임계구역 해결 조건 -->
- [임계구역 해결 방법]() <!-- 피터슨 알고리즘, 데커 알고리즘, 세마포어 -->
- [교착 상태]() <!-- 교착 상태 개념, 발생 상황, 교착 상태 필요조건 -->
- [교착 상태 해결 방법]() <!-- 예방, 회피, 검출, 회복 -->
- [디바이스 드라이버]()
## 컴퓨터 구조
- [폰 노이만 구조]()
- [메모리 계층]()
- [명령어 집합 아키텍처(Instruction Set Architecture, ISA)]()
- [버스]() <!-- http://wiki.hash.kr/index.php/%EB%B2%84%EC%8A%A4_(%EC%BB%B4%ED%93%A8%ED%84%B0)#cite_note-.E2.80.9C.EC.8B.9C.EC.8A.A4.ED.85.9C-3 -->
- [병목 현상]()
- [빅엔디언과 리틀엔디언]()
- [참조 지역성의 원리]()
- [중앙 처리 장치(Central Processing Unit, CPU)]() <!-- CPU 구조와 레지스터 종류, CPU 실행 주기, LGA, PGA, BGA -->
- [레지스터]() <!-- SISO, PISO, SIPO, PIPO 및 회로 -->
- [ALU]() <!-- 가산기, 감산기, 멀티 비트 가신기, 보수기, 시프터, 오버플로우 검출기 -->
- [파이프라인]()
- [제어 장치]()
- [기억 장치(Memory)]() <!-- 레지스터, 주기억장치, 보조기억장치, 캐시 메모리 -->
- [캐시 일관성 문제]()
- [입출력 장치(Input/Output Device, I/O Device)]()
- [메인보드(Main Board)]()
- [메인보드 칩셋(Chipset)]() <!-- https://blog.naver.com/revenssy/221466909023 -->
- [전원 공급 장치(Power Supply)]()
- [컴퓨터 온도와 쿨러]()
- [단일/멀티 프로세서]()
- [SoC]()
- [FPU]()
- [GPU와 GPGPU]()
- [MMU]()
- [하드웨어 가속이란?]()
## CPU 스케줄링(Scheduling)
- [CPU 스케줄링]() <!-- 스케줄링 단계(고수준, 중간 수준, 저수준)와 목적, 선점형과 비선점형, 프로세스 우선순위, CPU 집중 프로세스와 입출력 집중 프로세스 -->
- [다중 큐]()
- [정적 스케줄링과 동적 스케줄링]()
- [CPU 스케줄링 알고리즘 종류]()
## 메모리 관리
- [메모리 관리]() <!-- https://ws-pace.tistory.com/27, https://velog.io/@jisoolee11/%EB%A9%94%EB%AA%A8%EB%A6%AC-%EA%B4%80%EB%A6%AC#%EB%8F%99%EC%A0%81-%EC%A0%81%EC%9E%ACdynamic-loading -->
- [메모리 할당 알고리즘]()
- [메모리 오버레이(Overlay)와 스왑]()
- [메모리 분할]() <!-- 가변 분할, 고정 분할, 버디 시스템 -->
## 가상 메모리(Virtual Memory)
- [가상 메모리]() <!-- 가상 메모리의 개념과 매핑 테이블 -->
- [페이징]() <!-- 페이징 기법 구현 및 주소 변환 -->
- [페이지 테이블]() <!-- 페이지 테이블 관리 및 매핑 방식 -->
- [세그먼테이션]() <!-- 세그먼테이션 기법의 구현 및 주소 변환 -->
- [세그먼테이션 페이징 혼용 기법]()
- [요구 페이징(Demand Paging), 페이지 폴트(Page Faults)]() <!-- https://superohinsung.tistory.com/127 -->
- [페이지 교체 알고리즘]() <!-- 페이지 교체 알고리즘 개념와 종류 -->
- [스레싱과 프레임 할당]() <!-- 스레싱 개념과 정적 할당, 동적 할당 -->
## 입출력 시스템
- [입출력 관리]()
- [입출력장치와 채널]()
- [입출력 버스]()
- [직접 메모리 접근(Direct Memory Access)]() <!-- https://ko.wikipedia.org/wiki/%EC%A7%81%EC%A0%91_%EB%A9%94%EB%AA%A8%EB%A6%AC_%EC%A0%91%EA%B7%BC -->
- [버퍼]()
## 디스크 장치
- [HDD와 SSD]() <!-- HDD, HDD 구조, SSD, SSD와 HDD의 차이점, 전송 시간, https://whitesnake1004.tistory.com/273 -->
- [디스크 관리]() <!-- 파티션, 마운트, 포맷(느린/빠른/로우 레벨 포매팅), 조각 모음 -->
- [MBR과 GPT]()
- [네트워크 저장장치]() <!-- DAS, NAS, SAN -->
- [디스크 스케줄링]() <!-- 스케줄링 목적과 알고리즘 종류 -->
- [RAID]()
## 데이터 표현
- [진법과 정보 단위]()
- [데이터의 종류, 데이터 타입]()
### 정수 표현
- [2진법의 정수 표현]()
- [부호없는 정수]()
- [부호있는 정수]()
### 실수 표현
- [고정 소수점]()
- [부동 소수점]() <!-- https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=jwyoon25&logNo=221389077105 -->
### 문자 표현
- [아스키 코드]()
- [유니 코드]()
- [EUC-KR]()
- [Base64]()
## 논리 회로
- [논리 회로란?]()
- [기본 게이트]()
- [논리식, 논리도, 진리표]()
## 조합 논리 회로
- [조합 논리 회로란?]()
- [불 대수 법칙]()
- [And-Or, Or-And 회로]()
- [논리식의 간소화]()
- [K-map]()
- [Don't Care 조건]()
- [멀티 플렉서와 디-멀티 플렉서]()
- [이진 디코더와 이진 인코더]()
## 순서 논리 회로
- [순서 논리 회로란?]()
- [Stable/Unstable]()
- [SR latch]()
- [SR flip-flop]()
- [flip-flop 종류]()
### 카운터
- [비동기식 카운터]()
- [동기식 카운터]()
## 프로세스
- [프로세스란?]()
- [프로세스 생성, 종료]()
- [포그라운드(Foreground)와 백그라운드(Background) 프로세스]()
- [프로세스 주소 공간(Process Address Space)]() <!-- https://hyeyoo.com/175 -->
- [프로세스 상태]()
- [프로세스 제어 블록]()
- [문맥 교환]()
- [프로세스 계층 구조]() <!-- 부모 프로세스, 자식 프로세스, fork와 exec 시스템 콜 -->
- [멀티 프로세스]()
- [프로세스 간 통신]()
- [프로세스 간 동기화 문제]()
- [메모리 누수 문제]()
- [프로세스 관리 문제]()
- [데몬 프로세스]()
## 스레드
- [스레드란?]()
- [동시성과 병렬성의 차이]()
- [스레드 구조]()
- [스레드 레벨]()
- [Blocking과 Non-Blocking]()
- [멀티 스레드]()
- [스레드 안전]()
- [스레드 간 동기화 문제]()
- [데몬 스레드]()
## 파일 시스템
- [파일 시스템]() <!-- 파일 시스템 개념, 파일 시스템 기능, MBR, 파티션 테이블, 부트 블록, 볼륨 제어 블록 -->
- [파일 디스크립터과 파일 테이블]() <!-- 파일 디스크립터, 파일 디스크립터 테이블, 클러스터, Open File Table, https://www.freecodecamp.org/news/file-systems-architecture-explained/ -->
- [가상 파일 시스템]()
### 파일
- [파일 이름]() <!-- 파일 이름의 규칙 -->
- [파일 종류와 확장자]() <!-- 종류(실행/데이터 파일), 확장자 종류와 개념 -->
- [Linux 파일 종류]() <!-- https://nerd-mix.tistory.com/28 참고 -->
### 디렉토리
## Boot
- [컴퓨터 부팅 과정]() <!-- https://dkrnfls.tistory.com/110 -->
- [MBR, VBR]() <!-- MBR https://lemonpoo22.tistory.com/23, VBR https://www.techopedia.com/definition/25922/volume-boot-record-vbr -->
- [GPT 파티션 방식]()