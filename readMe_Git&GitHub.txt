[GitHub에 업로드하기]

1. PC에 Git 프로그램 설치가 되어있어야 함.
  1) 설치 => https://git-scm.com 다운로드
                 다운로드 후 설치실행(순서대로 클릭)
  2) 삭제 => 윈도우키+R => appwiz.cpl
                 => Git 항목을 찾은 후 우클릭하고 삭제 클릭
  3) 설치 후 정상설치 확인 => 시작메뉴 버튼 클릭
                                    => Git-Bash 항목을 찾아서 클릭
                                    => Git-Bash 창에서 
                                         git --version 입력 후 엔터
                                         버전이 확인되면 정상설치 완료

2. Git Bash 프로그램을 사용한 GitHub 전역 변수 설정
   (깃 배쉬)
   1) 사용자 아이디(=사용자 이름)
       git config --global user.name  본인ID
   2) 사용자 이메일
       git config --global user.email  본인이메일

   => GitHub 홈페이지에서 회원가입할 때
        사용한 ID와 Email을 사용해야 함.

   참고. GitHub 홈페이지 => https://www.github.com
          홈페이지에서 회원가입(=> Sign Up)해야 함.

   보기. ID => zzupd
           Email => zzupd@naver.com

   3) 깃 배쉬에서 사용자이름과 사용자이메일
       등록여부 확인하기 => git config --list
       
------------------------------------------------------------

[GitHub에서의 작업]

1. ID(=사용자이름), Email(=사용자 이메일)이
   등록되어 있어야 함.
   즉, 회원가입되어 있어야 함.

2. https://www.github.com 사이트에 로그인 

3. 외부접속 인증(=허가) 토큰(Token) 
   발급받기
 1) 우측상단 "마이페이지 아이콘" 클릭
 2) "Settings" 항목 클릭
 3) 왼쪽 본인 아이디가 있는 영역에서
    (= Your personal account)
    아래쪽에 있는 항목중에서
    "Developer settings" 클릭
 4) 왼쪽 메뉴 항목에서
    "Personal access tokens" 항목 클릭
 5) "Personal access tokens" 페이지에서
     생성된 토큰이 있다면 
     토큰을 그대로 사용할지, 
     토큰을 제거하고 새로 발급받을지 결정
     (사용기한을 보고 결정하거나
      본인의 작업에 사용가능여부를 스스로
      판단하여 재사용할지 제거 후
       새로 발급받을지를 결정함.)
      => 생성된 토큰이 표시되지 않는다면
           토큰을 새로 발급받음.
           만일 토큰이 존재하는데,
           재사용여부에 대해 잘 모르겠다면
           이 경우에도 토큰을 제거하고
           새로 발급받음.
  6) 토큰 재발급 =>
      "Personal access tokens" 페이지에서
      기존의 토큰을 모두 제거 후
       "Generate new token" 버튼 클릭
  7) "New personal access token" 페이지에서
      아래 3개를 입력 후 확인버튼 클릭.
      (1) Note => 토큰 이름       
      (2) Expiration => 토큰 사용기한
      (3) Select scopes => 토큰 사용영역

  8) Note(토큰 이름) 형식 =>

      A : 토큰생성한사람
      B : 토큰생성일
      C : 업무명
      D : 옵션(=기타내용, 생략가능)

        A_B_C_D  또는 A_BC_D
        참고. 다른 형식으로 기재 가능하며
                회사마다 다름
     보기.   zzupd_211026_GalleryList_테스트용
                A         B           C           D
              또는
              zzupd_211026_GalleryList               
              또는
              zzupd_211026GalleryList               

   9) Expiration (토큰 사용할 수 있는 기간)
       => 7 days 를 설정했으나
            본인이 원하는 기간을 선택하거나
            입력하면 됨.

   10) Select scopes(토큰 사용영역)
        => repo 만 체크하며
             아래쪽 항목들은 자동 체크됨
            (= repository를 의미함, 저장소)

   11) "Generate token" 버튼 클릭하여
         토큰 생성
        주의!  토큰 코드는 따로 복사해둠.
                 (다신 못 봄)

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

------------------------------------------------------------

4. 저장소 생성

-------------------------------------------------------

5. Visual Studio Code 에서 Git을 사용한 
 GitHub에 연동하고 업로드하기









