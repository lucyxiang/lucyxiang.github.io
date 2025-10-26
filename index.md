---
layout: default
title: Home
---

<div class="hero-container">
  <img id="cow-image" src="" alt="Cow" class="hero-image">
  <p class="hero-subtitle">Excited to meet moo</p>
</div>

<script>
  const cowImages = [
    '{{ "/assets/cow_1.jpg" | relative_url }}',
    '{{ "/assets/cow_2.jpg" | relative_url }}',
    '{{ "/assets/cow_3.jpg" | relative_url }}',
    '{{ "/assets/cow_4.jpg" | relative_url }}',
    '{{ "/assets/cow_5.jpg" | relative_url }}',
    '{{ "/assets/cow_6.jpg" | relative_url }}'
  ];

  const randomImage = cowImages[Math.floor(Math.random() * cowImages.length)];
  document.getElementById('cow-image').src = randomImage;
</script>
