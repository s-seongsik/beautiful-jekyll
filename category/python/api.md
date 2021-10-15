---
layout: post
title: API란 무엇이며, 좋은 API를 설계하기 위한 방법이 무엇일까?
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---

회사에서 naver cloud server와 Docker로 서비스 환경을 구축하고, 구축된 환경에 REST API를 개발 및 배포하는 작업을 맡게되었다.

개발하기 앞서, 다음과 같은 질문을 던져보았다.
**1. REST란 무엇인가?**
**2. REST API란 무엇이며**, 
**3. REST API 설계 방법** 

***1. REST란 무엇인가?***
> 'Representational State Transfer'의 약자로, 자원을 이름으로 구분하고 자원의 상태(**정보**)를 주고 받는 모든 것을 의미한다.
즉, 자원(resource)의 표현(representation) 에 의한 상태 전달(json, XML를 통해 데이터를 주고받는 것이 일반적)이다.

정의대로 이해하려고하면 무슨말인지 이해가 어려울 수 있으니 더 쉽게 풀어보자면

HTTP URI의 이름을 정하는것을 **자원(resource)**이라고 하고 HTTP Method(POST, GET, PUT, DELETE) 방식으로 CRUD 작업을 수행하는 것이다.

1. (POST) localhost:8080/user --> user 정보를 등록 
2. (GET) localhost:8080/user --> user 정보 조회
3. (PUT) localhost:8080/user --> user 정보 수정
4. (DELTE) localhost:8080/user --> user 정보 삭제

=> "/user" 라는 **자원(resource)**을 Client가  POST(등록), GET(조회), PUT(수정), DELETE(삭제) 행위에 따라 요청하게 되면
server는 이제 적절한 정보를 json, xml 등의 형태로 응답해주는 것을 REST이다.


***2. REST API란 무엇인가?***
- API(Application Programming Interface)는 컴퓨터 프로그램간 상호작용을 촉진하며, 서로 정보를 교환하는 것
- REST API란 위에 REST기반의 서비스를 API로 구현한 것을 말한다.
- 간단히 말해 REST형식으로 서비스를 구현하고, Client(app)에서 필요한 정보를 요청하면 알맞은 정보를 json 등의 형태로 정보를 리턴해주는 것을 말한다.
- 카카오맵, 구글맵, 공공데이터, 등 OpenApi를 제공하는 업체들은 대부분 REST API로 제공한다.

***3. REST API 설계 방법***

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |


How about a yummy crepe?

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg)

It can also be centered!

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg){: .mx-auto.d-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
