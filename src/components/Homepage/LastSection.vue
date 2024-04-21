
<script setup lang="ts">
import Container from '../Container.vue'

</script>

<template>
    <div class="rajel">
        <Container>
            <main>
                <h1>Commence dès maintenant</h1>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cum, est. Odio quasi vero rerum sed?</p>
                <button>Ouvrir un compte</button>
            </main>
        </Container>
    </div>
    <div class="anounce-bar">
        <Container>
            <h2>Vous aimerez réussir? Nous vous aiderons à l'accomplir!</h2>
        </Container>
    </div>
</template>

<style scoped>
.rajel {
    margin: 100px 0;
}

main {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
    width: 100%;
    background-image: url('../../assets/images/background.jpg');
    justify-content: center;
    align-items: center;
    color: white;
    padding: 80px 10px;
}

h1 {
    text-align: center;
    font-size: 2.7rem;
    font-weight: 700;


}

p {
    text-align: center;
    font-size: 1.3rem;

}

button {
    text-align: center;
    font-size: 1.3rem;
    font-weight: 600;
    color: white;
    background-color: #F78000;
    padding: 15px 20px;
    border: none;
    margin-top: 20px;
    cursor: pointer;
    transition: all ease-out 0.3s;
    width: fit-content;
}

button:hover {
    color: #F78000;
    background-color: transparent;
    border: 1px solid #F78000;

}

.anounce-bar {
    background-image: url('../../assets/images/background.jpg');
}

h2 {
    font-size: 1.8rem;
    font-weight: 500;
    color: white;
}
</style>