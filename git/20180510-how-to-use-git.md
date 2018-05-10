
# GIT
## 1. What's the use of GIT?
 `**source version management**` & `**collaboration**`
## 2. Steps (a. from LOCAL / b. from GITHUB_clone)
 #### a-1. $ git init
 #### a-2. $ git add FILENAME
 #### a-3. $ git commit -m "MESSAGE"
 #### a-4. $ git remote add NICKNAME URL
 #### a-5. $ git push NICKNAME master

 #### b-1. GITHUB 에서 repository 생성 후       
 #### b-2. $ git clone URL      
 #### a-3. $ git add FILENAME
 #### a-4. $ git commit -m "MESSAGE"
 #### a-5. $ git push NICKNAME master

# BRANCH
## 1. What's the use of BRANCH?
 `**master**`는 배포용으로만 사용하고, 개발시 웹 서비스의 기능별로 add/commit을 하기 위해서 소스코드를 분기하는 목적  
 쉽게 말해서, 백업과 비슷한 의미......?
## 2. Commands
 #### **$ git branch** -> 접근 가능한 `로컬` 브랜치 보여줘
 #### **$ git branch -r** -> 접근 가능한 `remote` 브랜치 보여줘
 #### **$ git branch -a** -> 접근 가능한 `모든` 브랜치 보여줘
 #### **$ git branch NAME** -> 새로운 브랜치 `생성`하자
 #### **$ git checkout NAME** -> 다른 브랜치로 `이동`하자
 #### **$ git checkout -b NEWNAME**
 #### **$ git merge NAME** -> merge할 BRANCH에서 실행하는 명령. (주로 `master` // merge `당하는` BRANCH의 이름을 적는다)
