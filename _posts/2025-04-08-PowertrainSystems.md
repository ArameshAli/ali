---
layout: post
title: Powertrain & NVH Benchmarking in Battery Electric Vehicles
feature-img: "assets/img/powertrain.jpg"
thumbnail: "assets/img/powertrain.jpg"
tags: [Automotive, Powertrain]
categories: Automotive
---

Battery Electric Vehicles (BEVs) present a unique set of challenges and opportunities when it comes to **powertrain design** and **NVH (Noise, Vibration, and Harshness) performance**. During my time at **Toyota**, I worked on NVH benchmarking and powertrain system analysis across different BEV platforms.

---

## ⚙️ Powertrain Architecture Analysis

- Extraction of **RPM**, **torque**, and **PMSM motor behavior** in multiple BEV variants.
- Used **CATIA V5** and **BMS data** to analyze powertrain component contribution to overall system performance.
- Supported motor control refinement to improve efficiency and reduce drivetrain ripple.

---

## 🎧 NVH Benchmarking on BEVs

While BEVs eliminate combustion noise, they also expose subtle mechanical or gear-related noises.

- Conducted **Transfer Path Analysis (TPA)** to map sound transmission from motor to cabin.
- Used **Body Acoustic Sensitivity Mapping** to localize unwanted hums and rattles.
- Compared NVH signatures across **competitive models** (e.g., Nissan Leaf, VW ID.3).

---

## 🛠 Tools & Methods Used

- **CATIA V5** for design data
- **TPA software tools**
- **AutoCAD** for layout interpretation
- **BMS data analysis**
- Structured under **V-cycle methodology**

---

## ✅ Results

- Helped prioritize redesign of motor mounts and damping elements.
- Enabled data-driven selection of quieter drive units for the next-gen platform.
- Contributed to overall **acoustic comfort benchmarking** for Toyota’s future BEV lineup.

---

🔍 Interested in the technical details or analysis visuals? Check out my [Portfolio](/portfolio) or [About Me](/about).





Hopefully you will find enough information about how to set images in your blog here.
This is an example of a post which includes a feature image specified in the front matter of the post. 
The feature image spans the full-width of the page, and is shown with the title on permalink pages:

```yaml
feature-img: "assets/img/feature-img/desk-messy.jpeg"
thumbnail: "assets/img/thumbnails/feature-img/desk-messy.jpeg" 
```

You can also use a thumbnail, a smaller version of the same image to improve loading of the page.
The thumbnail will also be used when you share your article on other platform (linkedin, whatsapp, facebook, ...).

>  - And now it is working

You can also add images aligned in your post using the `aligner` include.
Make sure to separate all of the image path from in a string separated with `,`.
It by default look into `assets/img/` so give the path from there, example:

{% highlight ruby %}
{% raw %}
{% include aligner.html images="pexels/book-glass.jpeg,triangle.png" caption="A caption under the images" %}
{% endraw %}
{% endhighlight %}

{% include aligner.html images="pexels/book-glass.jpeg,feature-img/desk-messy.jpeg" caption="A caption under the images" %}


Here you have two images side by side, but you can set more and set the amount per columns 
(by specifying the number of columns or let it be automatic using `"auto"`):

{% highlight ruby %}
{% raw %}
{% include aligner.html images="portfolio/cabin.png,portfolio/cake.png,portfolio/circus.png" column=3 %}
{% endraw %}
{% endhighlight %}

{% include aligner.html images="portfolio/cabin.png,portfolio/cake.png,portfolio/circus.png" column=3 %}

it also works with only one images, it is made to display it smaller than normally.
However you can just use the Markdown way of doing it to get the image normal sized and centered.

{% highlight ruby %}
{% raw %}
# Markdown way
![Travel]({{ "/assets/img/pexels/computer.jpeg" | relative_url}})
# Aligner with only one image
{% include aligner.html images="pexels/computer.jpeg" %}
{% endraw %}
{% endhighlight %}

{% include aligner.html images="pexels/computer.jpeg" %}
