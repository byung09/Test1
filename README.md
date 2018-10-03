# Git 명령어 정리
&nbsp;

  <dl>
  
  <dt>git config --global --unset-all user.email</dt>
  <dd>: &nbsp; 전체 사용자 이메일을 삭제하는 명령어로 -all을 빼고 email 옆에 사용자이메일을 입력하면 사용자이메일을 설정하여 삭제하는 명령어. 
  </dd>
  
  <dt>git config --global --unset-all user.name</dt>
  <dd>: &nbsp; 전체 사용자 이름을 삭제하는 명령어로 -all을 빼고 name옆에 사용자이름을 입력하면 사용자이름을 설정하여 삭제하는 명령어. 
  </dd>
  
  <dt>git config - -global - -list</dt>
  <dd>: &nbsp; 위에서 설정한 정보가 제대로 삭제 되었는지 리스트확인을 할 수 있는 명령어.
  </dd>
  
  </dl>

---

  <dl>
  
  <dt>git init</dt>
  <dd>: &nbsp; cd를 이용하여 원하는 폴더로 이동후 폴더 기준으로 git이 활동할 수 있는 영역을 미리 만들어 주기위해 초기화(init)을 한다. 해당 폴더의 터
미널에서 git init 명령어로 미리 환경을 구성해준다. 최초 한번만 해주면된다.
  </dd>
  
  <dt>ls -al</dt>
  <dd>: &nbsp;제대로 구성이 되었다면 위 명령어를 통해 .git이라는 파일을 확인할 수 있다.</dd>
  
  <dt>git clone <저장소url></dt>
  <dd>: &nbsp;말그대로 해당 소스를 그대로 복제해온다는 의미로, git repository 전체를 가져온다
clone과 pull의 차이점은 clone은 git repository전체를 가져오는것이고, pull은 파일만 가져온다는점이다.
  </dd>
  
  </dl>
  
---
  
  <dl>
  <dt>git add <파일></dt>
  <dd>: &nbsp;내가 커밋하고 싶은 파일을 지정해서 스테이지에 올리거나 파일을 새로 추적할 때 사용
  </dd>
  </dl>

---

  <dl>
  <dt>git commit -m “<메시지>”</dt>
  <dd>: &nbsp; add된 txt파일에 대해 변경사항을 적용하고 새로이 저장할 수 있다. git add후 수정을 했다면 commit전에 다시한번 add를 해야 커밋에 수정사항이 반영된다.
  </dd>
  </dl>
  

