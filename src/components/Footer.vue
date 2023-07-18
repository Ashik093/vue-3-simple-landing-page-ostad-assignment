<template>
    <div class="site-footer">
        <div class="footer-dots"></div>
        <div class="container">
            <div class="row">
                <div class="col-lg-4">
                    <div class="widget">
                        <h3>About {{data.about.logo}}<span class="text-primary">.</span> </h3>
                        <p>{{data.about.desc}}</p>
                    </div>
                    <div class="widget">
                        <h3>Connect</h3>
                        <ul class="list-unstyled social">
                            <li v-for="(item,index) in data.socialmedia" :key="index"><a :href="item.link"><span :class="item.icon"></span></a></li>
                           
                        </ul>
                    </div>
                </div>
                <div class="col-lg-2 ml-auto">
                    <div class="widget">
                        <h3>Projects</h3>
                        <ul class="list-unstyled float-left links">
                            <li v-for="(item,index) in data.projects" :key="index"><a :href="item.link">{{item.name}}</a></li>
                            
                        </ul>
                    </div>
                </div>
                <div class="col-lg-2">
                    <div class="widget">
                        <h3>Services</h3>
                        <ul class="list-unstyled float-left links">
                            <li v-for="(item,index) in data.services" :key="index"><a :href="item.link">{{item.name}}</a></li>
                            
                        </ul>
                    </div>
                </div>
                <div class="col-lg-3">
                    <div class="widget">
                        <h3>Contact</h3>
                        <address>{{data.contact.address}}</address>
                        <ul class="list-unstyled links mb-4">
                            <li><a href="#">{{data.contact.phoneOne}}</a></li>
                            <li><a href="#">{{data.contact.phoneTwo}}</a></li>
                            <li><a href="#"><span class="__cf_email__" data-cfemail="cfa6a1a9a08fa2b6aba0a2aea6a1e1aca0a2">{{data.contact.email}}</span></a></li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="row mt-5">
                <div class="col-12 text-center">
                    <p>

                        Copyright &copy; All rights reserved | This template is made with <i class="icon-heart text-danger" aria-hidden="true"></i> by <a href="https://colorlib.com" target="_blank">Colorlib</a>
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
    const data={
       about:{
            logo:"Launch",
            desc:"Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts."
       },
       socialmedia:[
            {
                link:"#",
                icon:"icon-instagram",
               
            },
            {
                link:"#",
                icon:"icon-twitter",
               
            },
            {
                link:"#",
                icon:"icon-facebook",
               
            },
            {
                link:"#",
                icon:"icon-linkedin",
               
            },
            {
                link:"#",
                icon:"icon-pinterest",
               
            },
            {
                link:"#",
                icon:"icon-dribbble",
               
            }
       ],
       projects:[
            {
                name:"La Lega Stadium",
                link:"i#",
               
            },
            {
                name:"France Building",
                link:"#",
               
            },
            {
                name:"22 New Homes",
                link:"#",
               
            },
            {
                name:"Manage Center",
                link:"#",
               
            },
            {
                name:"Sports Hall",
                link:"i#",
               
            }
       ],
       services:[
            {
                name:"Architect",
                link:"i#",
               
            },
            {
                name:"Interior Design",
                link:"#",
               
            },
            {
                name:"Landscape Design",
                link:"#",
               
            },
            {
                name:"Consultancy",
                link:"#",
               
            }
       ],
       contact:{
            address:"43 Raymouth Rd. Baltemoer, London 3910",
            phoneOne:"+1(123)-456-7890",
            phoneTwo:"+1(123)-456-7890",
            email:"info@mydomain.com",
            domain:"https://Colorlib.com/",
       }
    }
</script>





