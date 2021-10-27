[헤리터 갤러리 리스트 페이지]
홈디렉토리 =>
D:\webPub_0513\kjj\ex\Part03_BBS
   \p02_GalleryList_Heriter
html => bbs/galleryList.html
css => style/style_Reset.css
                /style.css
js  =>  script/jquery-3.6.0.min.js
                 /script.js
img   => images/

-------------------------------------


[Design]
1. 스타일링 - 포샵, CSS 등을 사용하여
                  화면을 시각적으로
                  돋보이도록 만드는 작업
2. 기획 - 설계를 의미함.


[설계(Design) 작업]
1. 헤더영역
    => div#joinEventArea>div#joinEventWrap

         div#outerHeaderArea
            >header#headerWrap
              >div#headerLogoArea + 
                (div#headerMenuArea
                      >nav#headerLNB + 
                        div#cartNsideGNB)

  1) 이벤트
    회원가입하면 16만원 쿠폰팩 이벤트 영역
  2) 헤더영역
      로고 + 헤더LNB(주문, 로그인, 회원가입)
             +  장바구니 +
       사이드GNB메뉴 버튼


2. Top버튼 + 카카오 회원가입버튼
    => div#sideFixedArea>
           div#topBtnArea + div#cacaoJoinArea

3. 사이드 GNB 메뉴
   => nav#sideGNBArea >
       div#eventMsgArea 
            1) 쿠폰 즉시 발급 안내 텍스트 : 
                회원가입하면 16만원 쿠폰팩 
            2) 목록, 닫기 버튼은 
                header#headerArea에서 제작

        + div#sideMenuLNB(cart, order, login)
        + ul#mainMenu


=> 와이어프레임


참고. 포트폴리오에서
       작업대상을 선정했고,
       벤치마킹 사이트도 지정했으며
       어떤 작업을 진행할건지 목록을 작성하고
       (메인페이지, 게시판, 상품목록, 회원가입,
        로그인, 장바구니, 기타 등등 본인이 
        필요하다고 생각하거나 또는 만들고 싶은 것들에
        대한 목록 작성, 스스로 만들기 어렵다고
        판단하면 제외하고 작업진행)
        진행할 작업목록이 작성되었다면
         각 작업에 대한 와이어프레임을 제작함.

------------------------------------------------------

4. div#wrap
5. footer 작업



---------------------


[Github 2021.8월 이후 추가 인증방식 적용]
1. 로그인
2. 우측 상단 [마이페이지] 아이콘 클릭
   => 펼침메뉴 하단에 [Settings] 클릭
3. 좌측 [Accounts settings] 사이드 메뉴 하단 
   [Developer settings] 클릭
4. [Developer settings] 사이드 메뉴 하단 
   [Personal access tokens] 클릭
5. [Personal access tokens] 제목 오른쪽
    [Generate new token] 버튼 클릭
6. [New personal access token] 내용 입력
   1) Note => 본인이 지정하는 토근 이름
         본인아이디_날짜_기타내용
         zzupd_211018_AccessToken
   2) Expiration (토근 유효 기간 설정)
        본인이 임의 설정
   3) Select scopes (접속 허용 범위 설정)
       => repo 전체 체크
   4) 하단의 [Generate token] 클릭    
7. 생성된 토큰 코드 별도 보관 
   => 보기. 훈련교사 토큰 

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

 --------------------------------------- Github 토큰 설정
+  VSC 접속 설정




[접속 인증 토큰을 사용한 깃허브 접속]

1. 접속인증 토큰
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
2. 저장소(Repository, 리포지터리)
3. VSCode에서의 접속


GNU(그누, 누) => 사용무료저작권,
                        수정 및 배포 무료 저작권
                        프로그램 자체를 판매 못함
                        수정하여 프로그램 판매 못함.
                        소스가 공개되어 있음(=오픈소스)

GPL => General Public License

                       
---------------------------------------------

[Git Bash 깃 배쉬]
=> 밍위, 밍더블유, 민지

MINGW


git config --list
=> 깃 관련 세팅 정보 출력



현재 작업상황
1. Git 프로그램 삭제 후 설치
   (Github와 무관함)
2. Github에 로그인 후 Token 발급받음
3. Github에 저장소(Repository, 리포지터리) 생성
4. 본인의 컴퓨터에서
   Github에 접속할때 필요한
   ID(=user.name)와 Email(=user.email) 을
   Git Bash에서 전역 환경변수로 등록 =>

   $ git config --global user.name 본인ID
   $ git config --global user.email 본인Email

   올바르게 등록되었는지 확인 =>
   $ git config --list
5. VSCode 작업
  1) 업로드(=형상관리 대상)할 홈디렉토리 선정
      및 프로그램 작성 후 최종 저장
      참고. 형상관리 = 버전관리
  2) VSCode에서 Git을 사용하는 아이콘 클릭
       또는 단축키  ctrl + sh + g
      홈디렉토리에서 깃을 처음 적용할 경우
      [리포지토리 초기화] 버튼이 나타남 
   3) [리포지토리 초기화] 버튼 클릭    
   4) [변경 사항]에 마우스를 위치하면
       [+] 기호 나타남 => 클릭
   5) [+] 기호를 클릭하면 상단에
      스테이징 진행 상태표시됨
      참고. 스테이징(Staging, 업로드 준비상태)
             진행 상태에서는
             각 파일 옆 기호가 "U"에서 "A"로 변경됨
   6) 스테이징 진행이 완료되면 상단에 있는
       "깃 메뉴 아이콘(...)" 클릭
   7) "깃 메뉴" 하위에 있는
      "분기" => "분기 이름 바꾸기" 클릭
       입력창이 나타나면 
       "master"에서 "main"으로 수정 후 엔터
   8) "깃 메뉴 아이콘(...)" =>
       "커밋" =>
       "스테이징 된 항목 커밋" 클릭 =>
       입력창에서 처음 입력할 경우 
       Github 리포지터리 이름 입력 후 엔터
       참고. 리포지터리 이름 입력할 때 
               앞뒤 공백 제거
        => 스테이징 된 파일 목록이 사라짐   
   9) "깃 메뉴 아이콘(...)" =>
       "원격" =>
       "원격 추가" 클릭 후
       Github에 있는 리포지터리 
       원격 URL을 복붙하고 엔터 =>
       원격이름은 최초 입력 시 
       리포지터리 이름 입력 후 엔터
       
   10) "깃 메뉴 아이콘(...)" =>
        "풀, 푸시" =>
        "다음으로 푸시" 클릭 =>
         입력창에서 생성한 원격 URL 선택

         여기서부터 토큰보안인증 추가됨 =>
         팝업창에서 "Token" 메뉴 찾은 후 클릭 =>
         복사해둔 토큰 붙여넣기 =>
         Sign in 클릭  => Github에서 업로드여부 확인
     
    
----------------------------------------------------

1. 천단위 구분 쉼표 적용
2. 페이징
3. 헤더메뉴 스티키
------------------------------------------------------      

[천단위 구분 쉼표 적용]


<script>
let num = 1234567;    // 123,456,789
// 데이터의 자료형이 number(=숫자형)이어야 함
console.log("num(원본 값) : " + num);
let setComma = num.toLocaleString();
console.log("setComma(천단위쉼표 적용) : " + setComma);
let closeComma = setComma.replace(/,/g, "");
console.log("closeComma(쉼표 제거) : " + closeComma);
</script>


355000
298000
5491
355000
288000
243
278000
228000
2058
11800099000315299000690001601600001390001542370002060001535260002600038879000790001732390003900016039000350003297002680012





[페이징]
=> div, table, a, img를 사용하여 생성함

관련용어 
1. 블럭(Block) : 1개의 화면에 표시되는 페이지 수.
                     1~10페이지 또는 1~20페이지
                     일반적으로 1~10페이지를 사용함.
                      보기. 11~20페이지
                             21~30페이지
2. 이전 블럭,   다음 블럭
   previous      next
   block          block
3. 이전 페이지, 다음 페이지
   previous       next
   page            page
4. 현재 페이지
    => 화면에 표시되는 페이지
         nowPage



                     

[헤더메뉴 Sticky 스티키]

              position: fixed;              position: sticky;

공통점              화면의 기준이 viewport (뷰포트)
                       즉, body요소 기준이 아님
                       그래서 스크롤링할 때 화면을
                       따라다니는 효과

차이점      2차원 공간이 소멸         2차원 공간이 유지
                                                left, top을 반드시
                                                적용해야만 함

               absolute의                   relative의
               특징을 갖는다.              특징을 갖는다
               (2차원 공간 소멸,           (2차원 공간 유지,
                3차원에서 겹침)            3차원에서
                                           자신의 영역 유지하므로
                                          left, top, bottom, right를
                                           적용하지 않으면 
                                           겹침없음)

