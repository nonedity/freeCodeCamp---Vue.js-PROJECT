<script setup>
import { ref } from 'vue'

const paragraf1 = ref("I am incredibly small and fast! My core library is only around 30KB, so I won't slow you down.")
const paragraf2 = ref("Easy to learn and use, even for beginners. I have a gentle learning curve, clear documentation, and a supportive community.")
const paragraf3 = ref("I can handle everything from simple interactive elements to complex single-page applications. I'm great for small projects and large - scale applications alike.")
</script>

<template>
    <main>
        <section>
            <h2>
                I'm <span class="highlight">Lightweight</span>
            </h2>
            <p>{{ paragraf1 }}</p>
        </section>
        <section>
            <h2>
                I'm <span class="highlight">Approachable</span>
            </h2>
            <p>{{ paragraf2 }}</p>
        </section>
        <section>
            <h2>
                I'm <span class="highlight">Versatile</span>
            </h2>
            <p>{{ paragraf3 }}</p>
        </section>
    </main>
</template>

<style scoped>
main {
    margin-top: 15px;
}

section {
    margin-top: 25px;
}

h2 {
    font-size: 1.3rem;
    color: #34495e;
    margin-bottom: 3px;
}

p {
    font-size: 0.9rem;
    color: #555;
}
</style>