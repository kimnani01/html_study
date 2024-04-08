# Visual Studio code(VScode)
* vs code 실행 시 가장 먼저 확인해야할 것!
* 왼쪽 탐색기가 당일 작업 폴더로 연결되어 있는지 확인하기!
* (위) 안되있다면 -> 파일 -> 작업폴더닫기 후 -> 폴더열기 다시 진행!
# html 시작
* git, gitHub 개념공부
* `<태그>` 웹페이지에서 의미적인 정보를 가지는 대상
## HTML5 버전선언
* `<!doctype html>`
## HTML 구조태그
* html : 웹의 시작과 끝. 문서 자체 의미.
* head : 웹 문서의 정보, 제목 포함
* meta : 웹 문서의 정보 기록
* title : 웹 문서의 제목(브라우저 상단 표시)
* body : 웹 문서 내용(실제 대부분의 서비스가 들어가는 본문)
## 구조 태그 속성
* `lang="ko"` html문서 언어 설정
* `charset="utf-8"` 다국어 문자열 설정
* `description` 사이트 요약 설명
* `keywords` 사이트 검색 키워드 설정
## 속성 문법
* `<태그 속성="값" 속성="값"></태그>`
* 태그와 속성 사이 공백
* 속성과 속성 사이 공백(속성 개수 제한없음)
* 속성은 시작태그에만 작성하기!
## 구조태그의 `title` 작성방법
* 메인페이지 -> 사이트명
* 메인페이지 -> 사이트명 | 광고문구추가
* 서브페이지 -> 페이지명 | 사이트명
* ex) 책이름 - 저자명 | 서점명
* ex) 판매아이템명 | 사이트명
## h1~h6 제목태그(block tag)
* h1~h3 태그는 meta keywords와 동일한 검색키워드로 활용된다. (대제목일수록 높음)
* h4~h6은 거의 사용하지 않는다.
* h1 대제목은 사이트의 로고 및, 서브 페이지 제목에서 주로 사용한다.
* h 제목의 1~6레벨은 순서대로 작성해야 한다.
## 단락 p(block tag)
* 한 줄 또는 여러 줄 단락 묶을 때 사용하는 태그
* 제목(h)태그 종류와는 형제 태그 관계로 사용해야 한다ㅏ. 부모-자식(x)
## 인라인태그 br, em, strong, del, s, sup, sub
* `br` : 블록 내 줄바꿈 태그
* `em` : 블록 내 강조 태그, 주로 내용 태그(p) 등에서 자식으로 사용
* `strong` : 블록 내 경고용 강조 태그 (위와 특징 동일)
* `del` : 삭제 텍스트, 쇼핑몰의 할인 전 가격 등에 사용
* `s` : 교체 텍스트, 쇼핑몰의 할인 전 가격 등에 사용(del 자주 사용)
* `sub, sup` : 윗첨자(sub), 아래첨자(sup) 수학, 과학 등의 기호에 사용
## 인용문 처리 blockquote, q
* `blockquote(block)` : 단락 자체가 인용문에 해당할 때 사용, p태그와 부모-자식 관계로 사용해선 안된다!
* `q(inline)` : 단락(p) 내에서 일부가 인용문에 해당할 때 사용
* 공통 속성 `cite="URL"` : `blockquote`, `q` 로 인용문 처리할 경우 출처 표시용도로 주소(URL)를 담아주는 속성.
## 특수문자 태그
* `&` 시작 `;` 종료
* ex) `&lt;``&gt;``&copy;``&reg;`
## 주소태그
* `address(block)` : 웹사이트의 관련 연락처, 소개, 고객센터 정보 등을 담을 때 사용
* footer 영역에 주로 사용
## 수평선 태그
* `hr(block)` : 복잡한 html 태그 경계 사용
* 주석과 같이 태그 구조 이해에 주로 사용
## 컴퓨터 명령어 태그
* `code(inline)` : 웹 강의 사이트에서 주로 사용하는 태그
## 하이퍼링크 태그 <a>
* block, inline 특징을 모두 가진다.
* 절대경로와 상대경로를 href 속성에 작성한다.
* 상대경로는 a태그 작성 중인 파일 위치 기준 연결하고자 한느 목적지 파일이 같은 위치에 있는지, 하위 위치에 있는지, 상위 위치에 있는지에 따라 다르게 작성한다.
* ./ 현재 위치에서 시작
* ../ 상위 폴더로 나가기
* `./doll.jpg` : 현재 위치에서 doll.jpg 파일 찾기
* `../doll.jpg` : 상위폴더로 한단계 나가서 doll.jpg 파일 찾기
* `../a/doll.jpg` : 상위폴더로 한단계 나가고 a 폴더로 들어가서 doll.jpg 파일 찾기
* `./b/doll.jpg` : 현재위치에서 b 폴더로 들어가서 doll.jpg 파일 찾기
## 바로가기링크란?
* `a href="#id"`
* 단순 페이지 이동이 아닌 특정 위치로 스크롤 이동하는 바로가기 기능
## 바로가기 링크 제작 순서 및 주의사항
1. 이동 목적지에 가장 가까운 태그에 `id` 적용하기
2. 링크 대상에 `#id` href 속성값에 담기
* 주의사항 : #은 아이디 이동 링크에만 사용하기
## 파비콘 적용 순서
1. 파비콘 크기로 이미지 다운받거나 편집하기
2. html에서 head 안에 link태그로 `favicon` href주소 연결하기
## 이미지태그 `img(inline)`
* `img src="url" alt=""`
* src 이미지 경로 속성의 값으로는 상대경로 방식으로 작성하는 것을 권장
* 대체텍스트 alt 속성을 필수 작성
* 이미지 사용시 의미전달이 필요한 이미지와 아닌 이미지를 구분해서 사용
## figure(block), figcaption(inline) 태그
* 문서 안 사진을 감싸는 틀로서 활용하고 사진의 캡션을 정의할 수 있다
## video 태그
* `<video src="동영상경로></video>"` 
* 원하는 유튜브 영상 우클릭 > 소스코드 복사 > 붙여넣기
* `<iframe src="https://www.youtube.com/embed/동영상주소?속성=값&속성=값">`
* autoplay=1 자동재생 
* mute=1 음소거
* loop=1 반복재생
## class, id 많이 사용하는 키워드
* wrapper, wrap, area 전체 묶는 영역
* contents, container 중~소 묶는 영역
* group, g 간단한 소그룹 영역
* top, btm, left, right 레이아웃 방향을 의미하는 키워드
* 예 : 의미있는단어_영역명
* 예시 : product_wrap, item_area, price_g, main_contents, top_btn
## div, span 그룹태그
### div
* 인라인과 블록이 2개 이상 형제일 경우 묶어주는 그룹태그
* 레이아웃 기준 1행에 2열 이상 배치일 경우
* 특정 의미를 가진 행에 같은 디자인 요소가 배치된 경우
### span
* 인라인이 2개 이상 형제일 경우 묶는 그룹태그
* 의미없는 디자인 요소 인라인 처리 필요 시 사용
