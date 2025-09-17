<template>
  <div class="about-wrapper">
    <div class="container">
      <div class="content-card">

        <div class="content">
          <!-- Left content -->
          <div class="left">
            <h2 class="subtitle">Why Work With Me?</h2>
            <h1 class="title">
              Cybersecurity Expertise <br /> You Can Trust
            </h1>
            <p class="description">
              I’m  a skilled and certified
              <strong>Security Analyst & Penetration Tester</strong> with hands-on
              experience in offensive security, bug bounty research, and vulnerability
              management. I help individuals and businesses strengthen their defenses
              against today’s advanced threats.
            </p>

            <div class="features-list">
              <div class="feature-item">
                <span class="feature-icon">
                  <svg class="icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M9 12l2 2 4-4m5.618-4.016A11.955 
                        11.955 0 0112 2.944a11.955 11.955 
                        0 01-8.618 3.04A12.015 12.015 0 
                        002.518 9a12.015 12.015 0 00-1.026 
                        3.016 12.008 12.008 0 00.56 
                        5.864A12.015 12.015 0 005.482 
                        21a12.015 12.015 0 005.023 2.062 
                        12.015 12.015 0 005.495-2.062 
                        12.015 12.015 0 003.964-3.416 
                        12.015 12.015 0 001.026-3.016A12.008 
                        12.008 0 0021.5 9a12.015 12.015 0 
                        00-1.026-3.04z"
                    />
                  </svg>
                </span>
                <div>
                  <h3 class="feature-title">Certified Professional</h3>
                  <p class="feature-description">
                    EC-Council & Cisco certified with proven expertise in penetration testing and
                    vulnerability assessments.
                  </p>
                </div>
              </div>

              <div class="feature-item">
                <span class="feature-icon">
                  <svg class="icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M9 12l2 2 4-4m5.618-4.016A11.955 
                        11.955 0 0112 2.944a11.955 11.955 
                        0 01-8.618 3.04A12.015 12.015 0 
                        002.518 9a12.015 12.015 0 00-1.026 
                        3.016 12.008 12.008 0 00.56 
                        5.864A12.015 12.015 0 005.482 
                        21a12.015 12.015 0 005.023 2.062 
                        12.015 12.015 0 005.495-2.062 
                        12.015 12.015 0 003.964-3.416 
                        12.015 12.015 0 001.026-3.016A12.008 
                        12.008 0 0021.5 9a12.015 12.015 0 
                        00-1.026-3.04z"
                    />
                  </svg>
                </span>
                <div>
                  <h3 class="feature-title">Freelance Security Partner</h3>
                  <p class="feature-description">
                    Available for penetration testing, bug bounty programs, and custom security
                    consulting.
                  </p>
                </div>
              </div>

              <div class="feature-item">
                <span class="feature-icon">
                  <svg class="icon" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      stroke-width="2"
                      d="M9 12l2 2 4-4m5.618-4.016A11.955 
                        11.955 0 0112 2.944a11.955 11.955 
                        0 01-8.618 3.04A12.015 12.015 0 
                        002.518 9a12.015 12.015 0 00-1.026 
                        3.016 12.008 12.008 0 00.56 
                        5.864A12.015 12.015 0 005.482 
                        21a12.015 12.015 0 005.023 2.062 
                        12.015 12.015 0 005.495-2.062 
                        12.015 12.015 0 003.964-3.416 
                        12.015 12.015 0 001.026-3.016A12.008 
                        12.008 0 0021.5 9a12.015 12.015 0 
                        00-1.026-3.04z"
                    />
                  </svg>
                </span>
                <div>
                  <h3 class="feature-title">Technical Skills</h3>
                  <p class="feature-description">
                    Proficient in Python, Go, vulnerability management, and backend API security
                    development.
                  </p>
                </div>
              </div>
            </div>
          </div>

          <!-- Right content -->
          <div class="right">
            <div class="shield-container">
              <img :src="AboutImg" alt="Cyber Security Shield" class="shield-image" />
              <div class="pulse-ring pulse-1"></div>
              <div class="pulse-ring pulse-2"></div>
              <div class="pulse-ring pulse-3"></div>
            </div>
            
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script setup>
import AboutImg from "@/assets/Group 1(1)-Photoroom.png"
</script>

<style scoped>
/* Main component container */
.about-wrapper {
    background-color: #0a1320;
    color: #e5e7eb; /* equivalent to text-gray-200 */
    /* padding: 80px 16px; */
    background: #000;

}

.container {
    width: 100%;
    height: 100%;
    max-width: 1280px;
    margin: 0 auto;
    padding-left: 1.5rem;
    padding-right: 1.5rem;
}

/* The main content card with the tilt effect */
.content-card {
    position: relative;
    background-color: #000;
    padding: 48px;
    /* transform: rotate(-2deg); */
    overflow: hidden;
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}

/* Inner content for z-index layering */
.content {
    position: relative;
    z-index: 10;
    display: flex;
    flex-direction: column;
    gap: 40px;
    align-items: center;
}

/* Left and Right sections */
.left,
.right {
    flex: 1;
    padding: 24px;
}

@media (min-width: 1024px) {
    .content {
        flex-direction: row;
        justify-content: space-between;
    }
    .left {
        text-align: left;
    }
    .description {
        margin: 0;
    }
}

/* Text styles */
.subtitle {
    font-size: 0.75rem;
    color: #00e396;
    font-weight: 600;
    letter-spacing: 0.05em;
    text-transform: uppercase;
}

.title {
    margin-top: 8px;
    font-size: 2.25rem;
    line-height: 1.1;
    font-weight: 800;
    color: white;
}
@media (min-width: 768px) {
    .title {
        font-size: 2.5rem;
    }
}

.description {
    margin-top: 16px;
    color: #9ca3af; /* equivalent to text-gray-400 */
    max-width: 560px;
    font-size: 0.875rem;
}
@media (min-width: 768px) {
    .description {
        font-size: 1rem;
    }
}

/* Features list */
.features-list {
    margin-top: 24px;
    display: flex;
    flex-direction: column;
    gap: 16px;
    text-align: left;
}

.feature-item {
    display: flex;
    align-items: flex-start;
}

.feature-icon {
    color: #00e396;
    flex-shrink: 0;
    margin-right: 12px;
}

.icon {
    height: 20px;
    width: 20px;
}

.feature-title {
    font-weight: 700;
    font-size: 1.125rem;
    color: white;
}

.feature-description {
    font-size: 0.875rem;
    color: #9ca3af;
}

/* Right side - Shield Image & Pulsing Rings */
.right {
    display: flex;
    justify-content: center;
    align-items: center;
}
@media (min-width: 1024px) {
    .right {
        justify-content: flex-end;
    }
}

.shield-container {
    position: relative;
    width: 100%;
    /* max-width: 448px; */
    aspect-ratio: 1 / 1;
    display: flex;
    justify-content: center;
    align-items: center;
    transform: rotate(-2deg);
}

.shield-image {
    width: 100%; /* equivalent to w-2/3 */
    height: auto;
    position: relative;
    z-index: 2;
}

.pulse-ring {
    position: absolute;
    border-radius: 50%;
    border: 1px solid #00e396;
    opacity: 0.3;
}

.pulse-1 {
    width: 100%;
    height: 100%;
    animation: pulse-animation 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}
.pulse-2 {
    width: 90%;
    height: 90%;
    animation: pulse-animation 4s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}
.pulse-3 {
    width: 80%;
    height: 80%;
    animation: pulse-animation 6s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}

/* Keyframes for the pulsing animation */
@keyframes pulse-animation {
    0%, 100% {
        transform: scale(1);
        opacity: 0.3;
    }
    50% {
        transform: scale(1.1);
        opacity: 0.5;
    }
}



/* Logos at the bottom */
.logos {
    position: relative;
    z-index: 10;
    margin-top: 40px;
    padding-top: 24px;
    border-top: 1px solid #374151;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 24px;
}
@media (min-width: 768px) {
    .logos {
        gap: 40px;
    }
}
@media (max-width: 768px) {
    .content-card{
      padding:0 0rem;
    }
    .content{
      padding: 0;
    }
    .title{
      font-size: 1.5rem;
    }
}
.logo-image {
    height: 24px;
    opacity: 0.6;
}
</style>