# Git

> 분산 버전 관리 시스템 

- 코드의 버전을 관리

## Git의 3가지 영역
- Working Directory : 실제 수정이 이루어지는 공간
- Staging Area : 다음 버전에 추가시킬 파일만 등록하는 중간 준비 영역
- Repository : Staging 공간에 있는 파일의 수정사항만 보관하는 곳

## Git의 동작
- git init : 현재 위치의 디렉토리에 git 레포 생성
- git status : 현재 스테이징 상태 확인
- git add : 스테이징 공간(추상)에 버전관리할 파일 추가
- git commit (-m) : 버전을 등록함 (무엇을 어떻게 수정했는 지에 대한 설명)
- git log : 커밋된 기록을 확인할 때

### vi 사용법
- insert : 키보드의 insert키 or I키, 종료하면 ESC
- save&quit : 모드 종료 후 ":wq"

## Git 레포를 원격에 올리기

> git remote add origin (주소)
> - 여기서의 origin은 별명, 올릴 목적지나 주소로부터 가져올 것을 별명으로 부르기 위해 쓰는 것
> - 이름을 다르게 사용할 수도 있음.
> - fetch용, push용으로 구분할 수 있음.

- git push : 현재 내용을 (목적지)에다가 (branch)로부터 넣음. 

### 실제 작업 사이클

1. 프로젝트 최초 1회 git init
2. 각 파일이 작업이 끝날 때마다 git add
3. 각 작업 단위 완료 시마다 git commit
4. 2~3 반복하다가 그날 작업이 끝나기 전에 git push

## 원격에 있는 레포를 복제해서 가져오기

> git clone (원격저장소 주소)
