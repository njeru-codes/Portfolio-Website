<template>
    <div class="experience-wrapper">
        <div class="container">
            <h2 class="section-title">Experience</h2>
            <div class="timeline">
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="dates">October 2025 - Present</span>
                        <h3 class="company">Foresight Tech Group</h3>
                        <p class="position">Information Security Engineer</p>
                        <ul class="duties">
                            <li>Escalate validated and confirmed incidents to the incident response team and notify clients of required mitigation actions.</li>
                            <li>Perform log analysis from diverse sources (FW, IDS, Windows DC, Cisco appliances, AV, email security, etc.).</li>
                            <li>Conduct threat intel research, run sandbox static analysis, and track/update incidents in line with client updates.</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="dates">March 2025 – October 2025</span>
                        <h3 class="company">Durrafx Liquiduity Limited</h3>
                        <p class="position">Software Developer</p>
                        <ul class="duties">
                            <li>Designed and developed DurraPay, a custom Payment Service Provider (PSP) system to streamline payment collections and disbursements.</li>
                            <li>Integrated secure payment workflows and APIs to handle transactions for both individual users and business clients.</li>
                            <li>Implemented robust authentication mechanisms, including JWT with device-level session control.</li>
                            <li>Conducted security assessments and applied best practices to harden application infrastructure.</li>
                        </ul>
                    </div>
                </div>
                
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="dates">Jan 2025 – March 2025</span>
                        <h3 class="company">PayheroKenya</h3>
                        <p class="position">Security Analyst Intern</p>
                        <ul class="duties">
                            <li>Documented findings and created technical reports to communicate risks and remediation steps to stakeholders.</li>
                            <li>Supported the development of internal security policies and best practices.</li>
                        </ul>
                    </div>
                </div>

                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-content">
                        <span class="dates">August 2024 - Jan 2025</span>
                        <h3 class="company">254m-Derivmpesa</h3>
                        <p class="position">Penetration Tester</p>
                        <ul class="duties">
                            <li>Conducted vulnerability assessments and penetration tests on internal systems and web applications.</li>
                            <li>Identified and documented security weaknesses, misconfigurations, and potential exploits.</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>
.experience-wrapper {
    background-color: #0a1320;
    color: #e5e7eb;
    padding: 80px 16px;
    font-family: Arial, sans-serif;
    background: #000;
}

.container {
    max-width: 960px;
    margin: 0 auto;
    padding: 0 16px;
}

.section-title {
    font-size: 2.25rem;
    font-weight: 700;
    text-align: center;
    color: white;
    margin-bottom: 48px;
}

.timeline {
    position: relative;
    /* Adjust padding to make space for the dot inside the line */
    padding-left: 0; 
    border-left: 2px solid #00e396; /* The main vertical line */
}

.timeline-item {
    position: relative;
    /* Adjust padding for the content to align with the line */
    padding: 24px 0 24px 60px; /* Increased left padding to push content right */
}

.timeline-dot {
    position: absolute;
    /* Adjust 'left' to align with the border-left of the .timeline */
    left: -12px; /* Half of its width to center it on the 2px line */
    top: 50%;
    transform: translateY(-50%);
    width: 24px;
    height: 24px;
    border: 2px solid #00e396;
    border-radius: 50%;
    background-color: #0a1320; /* Background color to hide the line segment behind it */
    z-index: 10;
    display: flex;
    justify-content: center;
    align-items: center;
}

.timeline-dot::after {
    content: '';
    display: block;
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background-color: #00e396;
    animation: pulse 2s infinite cubic-bezier(0.4, 0, 0.6, 1);
}

@keyframes pulse {
    0%, 100% {
        transform: scale(0.8);
        opacity: 0.6;
    }
    50% {
        transform: scale(1.1);
        opacity: 1;
    }
}

.timeline-content {
    background-color: #0d192a;
    padding: 24px;
    border-radius: 8px;
    border: 1px solid #374151;
}

.dates {
    display: block;
    font-size: 0.875rem;
    color: #00e396;
    font-weight: 600;
    margin-bottom: 8px;
}

.company {
    font-size: 1.5rem;
    font-weight: 700;
    color: white;
    margin: 0 0 4px 0;
}

.position {
    font-size: 1rem;
    font-weight: 400;
    color: #e5e7eb;
    margin: 0 0 16px 0;
}

.duties {
    list-style: none;
    padding: 0;
    margin: 0;
    color: #9ca3af;
}

.duties li {
    position: relative;
    padding-left: 20px;
    margin-bottom: 8px;
    font-size: 0.875rem;
}

.duties li::before {
    content: '•';
    color: #00e396;
    font-size: 1.25rem;
    position: absolute;
    left: 0;
    top: -2px;
}
</style>