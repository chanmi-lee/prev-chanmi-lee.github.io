---
layout: post
title:  "Jekyll on Windows"
date:   2018-08-07
excerpt: "How to run Jekyll on Windows"
image: "https://chanmi-lee.github.io/images/jekyll.jpg"
categories: "Jekyll"
tag:
- Jekyll
- Markup Language
- Ruby
- Windows
- Configuration
---

Jekyll은 Unix, Linux, Mac (OS X)를 지원합니다.
윈도우에서 Jekyll을 사용하기 위해서는 별도로 설치가 필요합니다.

### Pre-requirements

* Ruby + Ruby DevKit

---

### Jekyll 설치하기

* Step 1
  - [Ruby Installer](https://rubyinstaller.org/)를 설치합니다.
  - 권장: Ruby+DevKit version - Jekyll은 Ruby 기반이므로 함께 설치합니다.

<img src="{{ site.url }}/images/jekyll-on-windows-install-ruby.png">
Add Ruby executables to your PATH 선택 시 Step 2 생략

<img src="{{ site.url }}/images/jekyll-on-windows-run-ruby-installer.png">
> Ruby installer 실행 결과

* Step 2
  - 설치 후, 시작 메뉴에서 Command 창을 열고, 환경변수 **PATH** 를 설정해줍니다.
  - ex) C:\dev\Ruby

**주의** 경로에 한글이 포함되지 않도록 확인합니다.

* Step 3
  - 위에서 설치한 Ruby devkit이 있는 폴더로 이동합니다.
  - **> gem install jekyll** 명령으로 Jekyll을 설치합니다.

<img src="{{ site.url }}/images/jekyll-on-windows-install-jekyll.png">
> ERROR:  Could not find a valid gem 'jekyll' (>= 0) in any repository

[**Solutions**]
1. **> gem sources** 명령으로 Current sources에 'https://rubygems.org/'가 있는지 확인합니다. 
없다면, **> gem sources add https://rubygems.org/** 명령으로 추가해줍니다.

2. 회사 방화벽이나 Proxy 환경 내에서 설치하는 경우, 
**> gem install -p http://proxy.server.ip:8080 GEMNAME** 으로 우회하여 설치할 수 있습니다.

3. **.gemrc** 파일 내에서 관련 환경 변수들을 직접 추가/수정 하는 방법도 있습니다.

<img src="{{ site.url }}/images/jekyll-on-windows-gem-configurtion.png">

[gem command docs](https://guides.rubygems.org/command-reference/)를 참고하여 진행해주세요 :)

  - **> jekyll -v** 명령으로 Jekyll이 올바르게 설치되었는지 확인합니다.
<img src="{{ site.url }}/images/jekyll-on-windows-verify-jekyll.png">

* Step 4
  - 설치 후, **> jekyll new .** 을 실행해보면 정상적으로 동작하지 않는데, 이는 의존성을 갖는 패키지들의 설치가 필요하기 때문입니다. 
  관련된 패키지를 모두 설치해줍니다.
