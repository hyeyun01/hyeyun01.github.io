---
layout: post
title: Project Build Process(1)-Make Git Blog
date: 2021-12-12 15:18 +0800
last_modified_at: 2020-12-15 18:08:25 +0800
tags: [tutorial]
toc:  true
---
**2021-2학기 유레카프로젝트**
{: .message }
>Git Blog Project Build Process(1) - Make Git Blog.

처음으로 Git Blog를 만들어보았다.
이전까지 [Tistory](https://yuni01.tistory.com/)를 사용하며 Git Blog를 만들고 싶다고만 생각하다가 수업이라는 기회를 통해 블로그를 만들었고, 블로그 만드는 과정과 테마 적용, 글을 올리는 과정을 포스팅 하려고 한다.


## Make Git Blog Link !

우선 본인의 git 계정이 필요하다.

<img width="703" alt="KakaoTalk_20211215_191609143" src="https://user-images.githubusercontent.com/77826769/146168232-56b9f92b-7d01-40da-a3ce-12fffaf0399d.png">{: .align-center}

[username].github.io 라는 이름으로 repository를 하나 만들어준다.

Clone에서 https 링크를 복사한다.

Git Bash에서 다음 코드를 수행한다.
(오류 발생시 cd 명령어를 이용해 directory를 적절히 조정해준다 / cd .. : 상위 디렉토리로 이동)


{% highlight js %}
$ cd [directory(레포지토리 저장할 위치)]
$ git clone [복사한 링크 (마우스를 이용해 붙여넣기, ctrl+v 사용 X)]
{% endhighlight %}


## Apply the Theme

Jekyll에서 원하는 테마를 가져와서 수정하는 방법을 선택했다.
[http://jekyllthemes.org/](http://jekyllthemes.org/)에서 마음에 드는 테마의 소스코드 파일을 다운로드 한다.

레포지토리 폴더 내에 압축을 풀어 파일을 넣어준다.

{% highlight js %}
$ cd [directory (똑같이 따라왔다면 [username].github.io 폴더 일 것임)]
$ git add .
$ git commit -m '(ex)new theme(원하는 메세지를 입력하면 된다)'
$ git push origin master
{% endhighlight %}

Git Bash에서 해당 코드를 입력해주면
Github에 파일이 연동되도록 commit 해준 것이다.


## Edit the Code

제일 먼저 해줬던 일은 '_config.yml' 수정하기 이다.


![image]("https://user-images.githubusercontent.com/77826769/146174626-35cebdeb-ac7f-4496-9cfd-657aa927e349.png")

여기서 블로그 이름, 소개, 아이콘 사진 및 배경 사진을 _config.yml 파일에서 수정했다.

visual code를 이용해 한 파일씩 열어보면서 코드가 어떤 의미인지 파악하고 디렉토리에 사진을 배치하고 불러오는 식으로 하면 된다.

그 방법으로 아이콘을 수정하고, 내 이메일과 SNS 링크도 업로드할 수 있었다.
