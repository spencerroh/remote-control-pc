# remote-control-pc

## 기본 아키텍처
Master/Slave 구조, 1:N 의 별형 topology 사용

## Host(Master)
- 중앙에서 Secondary를 관리하고, 명령을 내리는 Control-Tower 역할 수행
- 각 Secondary를 관리하는 UI를 가진다.

## Device(Slave)
- GUI-less 프로그램
- Primary에서 오는 요청을 처리
- 배포성을 고려하여 자동 업데이트 기능 지원

## 명령
- 파일 시스템 드라이브 목록 조회
- 경로 내 파일/디렉토리 목록 조회
- 파일/디렉토리 이동/복사/삭제
- Primary에서 파일을 Secondary의 특정 경로에 복사
- 프로세스 목록 조회/종료
- 프로그램 실행
- 프로그램 업데이트 실행
- PC 재부팅/종료예약/종료
