# 오픈소스sw개론 과제

- ## top
  - 리눅스 시스템의 CPU 사용량, 메모리 사용량 등 전반적인 상황을 실시간으로 모니터링할 수 있는 명령어
  ![1](https://github.com/SSaemiy/homework/assets/171468506/db057e79-c42b-4485-8ce4-b4c70ccf2387)
  - 가장 상단에 있는 영역은 __'요약영역'__, 그 하단에 있는 영역은 __'디테일영역'__
  
  __1. 시스템 시간, Uptime, 유저 세션 수__
  
  __2. 로드 애버리지__ : 왼쪽에서 부터 1분, 5분, 15분 동안의 평균 시스템 부하를 보여줌.
  
  __3. Tasks__ : 현재 프로세스들의 상태 출력
  
  __4. CPU 사용량__ : CPU의 사용율을 출력
  
  __5. 메모리 사용량__
    
- ## ps
  - Process Status 의 약어, 현재 구동 중인 프로세스 정보를 확인
    ![2](https://github.com/SSaemiy/homework/assets/171468506/5c0a35c7-673d-4d40-91c9-0e261b02d7ed)
    
  __-e__ : 다른 사용자들이 구동시킨 모든 프로세스를 보여줌
    ![3](https://github.com/SSaemiy/homework/assets/171468506/2a3aaab6-4a8b-459d-adff-756f448a9ae7)

  __-f__ : 상세한 정보를 보여줌 (Full Format)
    ![4](https://github.com/SSaemiy/homework/assets/171468506/cdfd56c1-6889-43ce-b7b9-c00f01545052)

  __-l__ : -f 보다 더 상세한 정보를 보여줌 (Long Format)
    ![5](https://github.com/SSaemiy/homework/assets/171468506/68c02835-3ff4-4e71-89d5-66dcdd261085)

- ## jobs
  - 백그라운드에서 실행 중인 작업 목록 출력
  - 'jobs [OPTIONS] [JOB]' 형식으로 사용
    ![image](https://github.com/SSaemiy/homework/assets/171468506/15af9809-8557-4ef5-a7b6-d38ea6dd10ea)

- ## kill
  - 프로세스에 시그널을 보내어 원하는 동작 수행
  - 'kill [옵션] <PID>' 형식으로 사용
  - __-s <signal>__ : 특정 시그널을 사용하여 프로세스 종료
  - __-l,--list__ : 지원되는 시그널 목록 출력
  - __-a,--all__ : 현재 사용자에 속한 모든 프로세스 종료
  - __-q,--queue__ : 프로세스에 시그널을 보내는 대신 시그널을 대기열에 추가
