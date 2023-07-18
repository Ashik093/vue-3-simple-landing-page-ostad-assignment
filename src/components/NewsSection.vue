<template>
    <div class="untree_co-section bg-light">
        <div class="container">
            <div class="row mb-4">
                <div class="col-12 text-center">
                    <h2 class="heading">{{data.title}}</h2>
                    <p>{{data.subtitle}}</p>
                </div>
            </div>
            <div class="row">
                <div class="col-md-6 mb-4 mb-lg-0 col-lg-4" v-for="(item,index) in data.news" :key="index">
                    <div class="news-item">
                        <div class="vcard d-flex align-items-center mb-4">
                            <div class="img-wrap">
                                <img :src="item.image" alt="Image" class="img-fluid">
                            </div>
                            <div class="post-meta">
                                <strong>Posted by {{item.name}}</strong>
                                <span>{{item.date}}</span>
                            </div>
                        </div>
                        <div class="news-contents mb-4">
                            <span class="post-meta-2">{{item.meta}}</span>
                            <h3><a href="#">{{item.description}}</a></h3>
                        </div>
                        <p class="mb-0">
                            <a href="#" class="read-more-arrow">
                                <svg class="bi bi-arrow-right" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" d="M10.146 4.646a.5.5 0 0 1 .708 0l3 3a.5.5 0 0 1 0 .708l-3 3a.5.5 0 0 1-.708-.708L12.793 8l-2.647-2.646a.5.5 0 0 1 0-.708z" />
<path fill-rule="evenodd" d="M2 8a.5.5 0 0 1 .5-.5H13a.5.5 0 0 1 0 1H2.5A.5.5 0 0 1 2 8z" />
</svg>
                            </a>
                        </p>
                    </div>
                </div>
               
            </div>
        </div>
    </div>
</template>
<script setup>
    const data={
        title:"Our News",
        subtitle:"Far from the countries Vokalia and Consonantia",
        news:[
            {
                by:"James",
                image:"https://preview.colorlib.com/theme/launch/images/person_1.jpg",
                date:"Jun 14, 2020",
                meta:"Digital Service, 4 min read",
                description:"Far far away behind the word mountains far from the countries"
            }
            ,{
                by:"James",
                image:"https://preview.colorlib.com/theme/launch/images/person_1.jpg",
                date:"Jun 14, 2020",
                meta:"Digital Service, 4 min read",
                description:"Far far away behind the word mountains far from the countries"
            }
            ,{
                by:"James",
                image:"https://preview.colorlib.com/theme/launch/images/person_1.jpg",
                date:"Jun 14, 2020",
                meta:"Digital Service, 4 min read",
                description:"Far far away behind the word mountains far from the countries"
            }
        ]
    }
</script>