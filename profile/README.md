<div align=center>
   <h1>
    :smiley:SM COSSTON 대회
   </h1>
   <h3>
   SM웰니스 github organization
   </h3>
 </div>

## 레포지토리 생성(프론트, 백엔드)
* .gitignore 생성 보안이 필요한 디렉토리는 git에 포함 시키지 않는다. 
* 서로서로 기능을 달리 구현할 것임 따라서 branch를 꼭 파서 코딩 후, main과 결합 <code> main이 안돌아가는 걸 방지하기 위함</code>

## :wrench: 진행 방법
1. 원격저장소 로컬에 가져오기 <br>
<code> **https://github.com/SM-Wellness/레포이름.git** </code> 
2. 로컬에서 <strong>기능 브랜치</strong> 생성하기<br>
local workspace에 'login'라는 이름으로 브랜치 생성<br>
<code> **git branch login** </code>
3. 로컬에서 브랜치를 변경 후 git add로 추가, commit, push를 진행
4. 코드 리뷰가 필요 할 시, pull request 작성 해야함.
5. 한 기능을 같이 코딩할 시 -> login branch로 이동 후, pull해서 가져옴.
6. commit, <code><strong> git push -u origin login</strong> 푸쉬 작업 후,</code>  원격저장소 github에서 pull request를 진행 

**※기능을 완성했다면?**<br>
1. <code>**git checkout login**</code>  - main에서 csyeob 브랜치로 전환 로컬에서 작업
2. <code>**git commit -m "message"**</code> - 작업 후 <code>**git add .**</code> 이후 커밋
3. <code>**git push origin login**</code>  - 원격저장소 csyeob 브랜치에 푸시
4. <code>**git checkout main**</code>  - 브랜치 전환(main에 merge 요청하기 위함)
5. <code>**git pull**</code> - 원격저장소 main의 최신 정보를 로컬에 업데이트 시키기(최신정보가 아니면 push가 안됨)
6. <code>**git merge login**</code>  - main에 login 기능 브랜치 작업 반영
7. <code>**git push -u origin main**</code> - 원격저장소 main에 반영
