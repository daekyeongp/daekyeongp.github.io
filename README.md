<div align="center">

  # Chirpy Jekyll Theme

  A minimal, responsive, and powerful Jekyll theme for presenting professional writing.

  [![Gem Version](https://img.shields.io/gem/v/jekyll-theme-chirpy?color=brightgreen)](https://rubygems.org/gems/jekyll-theme-chirpy)
  [![Build Status](https://github.com/cotes2020/jekyll-theme-chirpy/workflows/build/badge.svg?branch=master&event=push)](https://github.com/cotes2020/jekyll-theme-chirpy/actions?query=branch%3Amaster+event%3Apush)
  [![Codacy Badge](https://app.codacy.com/project/badge/Grade/4e556876a3c54d5e8f2d2857c4f43894)](https://www.codacy.com/gh/cotes2020/jekyll-theme-chirpy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cotes2020/jekyll-theme-chirpy&amp;utm_campaign=Badge_Grade)
  [![GitHub license](https://img.shields.io/github/license/cotes2020/jekyll-theme-chirpy.svg)](https://github.com/cotes2020/jekyll-theme-chirpy/blob/master/LICENSE)
  [![996.icu](https://img.shields.io/badge/link-996.icu-%23FF4D5B.svg)](https://996.icu)

  [**Live Demo →**](https://cotes2020.github.io/chirpy-demo)

  [![Devices Mockup](https://raw.githubusercontent.com/cotes2020/chirpy-images/main/commons/devices-mockup.png)](https://cotes2020.github.io/chirpy-demo)

</div>

## Features

- Localized Layout
- Dark/Light Theme Mode
- Pinned Posts
- Hierarchical Categories
- Last Modified Date for Posts
- Table of Contents
- Auto-generated Related Posts
- Syntax Highlighting
- Mathematical Expressions
- Mermaid Diagram & Flowchart
- Disqus/Utterances/Giscus Comments
- Search
- Atom Feeds
- Google Analytics
- GA Pageviews Reporting
- SEO & Performance Optimization


## Quick Start

Before starting, please follow the instructions in the [Jekyll Docs](https://jekyllrb.com/docs/installation/) to complete the installation of `Ruby`, `RubyGems`, `Jekyll`, and `Bundler`. In addition, [Git](https://git-scm.com/) is also required to be installed.

### Step 1. Creating a New Site

Create a new repository from the [**Chirpy Starter**](https://github.com/cotes2020/chirpy-starter/generate) and name it `<GH_USERNAME>.github.io`, where `GH_USERNAME` represents your GitHub username.

### Step 2. Installing Dependencies

Before running for the first time, go to the root directory of your site, and install dependencies as follows:

```console
$ bundle
```

### Step 3. Running Local Server

Run the following command in the root directory of the site:

```console
$ bundle exec jekyll s
```

Or run with Docker:

```console
$ docker run -it --rm \
    --volume="$PWD:/srv/jekyll" \
    -p 4000:4000 jekyll/jekyll \
    jekyll serve
```

After a while, navigate to the site at <http://localhost:4000>.

## Documentation

For more details on usage, please refer to the tutorial on the [demo website](https://cotes2020.github.io/chirpy-demo/) / [wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki). Note that the tutorial is based on the [latest tag](https://github.com/cotes2020/jekyll-theme-chirpy/tags), and the features of the default branch are usually ahead of the documentation.

## Contributing

Welcome to report bugs, improve code quality or submit a new feature. For more information, see [contributing guidelines](.github/CONTRIBUTING.md).

## Credits

This theme is mainly built with [Jekyll](https://jekyllrb.com/) ecosystem, [Bootstrap](https://getbootstrap.com/), [Font Awesome](https://fontawesome.com/) and some other wonderful tools (their copyright information can be found in the relevant files). The avatar and favicon design come from [Clipart Max](https://www.clipartmax.com/middle/m2i8b1m2K9Z5m2K9_ant-clipart-childrens-ant-cute/).

:tada: Thanks to all the volunteers who contributed to this project, their GitHub IDs are on [this list](https://github.com/cotes2020/jekyll-theme-chirpy/graphs/contributors). Also, I won't forget those guys who submitted the issues or unmerged PR because they reported bugs, shared ideas, or inspired me to write more readable documentation.

Last but not least, thank [JetBrains][jb] for providing the OSS development license.

## Sponsoring

If you like this theme or find it helpful, please consider sponsoring me, because it will encourage and help me better maintain the project, I will be very grateful!

[![Ko-fi](https://img.shields.io/badge/-Buy%20Me%20a%20Coffee-ff5f5f?logo=ko-fi&logoColor=white)](https://ko-fi.com/coteschung)
[![Wechat Pay](https://img.shields.io/badge/-Tip%20Me%20on%20WeChat-brightgreen?logo=wechat&logoColor=white)][cn-donation]
[![Alipay](https://img.shields.io/badge/-Tip%20Me%20on%20Alipay-blue?logo=alipay&logoColor=white)][cn-donation]

## License

This work is published under [MIT](https://github.com/cotes2020/jekyll-theme-chirpy/blob/master/LICENSE) License.

<!-- ReadMe links -->

[jb]: https://www.jetbrains.com/?from=jekyll-theme-chirpy
[cn-donation]: https://cotes.gitee.io/alipay-wechat-donation/

_config.yml : 블로그의 기본 설정 파일입니다. 기본 환경세팅은 모두 여기에서 합니다.
_data : 왼쪽 사이드바와 포스트 하단의 공유하기 버튼등의 구성을 변경할 수 있습니다. 언어 설정에 따라 기본적으로 화면에 나오는 단어들을 변경할 수 있습니다.
_include : 사이드바, toc, 구글애널리틱스, footer, 댓글 등의 대부분의 모듈형으로 삽입되는 UI를 변경할 수 있습니다
_layout : 블로그 전역에 적용되는 기본 형식, 카테고리, 포스트 등에 적용되는 형식등을 변경할 수 있습니다.
_posts : 내가 작성한 블로그 글을 저장해 두는 곳입니다.
_sass : css 파일을 커스터마이징 할 수 있습니다.
_site : 로컬에서 실행할 때, 화면 UI를 구성하는 모든 내용이 들어 있습니다. 이곳의 내용을 변경하면 로컬에는 잘 반영되지만, git에는 올라가지 않습니다. 또한 다른 기본 디렉토리의 내용을 변경하고 빌드하게 되면 이곳의 내용이 바뀌게 됩니다.
_tabs : 왼쪽 사이드바의 기본 탭메뉴들에 대한 랜딩페이지가 들어 있습니다.
assets : css, img등이 있습니다. 포스팅에 들어갈 이미지는 assets/img 아래에 넣으면 됩니다.
tools : github에서 자동 배포를 위한 코드가 들어 있습니다. 이곳은 아예 건들지 맙시다