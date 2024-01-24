

<script setup lang="ts">
import { ref, onMounted } from "vue";
import Container from '../Container.vue';

const testimonials = ref([
    { text: 'Testimonial 1', author: 'Author 1', img: 'https://img.freepik.com/free-photo/happiness-wellbeing-confidence-concept-cheerful-attractive-african-american-woman-curly-haircut-cross-arms-chest-self-assured-powerful-pose-smiling-determined-wear-yellow-sweater_176420-35063.jpg', isShow: true },
    { text: 'Testimonial 2 Testimonial 2Testimonial  Testimonial 2 Testimonial 2Testimonial 2Testimonial 2Testimonial Testimonial 2 Testimonial 2Testimonial 2Testimonial 2Testimonial 2Testimonial 2Testimonial 2Testimonial 2Testimonial 2', author: 'Author 2', img: 'https://image.shutterstock.com/image-photo/image-young-asian-woman-company-260nw-2122700972.jpg', isShow: false },
    { text: 'Testimonial 3', author: 'Author 3', img: 'https://i0.wp.com/post.healthline.com/wp-content/uploads/2021/02/Left-Handed-Male-Writing-1296x728-Header.jpg?w=1155&h=1528', isShow: false }
]);

const totalSlides = testimonials.value.length;
const currentSlide = ref(0);
const nextSlide = () => {
    testimonials.value[currentSlide.value].isShow = !testimonials.value[currentSlide.value].isShow
    currentSlide.value = (currentSlide.value + 1) % totalSlides;
    testimonials.value[currentSlide.value].isShow = !testimonials.value[currentSlide.value].isShow


};

onMounted(() => {
    // Start auto-sliding (adjust the interval as needed)
    setInterval(nextSlide, 4000);
});

</script>

<template>
    <div class="bgcolor">
        <Container>
            <div class="header">
                <h1>Recommandé par les majeurs</h1>
                <h4>Ne prends pas notre parole. Écoutes les lauréats des années passées.</h4>
            </div>
            <div class="bgwhite">
                <transition name="fade" mode="out-in">
                    <div :key="currentSlide" class="testimonial" v-if="testimonials[currentSlide].isShow">
                        <div class="pic"> <img :src=testimonials[currentSlide].img alt=""></div>
                        <p>{{ testimonials[currentSlide].text }}</p>
                        <h6>{{ testimonials[currentSlide].author }}</h6>
                        <p> Major Résidanat Sidi Bel Abbes 2023</p>
                    </div>
                </transition>
            </div>
        </Container>
    </div>
</template>


<style scoped>
.bgcolor {
    background-color: #0025f75d;
    padding-bottom: 70px;
}

.testimonial {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 20px;
    margin: 2rem 0;
}

.pic {
    width: 200px;
    height: 200px;
    border-radius: 360px;
    overflow: hidden;
    margin-bottom: 20px;
}

.pic img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.testimonial p {
    width: 70%;
    text-align: center;
    font-size: 1.1rem;
    font-weight: 400;
}

.testimonial h6 {
    font-size: 1.3rem;
    font-weight: 600;


}

.bgwhite {
    background-color: #f5f5f5;
    padding: 4rem 0;
    position: relative;
}

.header {
    text-align: center;
    margin: 50px 0 70px 0;
}

.header h1 {
    font-size: 2.5rem;
    font-weight: 700;
    margin-bottom: 15px;
}

.header h4 {
    font-size: 1.5rem;
    font-weight: 500;
}

.fade-enter-from {
    opacity: 0;
}

.fade-enter-to {
    opacity: 1;

}


.fade-enter-active {
    transition: opacity 1s;

}

.fade-leave-from {
    opacity: 1;

}

.fade-leave-to {
    opacity: 0;

}

.fade-leave-active {
    transition: opacity 1s;
}
</style>