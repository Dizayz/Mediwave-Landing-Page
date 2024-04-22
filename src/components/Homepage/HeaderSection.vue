<script setup lang="ts">
import Container from "../Container.vue"


</script>

<template>
    <div class="header-section">
        <Container>
            <main>
                <nav>
                    <div class="img-container">
                        <img src="../../assets/images/mediwave-logo.png" alt="mediwave-logo">
                    </div>

                    <RouterLink to="/login" class="connexion"> Connexion</RouterLink>
                </nav>
                <div class="header-contenue">
                    <div class="header-detail">
                        <h1>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        </h1>
                        <h5>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Provident facere iste,
                            cumque repellendus debitis dolorem blanditiis obcaecati ex exercitationem at!</h5>
                        <button>Commencer gratuitement</button>
                    </div>
                    <div class="header-img">
                        <img src="../../assets/images/medecine-pic.svg" alt="svg">
                    </div>
                </div>
                <div class="footer-header">
                    <div class="item"><font-awesome-icon :icon="['far', 'circle-check']" class="inset-color" />
                        <p>Contenu riche et fiable</p>
                    </div>
                    <div class="item"><font-awesome-icon :icon="['far', 'circle-check']"  class="inset-color"/>
                        <p>Plateforme stable
                        </p>
                    </div>
                    <div class="item"><font-awesome-icon :icon="['far', 'circle-check']"  class="inset-color"/>
                        <p>Application mobile</p>
                    </div>
                </div>
            </main>
        </Container>
    </div>
</template>

<style scoped>
.header-section {
    background-image: url('../../assets/images/background.jpg');
}

main {
    position: relative;
    padding-bottom: 80px;
}

.footer-header {
    width: 100%;
    padding: 30px 60px;
    display: flex;
    flex-wrap: wrap;
    background-color: #f5f5f5;
    border-radius: 10px;
    margin-top: 50px;
    margin-bottom: -160px;
    box-shadow: -1px 8px 28px 1px rgba(0, 0, 0, 0.39);
    -webkit-box-shadow: -1px 8px 28px 1px rgba(0, 0, 0, 0.39);
    -moz-box-shadow: -1px 8px 28px 1px rgba(0, 0, 0, 0.39);
    gap: 15px;

}

.footer-header .item {
    display: flex;
    gap: 10px;
    align-items: center;
    font-size: 1.3rem;
    margin: auto;

}

.footer-header p {
    color: black;
    font-weight: 500;
    white-space: nowrap;
}

.header-contenue {
    display: flex;
    align-items: center;
    gap: 30px;

}

.header-img {
    width: 50%;
}

.header-img img {
    width: 100%;
    object-fit: cover;
}

.header-detail {

    color: white;
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.header-detail h1 {
    font-size: 3rem;
    font-weight: 700;
    line-height: 1.2;
       
}

.header-detail h5 {
    font-size: 1.3rem;
}

.header-detail button {
    width: fit-content;
    background-color: #f78000;
    color: white;
    font-size: 1.2rem;
    font-weight: 600;
    padding: 15px 30px;
    border-radius: 10px;
    border: none;
    margin-top: 30px;
}



nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 25px;
    gap: 3rem;
}

.img-container {
    width: 200px;
}

.img-container img {
    width: 100%;
}

.connexion {
    padding: 10px 20px;
    background-color: #f78000;
    border-radius: 10px;
    text-decoration: none;
    font-size: 1.1rem;
    font-weight: 700;
    color: white;
}

@media (max-width:1080px) {
    .header-contenue {
        flex-direction: column;
        align-items: left;
        gap: 50px;
    }

    .footer-header {
        text-align: left;
    }
}
</style>