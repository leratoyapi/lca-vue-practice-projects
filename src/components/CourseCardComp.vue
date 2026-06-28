<template>
  <div class="course-card">
    <div class="card-one">
      <img :src="amuseBoucheImg" alt="Amuse Bouche" />
      <h2 class="course-title">Amuse Bouche</h2>
      <p class="chef-name">Chef Masinda</p>
      <p class="price">R 200</p>
      <p class="skill-level">Intermediate</p>
      <p class="description">Smoked black marlin, tamarind & lemongrass dressing served with reserve Cap Classique Blanc de Blancs.</p>
      <button class="buy-now">Buy Now</button>
    </div>

    <div class="card-two">
      <img :src="painArtisanalImg" alt="Pain Artisanal" />
      <h2 class="course-title">Pain Artisanal</h2>
      <p class="chef-name">Chef Kunene</p>
      <p class="price">R 190</p>
      <p class="skill-level">Beginner</p>
      <p class="description">Warm brioche with house-made compound butters.</p>
      <button class="sold-out">Sold Out</button>
    </div>

    <div class="card-three">
      <img :src="dessertImg" alt="Dessert" />
      <h2 class="course-title">Dessert</h2>
      <p class="chef-name">Chef Fani</p>
      <p class="price">R 250</p>
      <p class="skill-level">Advanced</p>
      <p class="description">Grand Marnier soufflé with vanilla ice cream.</p>
      <button class="sold-out">Sold Out</button>
    </div>
  </div>
</template>

<script setup>
import amuseBoucheImg from '@/assets/course-images/amuse-bouche.jpg'
import painArtisanalImg from '@/assets/course-images/pain-artisanal.jpg'
import dessertImg from '@/assets/course-images/dessert.jpg'
</script>

<style scoped>
.course-card {
  display: grid;
  gap: 1.2rem;
}
.card-one,
.card-two,
.card-three {
  border: 1px solid #ddd;
  padding: 1rem;
  border-radius: 0.75rem;
  background: #fff;
}
.course-title {
  margin: 0.75rem 0 0.25rem;
}
.chef-name,
.price,
.skill-level,
.description {
  margin: 0.35rem 0;
}
img {
  width: 100%;
  display: block;
  border-radius: 0.75rem;
  object-fit: cover;
}
button {
  margin-top: 0.75rem;
  padding: 0.75rem 1rem;
  border: none;
  border-radius: 0.5rem;
  cursor: pointer;
  font-weight: 600;
}
.buy-now {
  background-color: #2563eb;
  color: #fff;
}
.sold-out {
  background-color: #6b7280;
  color: #fff;
}
</style>
