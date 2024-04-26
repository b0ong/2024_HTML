# HTML 교육
## DAY05
- 클래스 속성은 중복될 때
- id는 고유한 식별자
- 입력을 할 때는 form태그를 사용! 서버로 입력받은 내용을 넘겨야 하기 때문에!

### 속성
```html
<head>
    <meta charset="UTF-8">
    <title>attiribute</title>
  <style>
    input[type="text"] {
      background: aqua;
    }
    input[type="password"] {
      background: green;
    }
  </style>
</head>
<body>
<form>
  <input type="text">
  <input type="password">
</form>
</body>
```
- 속성선택자: 대괄호를 사용한다. 선택자[속성=값], input태그의 type속성에 사용
![img.png](images/attiribute.png)
- head부분에 style태크 사용함.

### DESC
```html
<head>
    <meta charset="UTF-8">
    <title>DESC</title>
    <style>
        #header > h1 {
            color: green;
        }
        #section > li{
            color: orange;
        }
    </style>
</head>
<body>
<div id="header">
<h1>CSS 선택자 기본</h1>
<h2>기본 선택자</h2>
<ul id="section">
  <li>전체 선택자</li>
  <li>태그 선택자</li>
  <li>아이디 선택자</li>
  <li>클래스 선택자</li>
</ul>
</div>
</body>
```
- 자식선택자: > 표시로 자식관계를 나타낸다.\
![img.png](images/desc.png)
- #을 쓴이유는 id이기때문에 사용함.
```html
<head>
    <meta charset="UTF-8">
    <title>Title</title>
  <style>
    #header > h1{
      color: red;
    }
    #section h1 {
      color: #dbad3b;
    }
  </style>
</head>
<body>
<div id="header">
  <h1 class="title">후손 선택자</h1>
  <div id="nav">
    <h1>Navigation</h1>
  </div>
</div>
<div id="section">
  <h1 class="title">애국가</h1>
  <p>
    동해물과 백두산이 마르고 ...
  </p>
</div>

</body>
```
- header id의 후손인 모든 h1태그에 적용, nav id자식인 h1태그도 적용
- #header h1, h2 {color: red;}
- #header h1, #header h2 {color: red;}\
![img_1.png](images/desc1.png)

### DESC Table
```html
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<style>
  table >tbody > tr > th {
    color: aqua;
  }
</style>
<body>
<table border="1">
  <tr>
    <th>이름</th>
    <th>지역</th>
  </tr>
  <tr>
    <td>장경호</td>
    <td>부산 수영구 망미동</td>
  </tr>
</table>
</body>
</html>
```
- table 태그는 주의해야함
- 개발자 모드에서 확인하면 table 태그에 tbody태그가 자동으로 추가되어 있음.\
따라서 table > tbody > tr > th 순으로 해야함\
![img_1.png](images/Checking_source.png)
![img_2.png](images/desc_table.png)
### Action
```html
<head>
    <meta charset="UTF-8">
    <title>반응 선택자</title>
    <style>
        h4:hover {
            color: red;
        }
        h4:active {
            color: aqua;
        }
    </style>
</head>
<body>
<h4>반응 선택자</h4>
</body>
```
- 반응선택자: 사용자의 반응으로 hover와 action상태가 만들어 진다.
- 마우스의 커서를 올리는 행위가 hover적용, 클릭하면 action적용.\
![actionExample](images/actionExample.mov)