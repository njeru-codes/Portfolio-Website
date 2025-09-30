<template>
  <div class="hero-section">
    <div class="container">
      
      <!-- header -->
      <div class="header">
        <div class="header-controls">
          <div class="dot red"></div>
          <div class="dot yellow"></div>
          <div class="dot green"></div>
          <p class="path">
            <span>root@access: </span>$ cat welcome.txt</p>
        </div>
      </div>
      <!-- header -->


      <div class="content">
        <div class="left-content">
          <img :src="HeroImg" alt="Hero Image" class="hero-image" />
        </div>

      <div class="text-content">
          <p class="hero-tagline">
            <span class="fold">[</span>    
            unlocking the undetectable. <span class="cursor">_ </span>
            <span class="fold">]</span>
          </p>
          <h1 class="hero-title">
            NJERU MTWAITI
          </h1>
          <h2 class="hero-subtitle">
            Offensive Security Engineer
          </h2>
          <p class="hero-description">
            I specialize in penetration testing, red teaming operations, and deep-dive vulnerability research, focusing on both network infrastructure and proprietary software security.
          </p>

          

          <div class="hero-links">
            <span>> Exploits/</span>
            <span>> Research/</span>
            <span>> Tools/</span>
            <span>> Contact/</span>
          </div>

          <div class="hero-actions">
            <a href="#research" class="btn-primary">
              <span class="neon-glow">Execute: Portfolio</span>
            </a>
            <a href="" target="_blank" class="btn-secondary">
              <span>Connect: PGP Key</span>
            </a>
          </div>


      </div>
      </div>

      <div class="header end-header">
            <div class="header-controls">
              <h3 class="path">
                <span>root@access: </span>~$
              </h3>
            </div>
      </div>

    </div>
  </div>
</template>


<script setup>
import HeroImg from "@/assets/Group2.png"
</script>

<style scoped>
:root {
            --color-accent-green: #00FF41; /* Primary Hacking Color */
            --color-accent-blue: #00BFFF; /* Secondary Data Color (Deep Sky Blue) */
            --color-dark: #070710;
}

.hero-section {
  background-color: #000;
  height: 100vh;
  width: 100%;
  padding: 2rem 0;
  position: relative;
  overflow: hidden;
  min-height: 100vh;
  display: flex;
  align-items: center;
}

.container {
  max-width: 1200px;
  width: 100%;
  height: fit-content;
  min-height: 80vh;
  margin: 0 auto;
  padding: 0 2rem;
  display: flex;
  flex-direction: column;
  gap: 2rem;
}


/* header */
.header {
  padding-bottom: 1rem;
  margin-bottom: 1rem;
  background: #332b2bf3;
  border-bottom: 1px solid #374151; 
  border-top-left-radius: 8px;
  border-top-right-radius: 8px;
  padding: 0.5rem 1.5rem;
  display: flex;
  align-items: center;
}

.header-controls {
  display: flex;
  align-items: center;
  gap: 0.5rem; 
  margin-bottom: 0.75rem;
}

.dot {
  width: 0.75rem; 
  height: 0.75rem;
  border-radius: 50%;
}

.dot.red {
  background-color: #ef4444; 
}
.dot.yellow {
  background-color: #f59e0b; 
}
.dot.green {
  background-color: #22c55e; 
}

.path {
  margin-left: 0.5rem;
  font-size: 1rem; 
  color: #9ca3af; 
  display: none;
}
.path span {
  color: #00FF41;
  font-weight: bold;
}
@media (min-width: 640px) {
  .path {
    display: inline; 
  }
}
.header.end-header {
  background: none;
  border: none;
  margin: 2rem 0;
}
/* end header */




.content{
  display: flex;
  flex-direction: row;
  flex: 1;
  align-items: center;
  justify-content: center;
  width: 100%;
  gap: 2rem;
}
.left-content{
  display: flex;
  flex: 2;
  width: 100%;
  height: 100%;
  align-items: center;
  justify-content: center;
}
.hero-image{
  width: 100%;
  max-width: 350px;
  height: auto;
  border-radius: 50%;
  border: 3px solid #cac8c823;
  box-shadow: 0 0 20px rgba(0, 255, 133, 0.3);
}


/* text content */
.text-content{
  display: flex;
  flex: 3;
  flex-direction: column;
}
.hero-tagline {
  font-size: clamp(0.8rem, 2vw, 1rem);
  font-weight: 400;
  margin-bottom: 30px;
  opacity: 0.8;
}
.hero-tagline .fold {
  color: #00ff405d;
  font-weight: bolder;
}
.cursor {
  color: #00FF41;;
  animation: blink 1s step-start infinite;
  font-weight: bolder;
}
@keyframes blink {
  50% { opacity: 0; }
}
.hero-title {
  font-weight: 900;
  margin-bottom: 0.5rem;
  line-height: 1;
  font-size: 2.25rem;
  color: #ffffff;
}

@media (min-width: 640px) {
  .hero-title {
    font-size: 3.75rem; 
  }
}

@media (min-width: 1024px) {
  .hero-title {
    font-size: 4.5rem; 
  }
}
.hero-subtitle {
  font-weight: 700; 
  font-size: 2.25rem; 
  color: var(--neon-green, #39ff14); 
}

@media (min-width: 640px) {
  .hero-subtitle {
    font-size: 1.5rem; 
  }
}

@media (min-width: 1024px) {
  .hero-subtitle {
    font-size: 1.8rem; 
  }
}
.hero-description {
  font-family: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol",
    "Noto Color Emoji"; 
  font-size: 1.125rem;
  color: #d1d5db; 
  margin: 2rem 0; 
  max-width: 42rem; 
}
.hero-links {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr)); 
  gap: 1rem; 
  margin-bottom: 2.5rem; 
  font-size: 1.23rem;
  font-weight: 900;
  cursor: pointer;
}

.hero-links span {
  color: #4ade80; 
}

@media (min-width: 640px) {
  .hero-links {
    grid-template-columns: repeat(4, minmax(0, 1fr)); /* sm:grid-cols-4 */
  }
}
.hero-actions {
  display: flex;
  flex-direction: column; 
  gap: 1rem; 
}

@media (min-width: 640px) {
  .hero-actions {
    flex-direction: row; 
    gap: 0; 
  }

  .hero-actions a + a {
    margin-left: 1rem; 
  }
}

.hero-actions a {
  flex: 1; /* flex-1 */
  text-align: center;
  padding: 0.75rem 1rem; /* py-3 */
  border-radius: 0.375rem; /* rounded-md */
  font-size: 1.125rem; /* text-lg */
  font-weight: 700; /* font-bold */
  background: transparent;
  text-decoration: none;
  transition: all 0.3s ease;
}

/* Primary button */
.btn-primary {
  border: 2px solid var(--neon, #39ff14); 
  color: var(--neon, #39ff14);
}

/* Secondary button */
.btn-secondary {
  border: 2px solid #4b5563; 
  color: #9ca3af; 
}
.btn-secondary:hover {
  font-weight: bold;
  color: #ffffff; 
}


/* text content */

</style>