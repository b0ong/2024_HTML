# HTML 교육
## DAY01
 ### HTML 기본 생성
#### 기본 틀
     ```html
        <!DOCTYPE html>
        <html lang="en">
        <head>
            <meta charset="UTF-8">
            <title>Title</title>
        </head>
        <body>
        
        </body>
        </html>
    ```
- 세부사항
  - head: 창에서 제목 부분 구글에서 탭에 해당함
  - title: 제목 구글 탭에서 제목이 정해짐
  - body: 화면에서 전체 창에 표시됨

- h1,h2,h3,h4... : 웹페이지에서 숫자에 따라 제목, 부제목 등 으로 나뉘어짐
  - title 밑에 link rel="stylesheet" href="style.css"/ 를 넣으면 css로 연결
    - 이럴경우 css파일을 추가 생성해야함.
    - rel : 속성, stylesheet : 값 
    - href : 속성, 위치경로를 의미함.
    ```html
    h1{
    color: white;
    background: black;
    }
    h3{
    color: yellow;
    background: blue;
    }
    ```
  - css 파일을 생성할 경우 글자 색이나 뒷배경 색을 지정할 수 있음.
    - h1,h2,h3... 은 해당 html파일에 있는 h1,h2,h3...이랑 같은 컬럼임.
#### 공백 띄우기
  - html에서 공백을 할려면 space로는 인식이 안됨
  - &nbsp로 해야 인식함. (' ; ' 를 붙여야함)

![공백 띄우기](https://github.com/b0ong/2024_HTML/blob/main/images/space.png)
#### Script
  - Script는 웹사이트를 열었을 때 알림창 같은 새 창을 여는 것임
#### 줄바꿈
  - hr 태그는 줄을 만들어 분리시키는 느낌을 줌

![hr사용예](https://github.com/b0ong/2024_HTML/blob/main/images/hr.png)

  - p 태그는 문단을 만든다.
  - br 태그는 줄바꿈, 시작태그가 없음. (enter느낌)
#### 링크삽입
  - 링크 삽입은 a href를 사용한다. (ex: a href="http://naver.com")
  - 위 경우는 새창이 열어지지 않고 현재 창에서 바로 들어가짐
  - 새창열기는 (a href="http://naver.com"target="_blank") 처럼 target, _blank 를 사용하면 됨