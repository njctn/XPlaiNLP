---
title: "Splash Page"
layout: splash
permalink: /splash-page/
date: 2016-03-23T11:48:41-04:00
feature_row:
  - image_path: /assets/images/bio-photo.jpg
    alt: "placeholder image 1"
    title: "Placeholder 1"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    size: "300"
  - image_path: /assets/images/bio-photo.jpg
    title: "Placeholder 3"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    size: "300"
  - image_path: /assets/images/bio-photo.jpg
    title: "Placeholder 3"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    size: "300"
feature_row2:
  - image_path: /assets/images/bio-photo.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`, trying to resize imge with `size: "width: 250px"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
    size: "500"
feature_row3:
  - image_path: /assets/images/bio-photo.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`, test this: `{: .align-center style="width: 25%;"}`'
    url: "#test-link"
feature_row4:
  - image_path: /assets/images/bio-photo.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`, test this: `{: .align-center style="width: 50%;"}`'
    url: "#test-link"
  - image_path: /assets/images/test.jpg
    alt: "test image"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`, test this: `{: feature_row4.align-center style="width: 50%;"}`'
    url: "#test-link"
---
<!---
feature rows built with liquid
https://www.fabriziomusacchio.com/blog/2021-08-12-Liquid_Cheat_Sheet/#the-liquid-template-language-and-its-main-components
-->

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

<!---
CSS added to the whole feature row with kramdown
https://www.fabriziomusacchio.com/blog/2021-08-11-Minimal_Mistakes_Cheat_Sheet/#kramdown
-->
{% include feature_row id="feature_row3" type="right" %}{: .align-center style="width: 25%;"}

{% include feature_row id="feature_row4" type="center" %}{: feature_row4.align-center style="width: 50%;"}

# image with base html
<img src="/assets/images/test.jpg" alt="test" width="200"/>

<figure style="width: 80px" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <figcaption>Image caption.</figcaption>
</figure>

### html only

<figure class="third">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <!--<figcaption>Charlott Jakob</figcaption> -->
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <!--<figcaption>Salar Mohtaj</figcaption> -->
    <figcaption>Ibrahim Baroud Charlott Jakob Salar Mohtaj</figcaption>
</figure>

<figure style="width: 250px" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <figcaption>Premtim Sahitaj</figcaption>
</figure>

<figure style="width: 250px" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <figcaption>Vera Schmitt</figcaption>
</figure>

# Student Assistants

<figure class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="" width="250">
  <figcaption>Ata Nizamoglu</figcaption>
</figure>

<figure style="width: 250px" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <figcaption>Ariana Sahitaj</figcaption>
</figure>

# Alumni

<figure style="width: 250px" class="align-center">
  <img src="{{ site.url }}{{ site.baseurl }}/assets/images/bio-photo.jpg" alt="">
  <figcaption>Martin Burghart</figcaption>
</figure>

