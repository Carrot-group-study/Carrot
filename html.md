내용 출처 => [웹 프로그래밍 튜토리얼](https://poiemaweb.com/)
<br>
바로가기<br>
[1.프런트엔드 개발자 학습 방향](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#1%ED%94%84%EB%9F%B0%ED%8A%B8%EC%97%94%EB%93%9C-%EA%B0%9C%EB%B0%9C%EC%9E%90-%ED%95%99%EC%8A%B5-%EB%B0%A9%ED%96%A5) <br>
[2.HTML5기본문법](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#2html5%EA%B8%B0%EB%B3%B8%EB%AC%B8%EB%B2%95) <br>
[3.시맨틱 요소와 검색 엔진](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#3%EC%8B%9C%EB%A7%A8%ED%8B%B1-%EC%9A%94%EC%86%8C%EC%99%80-%EA%B2%80%EC%83%89-%EC%97%94%EC%A7%84) <br>
[4.웹페이지의 구성하는 기본 태그](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#4%EC%9B%B9%ED%8E%98%EC%9D%B4%EC%A7%80%EC%9D%98-%EA%B5%AC%EC%84%B1%ED%95%98%EB%8A%94-%EA%B8%B0%EB%B3%B8-%ED%83%9C%EA%B7%B8) <br>
[5.텍스트 관련 태그](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#5-%ED%85%8D%EC%8A%A4%ED%8A%B8-%EA%B4%80%EB%A0%A8-%ED%83%9C%EA%B7%B8) <br>
[6.HTML의 핵심 개념인 Hyperlink](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#6html%EC%9D%98-%ED%95%B5%EC%8B%AC-%EA%B0%9C%EB%85%90%EC%9D%B8-hyperlink) <br>
[7.목록, 표 형식을 위한 태그](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#7%EB%AA%A9%EB%A1%9D%EA%B3%BC-%ED%91%9C-%ED%98%95%EC%8B%9D-%ED%91%9C%ED%98%84%EC%9D%84-%EC%9C%84%ED%95%9C-%ED%83%9C%EA%B7%B8)<br>
[8.멀티미디어(이미지, 동영상, 음악) 지원 태그](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#8%EB%A9%80%ED%8B%B0%EB%AF%B8%EB%94%94%EC%96%B4%EC%9D%B4%EB%AF%B8%EC%A7%80-%EB%8F%99%EC%98%81%EC%83%81-%EC%9D%8C%EC%95%85-%EC%A7%80%EC%9B%90-%ED%83%9C%EA%B7%B8)<br>
[9.사용자와의 커뮤니케이션](https://github.com/Carrot-group-study/NextToCarrot/blob/main/html.md#9%EC%82%AC%EC%9A%A9%EC%9E%90%EC%99%80%EC%9D%98-%EC%BB%A4%EB%AE%A4%EB%8B%88%EC%BC%80%EC%9D%B4%EC%85%98)<br>






# 1.프런트엔드 개발자 학습 방향

# 2.HTML5기본문법
Hyper Text Markup Language(HTML)<br>
Markup Language(마크업 언어)=Content(내용)+Structure(구조) => 구조화<br>

구조
```
<!DOCTYPE html>
<html>
<head></head>
<body></body>
</html>
```

comment, 주석
```
 <!--  -->
```

element, 요소
```
중첩
빈요소
```

Attribute, 속성<br>
속성은 요소의 특성을 정의하고, 속성에 대응하는 값을 가지고있다.
```
**Global Attribute(대부분의 요소에 글로벌하게 사용할 수 있는 )**
accesskey
autocapitalize
class
id
contentedittable
data-*
dir
draggable
exportparts
hidden
inputmode
is
itemid
itemprop
itemref
itemscope
itemtype
lang
part
slot
spellcheck
style
tabindex
title
translate
```

# 3.시맨틱 요소와 검색 엔진
검색엔진, SEO(크롤러-크롤링, 인덱서-인덱싱)<br>

Semantic Element의 중요성<br>

브라우저 ↔ 개발자 ↔ 검색엔진<br>

Semantic Web이란?<br>
 non-Semantic Element<br>
 Semantic Element<br>

# 4.웹페이지의 구성하는 기본 태그<br>
구조
```
<!DOCTYPE html>
<html>
<head></head>
<body></body>
</html>
```

1)문서 형식 정의 태그(DTD, Document Type Definition)<br>
브라우저에게 출력할 문서의 형식 지정<br>
대소문자 구별 X<br>
대부분의 웹개발은 html5로 이루어진다. HTML5 DTD=<!DOCTYPE html><br>

2)<html></html><br>
	모든 요소의 부모요소 = <html></html>를 제외한 모든 요소는 html요소의 자식 요소. 따라서, 모든 요소는 html요소 내부에 기술 단, DTD는 예외. 하나만 존재<br>
	
	3)<head></head><br>
		메타데이터 기술<br>
		화면관련 요소 포함X<br>
		단 하나만 존재<br>
		title, style, link, script, meta-keywords, description, author, charset등<br>
	4)<body></body><br>
메타데이터를 제외한 모든 요소가 포함되는 요소= 화면관련 및 구조관련 태그는 body요소의 자식요소. 단, 하나만 존재<br>
      
# 5. 텍스트 관련 태그
제목 태그(semantic)
```
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```

글자 형태 태그
```
b vs strong(semantic)
i vs em(semantic)
del vs ins
sub vs sup
small
mark
```

본문 태그
```
p
pre
강제기행br*연속공백&nbsp;
hr
q(짧은인용문) vs blockquote(긴 인용문)
```

# 6.HTML의 핵심 개념인 Hyperlink
Hyperlink = 특정 텍스트에서 다른 텍스트로 건너뛰어 읽을 수 있는 기능<br>

Hyperlink기능 => <a></a>요소가 담당<br>

<a></a><br>
속성="값"<br>
  href="파일경로(절대경로,상대경로), fragment identifier, mailto:, script"<br>
  target="_self, _blank"<br>

**target="_blank"의 취약점**<br>
 1)피싱공격(Tabnabbing)<br>
 2)피싱공격에 대비하여 rel="noopener noreferrer" 사용<br>
 3)피싱공격의 원인 : window.opener.open()으로 창을 열면, 부모창 참조 가능<br>
 4)"_blank"값을 가지는 a tag를 포함하여 area, base, form tag도 주의<br>

# 7.목록과 표 형식 표현을 위한 태그
목록<br>
네비게이션 메뉴 생성 할 때 자주 사용<br>
목록의 중첩(ol 안에 ul이 포함될 수 있고 ul안에 ol이 포함될 수 있다.)
```
<ul>
<li></li>
</ul>

<ol>
<li></li>
</ol>
```
```
	type 
		1(숫자 일, 하나)
		A(영문대문자, 에이)
		a(영문소문자, 에이)
		I(영문대문자, 아이)
		i(영문소문자, 아이)
	start
	reversed
```
<br>
표<br>
과거 레이아웃을 구성하는 경우에 사용
현재 레이아웃은 영역관련 태그를 사용
<br>
<table border="2"> <!--border="2"는 표의 구조를 직관적으로 확인하기 위해서 설정함.-->
	<caption>제목1</caption>
	<tr>
		<th>종류1</th>
		<th>종류2</th>
		<th>종류3</th>
		<th>종류4</th>
		<th>종류5</th>
	</tr>
	<tr>
		<td>테이블 내용1</td>
		<td>테이블 내용2</td>
		<td>테이블 내용3</td>
		<td>테이블 내용4</td>
		<td>테이블 내용5</td>
	</tr>
</table>
<br>
<table border="2"> <!--border="2"는 표의 구조를 직관적으로 확인하기 위해서 설정함.-->
	<caption>제목2</caption>
	<tr>
		<th>종류1</th>
		<td>테이블 내용1</td>
	</tr>
	<tr>
		<th>종류2</th>
		<td>테이블 내용2</td>
	</tr>
	<tr class="lightBlue">
		<th>종류3</th>
		<td>테이블 내용3</td>
	</tr>
	<tr>
		<th>종류4</th>
		<td>테이블 내용4</td>
	</tr>
	<tr>
		<th>종류5</th>
		<td>테이블 내용5</td>
	</tr>
</table><br>

<br>
테이블 제목<br>
-table의 자식태그로 <caption></caption>사용<br>
-caption 테이블의 제목을 나타낸다(기본:가운데)<br><br>
<br>테이블 병합<br>
tr의 자식태그인 th와 td태그의 속성으로 사용<br>
-colspan(해당 셀이 점유하는 "행-가로-왼쪽에서 오른쪽" 수 지정)<br>
-rowspan(해당 셀이 점유하는 "열-세로-위에서 아래" 수 지정)<br>
<br>

# 8.멀티미디어(이미지, 동영상, 음악) 지원 태그
1.이미지
```
빈요소
<img
	src="경로"
	alt="이미지표시가 안될 경우 나타내는 문장">
```

2.동영상
```
<video
	src="경로"
	poster="동영상 대기중에 표시할 이미지 경로"
	preload(재생전에 음악파일 모두 불러올지 여부)
	autoplay(자동재생여부)
	loop(반복재생여부)
	controls(음악재생도구표시여부-브라우저마다상이)
	width="너비지정"
	height="높이지정">
</video>
```

3.음악
```
<audio
	src="경로"
	preload
	autoplay
	loop
	controls>
</audio>
```

# 9.사용자와의 커뮤니케이션
|tag|attribute|value|
|---|---|---|
|input|type||
|||text|
|||button|
|||number|
|||password|
|||date|
|||datetime|
|||datetime-local|
|||month|
|||week|
|||time|
|||email|
|||file|
|||hidden|
|||image|
|||color|
|||checkbox|
|||radio|
|||range|
|||reset|
|||search|
|||submit|
|||tel|
|||url|
