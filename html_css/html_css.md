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