<template>
    <div class="untree_co-hero" id="home-section">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-12">
                    <div class="dots"></div>
                    <div class="row align-items-center">
                        <div class="col-lg-7 ml-auto order-lg-2">
                            <img :src="data.image" alt="Image" class="img-fluid">
                        </div>
                        <div class="col-lg-5">
                            <h1 class="heading">{{ data.title }}</h1>
                            <div class="excerpt">
                                <p v-html="data.description"></p>
                            </div>
                            <p data-aos="fade-up">
                                <a href="#features-section" class="btn btn-primary smoothscroll">See Features</a>
                                <a href="#pricing-section" class="btn btn-outline-primary smoothscroll">Pricing</a>
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
const data={
        title:"Promote Your Products by Colorlib",
        description:'Another cool free html css template by <a href="#" target="_blank" class="highlight">Colorlib</a> Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast',
        image:"https://preview.colorlib.com/theme/launch/images/market-launch-pana.svg"
    }
</script>