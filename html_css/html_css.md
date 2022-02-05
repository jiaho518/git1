# HTML

## HTML Introduction

- HTML : Hyper Text Markup Language

  - Hyper Text : 하이퍼링크로 연결된 웹 문서 => 웹 문서(페이지)
  - Markup Language : 표시 언어

- HTML 표시내용

  - Web Page의 Contents(내용)
    - Text Contents
    - Multimedia Contents : image, video, audio
      - Embedded Contents
  - Web Page의 Structure(구조)

- 학습 내용
  - 문법
  - 활용

## HTML Basic

- 기본구조

  ※ ` : backtick

  ```
  <!DOCTYPE html>
  <html>
    <head>
      웹 문서의 부가정보
    </head>
    <body>
      웹 문서의 내용
    </body>
  </html>
  ```

## HTML Element

- Tag와 Contents로 구성
- Tag는 시작태그와 종료태그로 구성
  - contents와 종료태그 없이 시작태그만 있는 요소 : 빈 요소(Empty Element)

```
<h1>제목</h1>

<br> => 빈 요소(Empty Element)

빈 요소 문법에 " / " 
```

## HTML Attribute

- HTML Tag의 추가정보

- syntax(문법) : name="value" (이름/값 쌍)

```
<img src(소스)="photo.jpg" alt(alternative : 대체 텍스트)="텍스트 또는 이미지">
```

## Text Contents Element

### Heading

- 제목
- h(heading)
  - h1~ h6

### Paragraph

- p(paragraph) : 단락

- hr(Horizontal Rules) : 수평선(단락을 구분)

- br(Line Break) : 강제 줄바꿈<br>
  (※ 강제 공백(Entity Code) : &nbsp; - Non-breaking space)<br>
  (※ & : apmersand)
  - HTML Text : 줄바꿈, 공백 인식
    - 공백 1칸으로 인식

### HTML List

- 순서없는 목록 : ul, li
- 순서있는 목록 : ol, li
-설명 목록 : dl, dt, dd

※ 포함관계/중첩관계(Nested Element)
- 포함하는 요소 : 부모요소(Parent), 조상요소(Ancestor)
- 포함되는 요소 : 자식요소(Child), 자손요소(Descendant)
- 이웃하는 요소 : 형제요소(sibilng)

### HTML Link

-하이퍼링크 연결


- a(anchor)
  - href(hypertext reference) attribute : 연결되는 페이지의 주소 정보
  - target attribute : 새탭 열기 설정
    - target="_blank" : 새탭 열기

- Bookmark 기능
  - 목적지에 id attribute를 사용해서 이름 지정
  - a 태그의 href 속성에 "#이름" 으로 표시

### HTML Table

- 표를 표시
- table(표 영역)
- tr(table row) : 행
- th(table heading) : 각 열의 제목
- td(table data) : 열 or 칸
- table generator
https://www.tablesgenerator.com/html_tables

## Multimedia Contents

### HTML image

- attribute(속성)
  - src(sourc) : 이미지의 파일 경로, 이름
  - alt(altanative) : 대체 텍스트 또는 이미지

### HTML Video

- video tag
-attribute(name만 사용하는 형태)
  - controls : 동영상 컨트롤(재생/일시정지/오디오) 버튼 표시 여부
  - autoplay : 자동 재생
  - muted : 음소거
  - loop : 반복 재생
  - poster : 영상 대체 이미지(썸네일)

## Semantic Element

- 영역을 구분하는 Element를 의미있게 사용하는 것

- header : 로고, 로그인 메뉴, 언어변경 등 상단 바
- nav(navigation) : gnb(global navigation bar / 메인영역), lnb(local navigation bar / 내부영역)
- section : 웹 페이지의 본문 / 영역 구분
- article : 웹 페이지의 본문 / 독립된 글or내용
- aside : 부수적인 내용 / 광고 배너
- footer : 웹 사이트의 하단 부분(위치 정보 및 관련 링크 등등)
- figure : 다이어그램/이미지 시작 요소
- main : 웹 페이지 본문 전체

## URL / File Path

- URL(Uniform Resource Locator)

```
https://www.naver.com/video/movie.mp4

=> https://도메인네임/상세경로(:포트번호)

IP 주소 : Internet Protocol 주소 => 인터넷에서 사용하는 실제 주소

Ex) 192.168.0.1 : 0~255까지의 숫자 4개로 구성

도메인 네임 : 영어 단어(줄임말)로 구성되어 있는 식별 이름

도메인 네임 서버(시스템) : 도메인 네임 => IP 주소로 변환
 
```

- 경로(URL/File Path) 지정 방식
  - root : 해당 경로의 가장 시작하는 위치
  - 절대 지정 방식
    - 파일 경로의 전체 URL을 표현하는 방식
  - 상대 지정 방식
    - 현재 페이지를 기준으로 일부 URL을 표현하는 방식
    - root 상대 경로 방식 : root를 기준으로 상대적인 URL 표현
```
Domain : www.abc.com

/(root) - html - Ex)index.html 
        - images - photo.jpg

절대 방식 : https://wwww.abc.com/images/photo.jpg

상대 방식(현재페이지 : index.html) : ../images/photo.jpg

root 상대방식 : /images/photo.jpg
```

## HTML Head

- head element
  - title : 웹사이트 제목(브라우저 탭에 표시)
  - meta* : 웹사이트 관련 정보
  - link : css 파일 불러오기
  - style : css 코드 작성
  - script : js 코드 작성 / 파일 불러오기

- meta
  - charset(character set) : 문자 set - 글자(문자)를 표시하는 방식
  - 종류/개수 => 용량
    - bit : 0/1이 저장되는 공간
    - 1bit가 저장/표현할 수 있는 개수(가짓수) : 2가지
    - 2 * 2 * 2 * 2 => 4 bit = > 16개
    - 1 byte = 8 bit => 256개 (byte < KB < MB < TB < PB ...)

  - UTF-8 : 글자(문자) 표기 방식 중 하나
    - UTF(Universal Coded Character Set + Transformation Format – 8-bit)
