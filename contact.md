---
layout: default
title: Contact
permalink: /contact/
---

<section class="hero" style="min-height: 80vh;">
    <div class="hero-content fade-in">
        <h1>Get In Touch</h1>
        <p>I'm always excited to collaborate on innovative ML/AI projects or discuss opportunities in the field. Let's connect!</p>

        <div class="contact-info">
            <a href="mailto:{{ site.author.email }}" class="contact-item">
                <span>📧</span>
                <span>{{ site.author.email }}</span>
            </a>
            <a href="{{ site.author.linkedin }}" target="_blank" rel="noopener" class="contact-item">
                <span>💼</span>
                <span>LinkedIn</span>
            </a>
            <a href="{{ site.author.github }}" target="_blank" rel="noopener" class="contact-item">
                <span>💻</span>
                <span>GitHub</span>
            </a>
            <a href="tel:{{ site.author.phone | remove: ' ' | remove: '(' | remove: ')' | remove: '-' }}" class="contact-item">
                <span>📱</span>
                <span>{{ site.author.phone }}</span>
            </a>
        </div>

        <div style="margin-top: 3rem;">
            <h2 style="color: #64ffda; margin-bottom: 1rem;">Let's Build Something Amazing Together</h2>
            <p>Whether you're looking to collaborate on research, need ML consulting, or want to discuss the latest in AI, I'd love to hear from you.</p>
        </div>
    </div>
</section>
