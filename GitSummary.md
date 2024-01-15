# Git 정리
## 1. 기본 설정
#### Git 계정 설정
    git config —global user.name ??
    git config —global user.email ??
    
#### 설정 확인
    git config user.name
    git config user.email

#### 로컬 저장소(PC 저장소) 설정
    git init
    
#### 원격 저장소(git hub 저장소)설정
    git remote add origin ??
    
#### 원격 저장소 설정 확인
    git remote -v
    
#### 원격 저장소 삭제
    git remote rm origin


## 2. 로컬 저장소 파일 → 원격 저장소
#### Add & Commit
    git add ??
    git commit -m “??”
    
#### Commit한 파일을 원격 저장소에 등록
    git push -u origin master

#### 참고
    git add .
    - working directory에 있는 모든 파일 add

    git commit -am “??”
    - add와 commtit 동시 수행


## 3. 원격 저장소 파일 → 로컬 저장소
#### Pull
    git pull origin master

#### Clone
    git clone ??
    
#### 참고: Pull-Clone 차이점
    
    git clone 명령은 로컬 저장소의 내용과 원격 저장소의 내용을 일치시킨다. 기존 작업 파일이 있을 경우 clone 명령을 사용하면 기존 작업 내용을 복구해야 하는 상황이 온다. 따라서 프로젝트에 처음 투입될 때 사용된다.

    git pull 명령은 원격 저장소의 내용을 가져와서 현재의 내용과 병합시킨다. 즉 변경 사항만 가져오면서 기존 작업 내용을 새로운 작업 내용으로 업데이트할 때 사용된다.

    git pull 명령은 병합 과정도 포함되어 있기 때문에, 이전에 commit을 하지 않을 시 덮어쓰기 에러가 발생할 수 있다. 즉 기존 작업에 대해 commit을 미리 해 두고 pull을 수행해주자.

    참조: <https://kimcoder.tistory.com/288>

## 기타
#### 브랜치 확인
    git branch
#### 브랜치 이동
    git checkout ??
#### Change Direcotry
    cd ??