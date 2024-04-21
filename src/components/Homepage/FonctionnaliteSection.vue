
<script setup lang="ts">
import Container from '../Container.vue'

</script>


<template>
    <div class="main">
        <Container>
            <div class="header">
                <h1>Fonctionnalités</h1>
            </div>
            <div class="fonctionaliter-grid">
                <div class="fonction">
                    <div> <font-awesome-icon class="icon" :icon="['fas', 'list-check']" /></div>
                    <h2>Lorem, ipsum.</h2>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                </div>
                <div class="fonction">
                    <div> <font-awesome-icon class="icon" :icon="['fas', 'list-check']" /></div>
                    <h2>Lorem, ipsum.</h2>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                </div>
                <div class="fonction">
                    <div> <font-awesome-icon class="icon" :icon="['fas', 'list-check']" /></div>
                    <h2>Lorem, ipsum.</h2>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                </div>
                <div class="fonction">
                    <div> <font-awesome-icon class="icon" :icon="['fas', 'list-check']" /></div>
                    <h2>Lorem, ipsum.</h2>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                </div>
                <div class="fonction">
                    <div> <font-awesome-icon class="icon" :icon="['fas', 'list-check']" /></div>
                    <h2>Lorem, ipsum.</h2>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                </div>
                <div class="fonction">
                    <div> <font-awesome-icon class="icon" :icon="['fas', 'list-check']" /></div>
                    <h2>Lorem, ipsum.</h2>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                </div>
                <div class="fonction">
                    <div> <font-awesome-icon class="icon" :icon="['fas', 'list-check']" /></div>
                    <h2>Lorem, ipsum.</h2>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                </div>
                <div class="fonction">
                    <div> <font-awesome-icon class="icon" :icon="['fas', 'list-check']" /></div>
                    <h2>Lorem, ipsum.</h2>
                    <p>Lorem ipsum dolor sit amet consectetur.</p>
                </div>
            </div>
        </Container>

    </div>
</template>
<style scoped>
.main {
    margin: 50px 0;
}

.fonctionaliter-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
}

h2 {
    font-size: 1.6rem;
    font-weight: 600;
        color: black;
}

p {
    font-size: 1.2rem;
        color: black;
}

.fonction {
    border: 1px solid rgba(128, 128, 128, 0.363);
    width: fit-content;
    padding: 40px;
    display: flex;
    flex-direction: column;
    align-items: left;
    justify-content: center;
    gap: 1rem;
    margin: auto;
}

.icon {
    font-size: 2.4rem;
    color: #F78000;
}

.header {
    text-align: center;
    margin: 50px 0 70px 0;
}

.header h1 {
    font-size: 2.5rem;
    font-weight: 700;
    margin-bottom: 15px;
        color: black;
}

@media (max-width:1150px) {
    .fonctionaliter-grid {
        grid-template-columns: repeat(3, 1fr);
    }
}

@media (max-width:850px) {
    .fonctionaliter-grid {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width:600px) {
    .fonctionaliter-grid {
        grid-template-columns: 1fr;
    }
}
</style>


