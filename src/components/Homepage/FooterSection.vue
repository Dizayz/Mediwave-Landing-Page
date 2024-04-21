
<script setup lang="ts">
import Container from "../Container.vue"

</script>


<template>
    <Container>
        <main>
            <div class="apps">
                <h3> Télécharger notre application</h3>
                <div class="text-img">
                    <a href="javascript:;"> <img
                            src="https://siamoisco.swipepages.media/2022/10/60f4bbb7a687f800106bfa3d/google-play-badge.svg"
                            alt=""></a>
                </div>
            </div>
            <div class="plus-info">
                <h3> En savoir plus</h3>
                <a href="javascript:;">Centre d'aide </a>
                <a href="javascript:;">FAQ </a>
                <a href="javascript:;">Politique de confidentialité</a>
                <a href="javascript:;">Conditions d'utilisation</a>
            </div>
            <div class="useful-links">
                <h3>Lien utiles </h3>
                <a href="javascript:;">Tarification </a>
                <a href="javascript:;">Blog </a>
                <a href="javascript:;">Avis des utilisateurs</a>
                <div class="social-links">
                    <font-awesome-icon class="icon" :icon="['fab', 'square-facebook']" />
                    <font-awesome-icon class="icon" :icon="['fab', 'square-instagram']" />
                    <font-awesome-icon class="icon" :icon="['fab', 'linkedin']" />
                </div>
            </div>
        </main>
        <hr>
        <div class="copyright">
            <div class="img-container">
                <img src="../../assets/images/mediwave-logo.png" alt="mediwave-logo">
            </div>
            <h4>
                Tous les droits sont réservés © 2023 MediWave</h4>
        </div>
    </Container>
</template>

<style scoped>
main {
    display: flex;
    flex-wrap: wrap;
    margin: 50px 0;
    justify-content: space-around;

}

.apps,
.plus-info,
.useful-links {
    display: flex;
    flex-direction: column;
    gap: 0.3rem;
    padding: 10px;
}

a {
    text-decoration: none;
    font-size: 1.2rem;
    font-weight: 400;
    width: fit-content;
    
}

a:hover {
    border-bottom: 1px solid blue;
}

h3 {
    font-size: 1.2rem;
    font-weight: 500;
    margin-bottom: 15px;    color: black;
}

.social-links {
    display: flex;
    gap: 15px;
    margin-top: 10px;
}

.icon {
    font-size: 2.2rem;
    cursor: pointer;
    color: #5E17EB;
}

.img-container {
    width: 200px;
}

.img-container img {
    width: 100%;
}

.copyright {
    margin: 40px 0 20px 0;
    display: flex;
    align-items: center;
    gap: 50px;
}

h4 {
    font-size: 1.2rem;
        color: black;
}

@media (max-width:760px) {
    main>* {
        margin-right: auto;
    }
}
</style>