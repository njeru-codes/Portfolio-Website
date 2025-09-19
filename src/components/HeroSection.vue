<template>
  <div class="hero-section">
    <div class="container">
      <div class="hero-content">
        <div class="text-content">
          <h1 class="hero-heading">I'M NJERU  MTWAITI</h1>
          <h2 class="hero-subheading">DELIVERING WORLD-CLASS CYBERSECURITY SOLUTIONS</h2>
          <p class="hero-description">
            As one of the leading experts in cybersecurity, I specialize in safeguarding your digital world 
            with unmatched precision and expertise. From comprehensive IT support to advanced security strategies,
             I provide a one-stop solution tailored to your needs. 
            A true one-man powerhouse, I ensure your security is never compromised.
          </p>
          <div class="button-group">
            <button class="primary-button">Learn More</button>
            <button class="secondary-button">Get in Touch</button>
          </div>
        </div>
        <div class="image-content">
          <img :src="HeroImg" alt="A professional man looking forward" class="hero-image">
        </div>
      </div>
    </div>
  </div>
</template>


<script setup>
import HeroImg from "@/assets/Group2.png"
</script>

<style scoped>


.hero-section {
  background-color: #000;
  height: 100vh;
  width: 100%;
  padding: 4rem 0;
  position: relative;
  overflow: hidden;
  /* Use a more flexible height on mobile */
  min-height: 100vh;
  display: flex;
  align-items: center;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
}

.hero-content {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 4rem;
  padding-top: 1rem;
  margin: auto;
}

.text-content {
  flex: 1.25;
}

.hero-heading {
  font-size: 1.2rem;
  font-weight: 600;
  color: #a0a0a0;
  letter-spacing: 2px;
  margin-bottom: 0.5rem;
}

.hero-subheading {
  font-size: 3.7rem;
  font-weight: 700;
  line-height: 1.2;
  margin: 0;
  color: #ffffff;
}

.hero-subheading span {
  color: #00ff7f;
}

.hero-description {
  color: #fff;
  line-height: 1.6;
  max-width: 600px;
  margin-top: 1.5rem;
  font-size: 1.2rem;
}

.button-group {
  display: flex;
  gap: 1rem;
  margin-top: 2rem;
}

.primary-button, .secondary-button {
  padding: 1rem 2.5rem;
  border-radius: 5px;
  font-weight: bold;
  cursor: pointer;
  transition: background-color 0.3s, color 0.3s;
  border: none;
}

.primary-button {
  background-color: #00ff7f;
  color: #121212;
}

.primary-button:hover {
  background-color: #00e66a;
}

.secondary-button {
  background-color: transparent;
  color: #ffffff;
  border: 1px solid #00ff7f;
}

.secondary-button:hover {
  background-color: #00ff7f;
  color: #121212;
}

.image-content {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center; /* Center the image vertically within its container */
}

.hero-image {
  max-width: 100%;
  height: auto;
  border-radius: 10px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
}

@media (max-width: 768px) {
  .hero-section {
    height: auto;
    padding: 2rem 0; /* Add more vertical padding for mobile */
  }

  .hero-content {
    flex-direction: column;
    padding-top: 0;
    padding-bottom: 0;
    gap: 2rem; /* Reduce the gap on mobile */
  }

  .text-content, .image-content {
    text-align: center;
    width: 100%; /* Ensure they take up the full width */
    padding: 0 0rem; 
  }

  .text-content {
    order: 1; /* Pushes the text content below the image */
  }

  .image-content {
    order: 2; /* Pushes the image to the top */
    padding-top: 2rem; /* Add space at the top */
  }

  .hero-heading {
    font-size: 1rem;
  }

  .hero-subheading {
    font-size: 2rem; /* A slightly smaller, more readable size */
  }

  .hero-description {
    max-width: 100%;
    font-size: 1rem;
    padding: 0 0.5rem; /* Add a little more padding */
  }

  .button-group {
    flex-direction: column; /* Stack buttons vertically */
    gap: 0.5rem; /* Reduce gap between buttons */
    align-items: center; /* Center the buttons */
  }

  .primary-button, .secondary-button {
    width: 80%; /* Make buttons full-width */
    padding: 0.75rem 1rem; /* Adjust padding for better sizing */
  }

  .hero-image {
    max-width: 80%; /* A better size for mobile screens */
    height: auto;
    margin-top: 0;
  }
}
</style>