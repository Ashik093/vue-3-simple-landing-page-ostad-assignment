<template>
    <div class="untree_co-section bg-light" id="pricing-section">
        <div class="container">
            <div class="row pricing-title">
                <div class="col-12 text-center">
                    <h2 class="heading">{{data.title}}</h2>
                    <p>{{data.subtitle}}</p>
                </div>
            </div>
            <div class="row justify-content-center">
                <div class="col-lg-10">
                    <div class="row">
                        <div class="col-lg-4" v-for="(item,index) in data.prices" :key="index">
                            <div class="pricing">
                                <div class="body">
                                    <div class="price">
                                        <span class="d-block plan">{{item.title}}</span>
                                        <span class="price"><sup>$</sup><span>{{item.amount}}</span></span>
                                    </div>
                                    <ul class="list-unstyled ul-check primary mb-5">
                                        <li v-for="(row,i) in item.feature" :key="i">{{row}}</li>
                                        
                                    </ul>
                                    <p class="text-center mb-0"><a href="#" class="btn " :class="item.class">Get Started</a></p>
                                </div>
                            </div>
                        </div>
                        
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
    const data={
        title:"Pricing",
        subtitle:"Pricing for everyone. Choose your plan now!",
        prices:[{
            title:"Free",
            amount:0,
            class:"btn-outline-primary",
            feature:[
                "There live the blind texts",
                "Far far away behind the word",
                "Far from the countries Vokalia and Consonantia"
            ]

        },{
            title:"Standard",
            amount:19.99,
            class:"btn-primary",
            feature:[
                "There live the blind texts",
                "Far far away behind the word",
                "Far from the countries Vokalia and Consonantia"
            ]

        },{
            title:"Premium",
            amount:79.99,
            class:"btn-outline-primary",
            feature:[
                "There live the blind texts",
                "Far far away behind the word",
                "Far from the countries Vokalia and Consonantia"
            ]

        }]
    }
</script>

