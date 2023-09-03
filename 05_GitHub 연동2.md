# GitHub(원격저장소) 연동


## 5. 원격 저장소와의 네 가지 상호 작용

- 클론(clone) : 원격 저장소 복제하기
- 푸시(push) : 원격 저장소에 밀어 넣기
- 패치(fetch) : 원격 저장소를 일단 가져만 오기
- 풀(pull) : 원격 저장소를 가져와서 합치기

---
### (1) 생성된 로컬 저장소와 원격 저장소 연결

생성된 로컬 저장소와 깃허브의 레파지토리인 원격 저장소를 연결할 수 있다.

#### 1) 소스트리에서 Remotes 명령 실행

[해당 로컬 저장소(study_git) 선택]> [설정] 메뉴 실행<br>
<img width="700" title="" src="../git_images/gh2-001-image.png">
<br>

[추가] 메뉴 클릭선택]> [설정] 메뉴 실행<br>
<img width="700" title="" src="../git_images/gh2-001-image.png">
<br>
---

  
### (2) 클론(clone)

깃허브상에 존재하는 원격 저장소를 여러분의 컴퓨터, 즉 로컬로 복사하여 가져오는 방법이다. 여러분이 직접 만든 원격 저장소 뿐 아니라 깃허브상에 공개된 모든 원격 저장소를 자신의 컴퓨터로 클론하여 가져올 수 있다.

#### 1) 원격 저장소 주소 복사하기

[해당 레파지토리 선택]> [Code] > [SSH] > 복사하기 아이콘 클릭<br>
<img width="700" title="" src="../git_images/gh2-01-image.png">
<br>

#### 2) 소스트리와 원격 저장소 연결

복제할 원격 저장소 선택 후 클론 버튼 클릭
<img width="500" title="" src="../git_images/gh2-02-image.png">
<br>

목적지 경로를 git-test-clone 으로 변경
<img width="500" title="" src="../git_images/gh2-03-image.png"><br>


```
ls 
ls -a git-test-clone
```
생성된 git-test-clone 폴더 확인
<img width="700" title="" src="../git_images/gh2-04-image.png">
<br><br>

소스트리에서 git-test-clone 확인 후 더블클릭 실행
<img width="700" title="" src="../git_images/gh2-05-image.png"><br>
<img width="700" title="" src="../git_images/gh2-06-image.png"><br>


#### 3) VSCode에 git-test-clone 폴더 추가하기

[File] > [Add Folder to Workspace..] 선택 <br>
<img width="700" title="" src="../git_images/gh2-07-image.png"><br>

연결된 git-test-clone 폴더에 README.md 파일 생성
<img width="700" title="" src="../git_images/gh2-08-image.png"><br>


워크스페이스에 등록된 git-test-clone의 파일 확인 후 commit 버튼 실행
<img width="700" title="" src="../git_images/gh2-09-image.png"><br>


커밋한 파일을 소스트리에서 확인한다.
<img width="700" title="" src="../git_images/gh2-10-image.png"><br>


원격 저장소에 보낼 파일 선택 후 push 버튼 클릭
<img width="700" title="" src="../git_images/gh2-11-image.png"><br>

전송 완료 후 [origin/main] 추가 된 것을 확인할 수 있다.  
<img width="700" title="" src="../git_images/gh2-12-image.png"><br>

원격 저장소의 git-test 레파지토리에 전송된 파일을 확인한다.
<img width="700" title="" src="../git_images/gh2-13-image.png"><br>

** README.md 파일 전송 후 VSCode에서도 직접 commit과 push를 실행할 수 있다!!!! ** 




