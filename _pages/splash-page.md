---
title: "Splash Page"
layout: splash
permalink: /splash-page/
date: 2016-03-23T11:48:41-04:00
feature_row:
  - image_path: assets/images/bio-photo.jpg
    alt: "placeholder image 1"
    title: "Placeholder 1"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder 2"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/bio-photo.jpg
    title: "Placeholder 3"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
feature_row2:
  - image_path: /assets/images/bio-photo.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
    img_url: '450x' 
feature_row3:
  - image_path: /assets/images/bio-photo.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`, test this: `{: .align-center style="width: 25%;"}`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/images/bio-photo.jpg{: .align-center style="width: 50%;"}
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`, test this: `{: .align-center style="width: 50%;"}`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/test.jpg
    alt: "test image"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`, test this: `{: .align-center style="width: 50%;"}`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---
<!---
feature rows built with liquid
https://www.fabriziomusacchio.com/blog/2021-08-12-Liquid_Cheat_Sheet/#the-liquid-template-language-and-its-main-components
-->
{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

<!---
CSS added to the whole feature row with kramdown
https://www.fabriziomusacchio.com/blog/2021-08-11-Minimal_Mistakes_Cheat_Sheet/#kramdown
-->
{% include feature_row id="feature_row3" type="right" %}{: .align-center style="width: 25%;"}

{% include feature_row id="feature_row4" type="center" %}{: .align-center style="width: 50%;"}

# image with base html
<img src="/assets/images/test.png" alt="test" width="200"/>

<figure style="width: 80px" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <figcaption>Image caption.</figcaption>
</figure>

