<template>
    <div class="untree_co-section" id="features-section">
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-lg-4">
                    <span class="caption">{{data.caption}}</span>
                    <h3 class="heading mb-4">{{data.heading}}</h3>
                    <div class="mb-4">
                        <p>{{data.description}}</p>
                        <ul class="list-unstyled ul-check primary">
                            <template v-for="(item,index) in data.list" :key="index">
                                <li>{{item}}</li>
                            </template>
                            
                        </ul>
                    </div>
                    <div class="mb-4">
                        <div class="untree_co-testimonial d-flex">
                            <div class="text">
                                <blockquote v-html="data.qoute.text">
                                   
                                </blockquote>
                                <div class="author d-flex">
                                    <div class="pic mr-3">
                                        <img :src="data.qoute.image" alt="Image" class="img-fluid">
                                    </div>
                                    <div>
                                        <strong class="d-block">{{data.qoute.name}}</strong><span class="d-block">{{data.qoute.possition}}</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-lg-7">
                    <a :href="data.video" class="btn-video">
                        <span class="wrap-icon-play">
<svg class="bi bi-play-fill" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
<path d="M11.596 8.697l-6.363 3.692c-.54.313-1.233-.066-1.233-.697V4.308c0-.63.692-1.01 1.233-.696l6.363 3.692a.802.802 0 0 1 0 1.393z" />
</svg>
</span>
                        <img :src="data.previewImage" class="img-fluid img-shadow">
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup> 
    const data={
        caption:"Digital Services",
        heading:"Selling Digital Services",
        description:"Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast",
        list:[
            "There live the blind texts","Far far away behind the word"
        ],
        video:"https://www.youtube.com/watch?v=mwtbEGNABWU&t=9s",
        previewImage:"https://preview.colorlib.com/theme/launch/images/dashboard.jpg.webp",
        qoute:{
            name:"James Anderson",
            possition:"Facebook, Product Lead",
            image:"https://preview.colorlib.com/theme/launch/images/person_1.jpg",
            text:'&ldquo;Separated they <span class="highlight">live in Bookmarksgrove right at the coast of the Semantics</span>, a large language ocean. A small river named Duden flows by their place and supplies it with the necessary regelialia. &rdquo;'
        },
    }
</script>