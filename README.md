# Mac-Terminal
this file contains terminal commands &amp; descriptions

## Terminal이란?

Terminal은 애플이 개발한 macOS 운영 체제에 포함된 단말 에뮬레이터로 CLI를 기반으로 shell을 통해 텍스트 명령어들을 컴퓨터의 언어로 변환시켜 사용자가 컴퓨터의 운영체제 접근을 가능하게 한다.

> GUI(Graphical User Interface) : 사용자의 편의를 위해 입출력 등의 기능들을 아이콘으로 나타낸 것 
> 
> CLI(Command Line Interface) : 텍스트 명령어를 통해 유저와 컴퓨터간의 상호작용 하는 것



## Terminal 명령어 


### NAVIGATING FILES

```
$ pwd     #현재 디렉토리 경로를 표시 

$ ls      #디렉토리 컨텐츠를 표시

$ ls -l     #디렉토리 컨텐츠를 긴 포멧으로 표시

$ ls -a     #숨겨진 파일 혹은 디렉토리를 표시

$ open .      #터미널의 현 경로를 파일 탐색기로 ((((((열기))))))

$ cd ()     #디렉토리를 ()로 이동

$ cd ..     #현재 경로의 상위 경로로 이동 

$ cd ~      #사용자의 최상위 디렉토리로 이동

$ cd -      #이전 경로로 이동

$ find      #특정 파일이나 디렉토리를 검색
  ex. find . -type file(or directory) -name "*.txt"(or "*.json")

$ clear     # 터미널 스크린 초기화
```

### CREATE AND MANAGE FILES

```
$ touch     #파일의 수정 날짜를 업데이트 (존재하지 않는 파일이라면 새로 생성)

$ cat     #파일의 내용을 표시

$ echo      #입력된 문자열을 터미널에 표시하거나 파일에 컨텐츠로 삽입
  ex. echo "Hello World" > newfile.txt (기존 문자열 덮어쓰기)
  ex. echo "Hello World2" >> newfile.txt (새로운 문자열 추가)
  
$ mkdir     #새로운 디렉토리 생성
  ex. mkdir -p sudo/new/personal.txt
  
$ cp (파일) (경로)     #원하는 경로에 파일을 복사
  ex. cp personal.txt Sudo/
  
$ mv      #원하는 경로에 파일을 이동

$ rm      #파일 삭제

$ rm -r     #디렉토리 삭제

$ grep      #특정 문자열을 포함한 파일을 표시
  ex. grep "new" *.txt

$ grep -n     #특정 문자열이 파일 내 몇번째 줄에 있는지 표시

$ grep -ni      # 대소문자 상관없이 특정 문자열이 파일 내 몇번째 줄에 있는지 표시

$ grep -nir     # 대소문자 상관없이 특정 문자열이 모든 디렉토리 내 몇번째 줄에 있는지 표시
  ex. grep -nir "new .
```

### SETTING ENVIRONMENT VARIABLES

```
$ export      #특정 문자열이 파일이나 디렉토리를 대변하도록 설정
  ex. export MY_FILE = "file"
  
$ env     #설정된 모든 환경변수를 확인

$ unset      #설정된 환경변수를 삭제
```
