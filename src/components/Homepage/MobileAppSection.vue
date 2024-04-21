
<script setup lang="ts">
import Container from '../Container.vue'

</script>

<template>
    <main>
        <Container>
            <div class="content">
                <div class="text-content">
                    <h1> Lorem ipsum dolor sit amet consectetur !</h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rem cumque
                        , pariatur beatae numquam suscipit illo!</p>
                    <div class="text-img">
                        <a href="javascript:;"> <img
                                src="https://siamoisco.swipepages.media/2022/10/60f4bbb7a687f800106bfa3d/google-play-badge.svg"
                                alt=""></a>
                    </div>
                </div>
                <div class="img-content">
                    <img src="../../assets/images/smartphone.png" alt="">
                </div>
            </div>
        </Container>

    </main>
</template>

<style scoped>
main {
    background-color: #0025f75d;
    padding: 6rem 0;
}

.content {
    display: flex;
    justify-content: center;
    gap: 20px;
}



.img-content {
    width: 40rem;
    position: relative;
    overflow: hidden;
}

.img-content>img {
    width: 100%;
    object-fit: cover;

}

.text-content {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    justify-content: center;
    text-align: left;

}

h1 {
    font-size: 2.4rem;
    line-height: 1.2;
    font-weight: 700;
     color: black;
}

p {
    font-size: 1.4rem;
     color: black;
}

@media (max-width:850px) {
    .content {
        flex-direction: column;
    }

    .img-content {
        width: 100%;
        height: 400px;
        position: relative;
    }

    .img-content img {
        width: 300px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    main {
        padding: 3rem 0;
    }
}
</style>