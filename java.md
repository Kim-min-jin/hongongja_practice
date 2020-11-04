# 1. thread 
# 기존 실행 흐름
main ---->  블로킹
# 스레드 실행 흐름
main -----> 블로킹 
thread ------->



# 1. 바이트 기반 스트림 
## 1.1. InputStream (프로그램이 도착지)
- int read(byte[] buf): 
  - 파라미터 : 읽을 값을 저장하는 공강
  - 반환값 : 읽은 바이트 수 
- void close(): 자원 반납 및 입력 스트림 종료(필수) 
  
## 1.2. OutputStream(프로그램이 출발지)
- void write(byte[]) 
  - 파라미터 : 출력 스트림으로 buf를 보냄
- void flush():
- void close(): 자원 반납 및 출력 스트림 종료(필수)

## 2.1. Reader(입력, 도착지)
- int read(char[] cbuf)
  - 파라미터 : cbuf에 문자열을 담음
  - 반환 : 읽은 문자 개수
## 2.2. Writer(출력, 출발지)
- void write(char[] cbuf)
  - 파라미터 : cbuf에 있는 내용을 출력으로 보냄
  - void write(String str)
    - 파라미터 : 출력으로 보낼 문자열
  - flush()
  - close()