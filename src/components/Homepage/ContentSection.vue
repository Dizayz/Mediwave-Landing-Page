
<script setup lang="ts">
import Container from '../Container.vue';

</script>

<template>
    <main>
        <Container>
            <h1>L'indispensable pour réussir</h1>
            <div class="content">
                <div class="content-item">
                    <div class="content-item-text">
                        <h4>Personnalise ta révision</h4>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Non minima perspiciatis fugiat modi
                            minus
                            repellat.
                        </p>
                        <button class="content-item-btn">Essaye maintenant</button>
                    </div>
                    <div class="content-item-img"><img src="../../assets/images/content-section.svg" alt=""></div>
                </div>
                <div class="content-item reverse">
                    <div class="content-item-img"><img src="../../assets/images/content-section.svg" alt=""></div>
                    <div class="content-item-text right">
                        <h4>Mémorise plus facilement</h4>
                        <div class="text-list">
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                        </div>
                        <button class="content-item-btn">Essaye maintenant</button>
                    </div>
                </div>
                <div class="content-item">
                    <div class="content-item-text">
                        <h4>Reste à jour</h4>
                        <div class="text-list">
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                        </div>
                        <button class="content-item-btn">Essaye maintenant</button>
                    </div>
                    <div class="content-item-img"><img src="../../assets/images/content-section.svg" alt=""></div>
                </div>
                <div class="content-item reverse">
                    <div class="content-item-img"><img src="../../assets/images/content-section.svg" alt=""></div>
                    <div class="content-item-text right">
                        <h4>Découvre tes points faibles</h4>
                        <div class="text-list">
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                        </div>
                        <button class="content-item-btn">Essaye maintenant</button>
                    </div>
                </div>
                <div class="content-item">
                    <div class="content-item-text">
                        <h4>Soit prêt la veille d'examen</h4>
                        <div class="text-list">
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                            <p> <font-awesome-icon :icon="['far', 'circle-check']" size="xl" class="icon" /> Lorem, ipsum
                                dolor.</p>
                        </div>
                        <button class="content-item-btn">Essaye maintenant</button>
                    </div>
                    <div class="content-item-img"><img src="../../assets/images/content-section.svg" alt=""></div>
                </div>
            </div>
        </Container>
    </main>
</template>

<style scoped>
main {
    margin-top: 100px;
}

h1 {
    text-align: center;
    font-size: 2.5rem;
    font-weight: 700;
    margin-bottom: 50px;
        color: black;
}

.content {

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 2rem;
}

.right {
    text-align: right;
}

.right>button {
    margin-left: auto;
}


.content-item {
    display: flex;
    align-items: center;
    justify-content: center;
}

.content-item-img,
.content-item-text {
    flex: 1;
    padding: 20px 40px;
}

.content-item-text {
    width: 100%;
    display: flex;
    flex-direction: column;
    gap: 30px;
}

.content-item-btn {
    padding: 18px 22px;
    background-color: #f78000;
    text-decoration: none;
    font-size: 1.1rem;
    font-weight: 700;
    color: white;
    width: fit-content;
    border: none;
    cursor: pointer;

}

.content-item-img img {
    width: 100%;
    object-fit: cover;
    box-shadow: 0px 5px 15px 2px rgba(0, 0, 0, 0.39);
}

h4 {
    font-size: 1.8rem;
    font-weight: 600;
        color: black;

}

p {
    font-size: 1.2rem;
    font-weight: 400;
        color: black;
}

.text-list {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.text-list p {
    font-size: 1.2rem;
        color: black;
}

.icon {
    margin-right: 10px;
        color: black;
}

@media (max-width:900px) {

    .content-item {
        display: flex;
        flex-direction: column;
    }

    .reverse {
        flex-direction: column-reverse;
    }

    .right {
        text-align: left;
    }

    .right>button {
        margin-left: 0;
        margin-right: auto;
    }
}
</style>