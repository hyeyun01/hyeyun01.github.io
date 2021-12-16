---
layout: post
title: Project Build Process(2) Use Ruby
date: 2021-12-15 15:18 +0800
last_modified_at: 2020-12-15 18:08:25 +0800
Catrgories: [Git-Blog]
tags: [tutorial]
toc:  true
---
**2021-2학기 유레카프로젝트**
{: .message }


>Git Blog Project Build Process(2) - Use Ruby


다음으로는 Ruby와 Ruby on Rails를 설치했던 과정과, Ruby를 이용해 local host에 접근하는 방법으로 git blog의 변경상황을 딜레이 없이 빠르게 확인해보도록 하겠다.




## Ruby 설치

Ruby 공식 홈페이지에서 최신 버전의 Ruby를 다운 받으면 된다.


## Ruby on rails 설치

cmd 창에서

{% highlight js %}
$ gem install rails
$ rails -v
{% endhighlight %}


를 입력해 rails를 설치하고, 버전이 잘 뜨는지 확인해준다.

<img width="169" alt="KakaoTalk_20211216_161841128" src="https://user-images.githubusercontent.com/77826769/146325591-2f69cd59-8178-44c2-b0ad-e46fbd868b09.png">

잘 뜬다.


## bundle exec jakyll serve

<img width="447" alt="KakaoTalk_20211216_162528359" src="https://user-images.githubusercontent.com/77826769/146326628-2b1ee386-d3de-41f1-a7c8-13d510320f42.png">


이렇게 뜨는데 도저히 뭘 설치하고 업데이트해도 해결이 안된다...
