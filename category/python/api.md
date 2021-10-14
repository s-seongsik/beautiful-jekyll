---
layout: category
title: API란 무엇이며, 좋은 API를 설계하기 위한 방법이 무엇일까?
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---

회사에서 naver cloud server와 Docker를 활용하여 환경을 구축하고, 구축된 환경에 REST API를 개발 및 배포하는 작업을 맡게되었다.

일단 API를 개발하기 앞서, **1. REST API란 무엇이며**, **2. 좋은 REST API를 개발하기 위해서 어떻게 설계하는 것이 옳바른가?** 의 질문을 던져보았다.

그냥 API는 어플리케이션끼리 데이터를 주고받는 인터페이스 아니야? 라는 거시적인 관점으로만 답변 할 수 있었다.

정확한 정의를 꼭 알아야 하나? 라고 물을 수 있지만, 나에게 what(그게 뭔데?), why(그걸 왜 사용하는데?), when(그걸 언제 사용하는데?), how(그걸 어떻게 사용하는데?) 4원칙은 성장에 중요한 요소라고 생각하기 때문에 짚고 넘어가려고 한다.

일단 API란

(여기부터 이어나가면 됨.)

## Here is a secondary heading

Here's a useless table:

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
