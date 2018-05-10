
# GIT
## 1. What's the use of GIT?
 `**source version management**` & `**collaboration**`
## 2. Steps (a. from LOCAL / b. from GITHUB_clone)
 #### a-1. $ git init
 #### a-2. $ git add FILENAME
 #### a-3. $ git commit -m "MESSAGE"
 #### a-4. $ git remote add NICKNAME URL
 #### a-5. $ git push NICKNAME master
***
 #### b-1. GITHUB 에서 repository 생성 후       
 #### b-2. $ git clone URL      
 #### a-3. $ git add FILENAME
 #### a-4. $ git commit -m "MESSAGE"
 #### a-5. $ git push NICKNAME master
***
# BRANCH
## 1. What's the use of BRANCH?
 **master**는 배포용으로만 사용하고, 개발시 웹 서비스의 기능별로 *add/commit*을 하기 위해서 소스코드를 분기하는 목적  
 쉽게 말해서, ~~백업과 비슷한 의미~~......?
## 2. Commands
 #### **$ git branch** -> 접근 가능한 `로컬` 브랜치 보여줘
 #### **$ git branch -r** -> 접근 가능한 `remote` 브랜치 보여줘
 #### **$ git branch -a** -> 접근 가능한 `모든` 브랜치 보여줘
 #### **$ git branch NAME** -> 새로운 브랜치 `생성`하자
 #### **$ git checkout NAME** -> 다른 브랜치로 `이동`하자
 #### **$ git checkout -b NEWNAME**
 #### **$ git merge NAME** -> merge할 BRANCH에서 실행하는 명령. (주로 `master` // merge `당하는` BRANCH의 이름을 적는다)
***
# GIT FLOW
 **KEY WORDS** (++현재까지 이해한 바++)는 기능별 *분리 작업* 및 *적용(commit)*을 깔끔하게 하기 위함이다. 문제 발생 시 원인 규명도 수월하고 문제가 발생한 지점의 관련 기능만을 수정할 수도 있으므로. 또한 기능별 작업자가 다를 수 있으므로 commit이 뒤섞이지 않도록 기능별로 분리해서 commit 해야만 한다.  
 ++push는 동시에 수행해도 무방함++
 ++COMMIT는 시간적 개념, BRANCH는 공간적 개념++

 Example.
        Master에 README.MD 생성됨       -> 이 시점(PM. 10)에서 BRANCH (develop) 생성
        IN develop BRANCH) README.MD 수정 중    -> IN Master) README.MD 변화 없음 *당연히*
        IN develop BRANCH) 수정 후 add/commit/push -> IN Master) README.MD 변화 없음 *당연히*
        IN Master) ++develop++ 내용을 `merge` 해오자 -> develop에서 ++commit된 시점의 소스++가 Master에 반영됨



