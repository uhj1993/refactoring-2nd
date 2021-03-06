# 프로세스의 상태

## 생성 상태

- 생성 상태(create)는 프로세스가 생성된 상태를 의미
- fork() || exec() 함수를 통해 생성
- 이때 PCB가 할당

### fork()

- 부모 프로세스의 주소 공간을 그대로 복사
- 새로운 자식 프로세스를 생성하는 함수

### exec()

- 새롭게 프로세스를 생성하는 함수

## 대기상태

- 대기 상태(ready)는 메모리 공간이 충분하면 메모리를 할당 받고, 아니면 아닌 상태로 대기
- CPU 스케줄러로부터 CPU 소유권이 넘어오길 기다리는 상태

## 대기 중단 상태

- 메모리 부족으로 일시 중단된 상태

## 실행 상태

- running은 CPU 소유권과 메모리를 할당받고 인스트럭션을 수행 중인 상태를 의미

## 중단 상태

- blocked는 어떤 이벤트가 발생한 이후 기다리며 프로세스가 차단된 상태
- I/O 디바이스에 의한 인터럽트로 이런 현상이 많이 발생하기도 함

## 일시 중단 상태

- 대기 중단과 유사하다. 중단된 상태에서 프로세스가 실행되려고 했으나 메모리 부족으로 일시 중단된 상태

## 종료 상태

- terminated는 메모리와 CPU 소유권을 모두 놓고 가는 상태
