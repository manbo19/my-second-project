# TIL

## 리눅스 명령어

1. ls

   > list(목록)

2. cd
   change directory (작업 경로 변경)

3. rm
   remove (파일 삭제)

4. mkdir  
   make directory (작업목록 생성)

5. rmdir  
   remove directory (작업목록 삭제)

6. touch  
   파일 생성

7. cat  
   파일의 내용 출력

## Git

1. init  
   git 생성
2. add <파일명>  
   staging area로 이동
3. commit -m <메시지>  
   Repository로 이동
4. push <원격저장소> <브랜치>  
   원격(GitHub)으로 이동
5. pull <원격저장소> <브랜치>  
   원격에서 로컬로 복사
6. clone <원격저장소> <브랜치>  
   원격에서 로컬로 복제

7. status  
   Staging area의 상태
8. log  
   repository의 상태

9. git commit --amend  
   바로 전 commit과 Staging area의 Merge을 할 때
10. git restore --staged <파일명>  
    Staging area의 파일을 Working Directory로 가져옴

![Git Sheat Sheet](asset/gitcheatsheet.gif)

## 문자코드와 인코딩

1. 문자코드란?  
   문자와 숫자를 1:1 매핑해놓은 값
   컴퓨터가 사용하는 0과 1로 변환할 때 사용되는 기준

   > 매핑된 것을 2진법에 따라 2진수로 바꾸고 인코딩 작업을 함
   > 문자코드에 따라 인코딩 방법이 달라짐

2. 인코딩이란? (<->디코딩)  
   나열된 2진수들을 어떻게 묶어서 처리하느냐
   매핑시켜놓은 것을 다시 조합해서 사용하는 것

3. 문자코드의 종류

- ASCII코드 (아스키문자코드)  
  7비트, 기본, 대표적

- 확장ASCII코드(확장아스키문자코드)  
  ANSI(안시코드), 8비트
  각 나라에서 사용하는 코드값에 맞게 불러와야 함

  > 한 비트는 코드페이지 값  
  > code page : 각 나라별로 제공됨
  > 대한민국 code page 값은 cp949

- 유니코드
- EUC-KR코드  
  조합형과 완성형이 있는데 거의 완성형 사용
  완성형으로 사용했을 때 없으면 깨짐
  한글은 문자가 깨지는 현상이 자주 발생함

  > 다국어를 지원해주는 코드인 UTF-8을 많이 사용함

4. 인코딩의 종류

- ASCII인코딩
- 확장ASCII인코딩
- 유니코드 인코딩
  > UTF-8  
  > 길이가 가변 걍 사용할만큼만, 제일 많이 사용  
  >  UTF-16  
  >  고정, 2바이트만 사용함  
  >  UTF-32
