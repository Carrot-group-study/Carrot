바로가기<br>
[프런트엔드 개발자 학습 방향](#-1.프런트엔드-개발자-학습-방향)<br>
[HTML5기본문법](#-2.html5-기본-문법)<br>
[시맨틱 요소와 검색 엔진](#-3.시맨틱-요소와-검색-엔진)<br>
[웹페이지의 구성하는 기본 태그](#-4.웹페이지의-구성하는-기본-태그)<br>
[텍스트 관련 태그](#-5.-텍스트-관련-태그)<br>
[HTML의 핵심 개념인 Hyperlink](#-6.HTML의-핵심-개념인-Hyperlink)<br>






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

<!DOCTYPE html><br>
  1)문서 형식 정의 태그(DTD, Document Type Definition)<br>
    브라우저에게 출력할 문서의 형식 지정<br>
  2)대소문자 구별 X<br>
    대부분의 웹개발은 html5로 이루어진다. HTML5 DTD가 <!DOCTYPE html><br>

<html></html><br>
  모든 요소의 부모요소 = <html></html>를 제외한 모든 요소는 html요소의 자식 요소<br>
  따라서 모든 요소는 html요소 내부에 기술 단, DTD은 예외<br>
  단 하나만 존재<br>

    <head></head><br>
      메타데이터 기술<br>
      화면관련 요소 포함X<br>
      단 하나만 존재<br>
      title, style, link, script, meta-keywords, description, author, charset등<br>

    <body></body><br>
      메타데이터를 제외한 모든 요소가 포함되는 요소= 화면관련 및 구조관련 태그는 body요소의 자식요소<br>
      단 하나만 존재<br>
      
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

target="_blank"의 취약점<br>
  1)피싱공격(Tabnabbing)<br>
  2)피싱공격에 대비하여 rel="noopener noreferrer" 사용<br>
  3)피싱공격의 원인 : window.opener.open()으로 창을 열면, 부모창 참조 가능<br>
  4)"_blank"값을 가지는 a tag를 포함하여 area, base, form tag도 주의<br>
