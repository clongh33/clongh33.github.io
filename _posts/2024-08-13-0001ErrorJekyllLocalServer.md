---
layout: single
title: "Error: 'bundle exec jekyll serve' is not working. [EN/KR]"
categories: troubleshooting
tag: [troubleshooting, blog, jekyll, github pages]
author_profile: true
use_math: true
---

I'm making Github page with Minimal mistake theme. 
But I had a trouble to operate local jekyll server and error message is down below. 

Minimal mistake 테마를 fork 해와서 깃허브 페이지로 블로그를 만드는 과정에서,
지킬 서버가 제대로 동작하지 않는 이슈가 있었습니다.

![jeykllErrorMsg]({{site.url}}/assets/images/0001/bundle exec jekyll serve Error.png){: .align-center}

So I research solution in the google and got this solution. 
Let's follow and try this methode. 

구글링을 통해서 몇가지 해결책을 찾을 수 있었고, 여러번의 시도 끝에 효과가 있었던 방법을 공유하겠습니다. 

![modifyingGemfile]({{site.url}}/assets/images/0001/Step01GemfileModifing.png){: .align-center}

First, we should modified Gemfile like this screen shot first. 
And let's install tzinfo and tzinfo-data.

일단, tzinfo 관련 에러가 올라오시는분은 tzinfo 와 tzinfo-data 를 위에 스크린샷을 따라서 설치해주세요.

```
gem install tzinfo
gem install tzinfo-data
```

After you install all the things. 
Let's do 'bundle' at the cmd Panel.

다 설치하셨으면 cmd 창에서 bundle 입력하여 번들 설치해주세요.

![cmdBundle]({{site.url}}/assets/images/0001/Step02.png){: .align-center}

After you finish bundle, let's try to operate local server once again.

설치가 끝났으면 다시 서버를 재실행 시켜주세요. 

![execServer]({{site.url}}/assets/images/0001/Step03.png){: .align-center}

![serverOperating]({{site.url}}/assets/images/0001/Step04.png){: .align-center}

Jekyll local server operate successfully!

지킬 서버가 정상적으로 재실행 되었습니다. 

If you find better solution, please let me know by comment. 
Thank you for reading.

더 좋은 해결책 혹은 다른 해결책을 아신다면 댓글로 알려주세요.
읽어주셔서 감사합니다.