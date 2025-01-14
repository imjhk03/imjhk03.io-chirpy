---
title: iOS 15에서 UIButton의 title이 Button으로 나타나는 현상 해결 방법
layout: post
categories: [Problem Solving]
tags: [uikit]
---

Xib로 `UIButton`을 만들면 보통 `Type`을 `Custom`으로 해서 만드는 경우가 있다. 이미지를 넣어서 이미지만 있는 버튼을 그릴 때는 Title 값을 빈 문자열로 둔다. 하지만 어떻게 설정하냐에 따라서 iOS 15에서는 Title 값에 Button이 나타나는 경우가 있다.

<img src="/assets/img/2022/07/26/image1.PNG" alt="A Button with image is showing title label saying Button" width="400"/>


이때는 `Style` 값을 `Default` 값으로 바꾼 뒤, Title 값을 지우면 해결이 된다.

<img src="/assets/img/2022/07/26/image2.png" alt="A Button with image without showing title label" width="400"/>

Xib 파일을 코드 상으로 확인했을 때, ```title="Button"```으로 되어 있는 게 없는지 체크하는 방법도 있다.

<img src="/assets/img/2022/07/26/image3.png" alt="Code difference image from xib file"/>