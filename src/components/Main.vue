<script setup>
import { ref } from 'vue'

const paragraf1 = ref("I am incredibly small and fast! My core library is only around 30KB, so I won't slow you down.")
const paragraf2 = ref("Easy to learn and use, even for beginners. I have a gentle learning curve, clear documentation, and a supportive community.")
const paragraf3 = ref("I can handle everything from simple interactive elements to complex single-page applications. I'm great for small projects and large - scale applications alike.")

const href = ref("https://instagram.com/nonedity")
const isBtnDisabled = ref(true)
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

            <div class="buttons">
                <button target="__blank" :href>My Instagram!</button>
                <button :disabled="isBtnDisabled">This is a disabled button.</button>
            </div>
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

.buttons {
    display: grid;
    grid-template-columns: 2fr 1fr;
}

button {
    background: #34495e;
    color: white;
    padding: 10px;
    border: 0;
    font-size: 1.1rem;
    border-radius: 0 5px 0 5px;
    font-weight: bold;
    margin: 15px 15px 0 0;
    cursor: pointer;
    transition: transform 0.2s;
}

button:hover {
    transform: scale(1.05);
}

button:disabled {
    background: grey;
    cursor: not-allowed;
    opacity: 0.5;
}
</style>