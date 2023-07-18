<template>
    <div class="untree_co-section" id="about-section">
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-lg-8">
                    <img :src="data.preview" alt="Image" class="img-fluid">
                </div>
                <div class="col-lg-4">
                    <div class="mb-4">
                        <span class="caption">{{data.subtitle}}</span>
                        <h2 class="heading">{{data.title}}</h2>
                    </div>
                    <div class="mb-4" v-html="data.text">
                        
                    </div>
                    <ul class="list-unstyled ul-check primary mb-4">
                        <li v-for="(item,index) in data.list" :key="index">{{item}}</li>
                        
                    </ul>
                    <div class="row count-numbers">
                        <div class="col-lg-6" v-for="(item,index) in data.counter" :key="index"> 
                            <span class="counter d-block"><span >{{item.number}}</span><span>{{item.unit}}</span></span>
                            <span class="caption-2">{{item.title}}</span>
                        </div>
                        
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
    const data={
        title:"About Us",
        subtitle:"ABOUT",
        preview:"https://preview.colorlib.com/theme/launch/images/about.svg",
        text:'<p>Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast</p><p>Separated they <span class="highlight">live in Bookmarksgrove right at the coast of the Semantics</span>, a large language ocean. A small river named Duden flows by their place and supplies it with the necessary regelialia.</p>',
        counter:[
            {
                title:"Members",
                number:"0",
                unit:"M",
            },
            {
                title:"Team",
                number:"0",
                unit:"M",
            }
        ],
        list:[
            "There live the blind texts",
            "Far far away behind the word",
            "Their place and supplies"
        ]
    }

</script>
