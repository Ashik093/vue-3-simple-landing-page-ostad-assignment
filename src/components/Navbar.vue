<template>
    <nav class="site-nav dark  mb-5 ">
        <div class="container">
            <div class="site-navigation">
                <a href="/" class="logo m-0 float-left">Launch<span class="text-primary">.</span></a>
                <ul class="js-clone-nav d-none d-lg-inline-block site-menu float-left">
                    <template v-for="(item,index) in data.menus" :key="index">
                        <li :class='[index==0?"active":"",item.hasChildren?"has-children":""]'>
                            <a :href="item.route" class="nav-link">{{ item.name }}</a>
                            <ul v-show="item.hasChildren" class="dropdown">

                                <template v-for="(row,i) in item.children" :key="i">
                                    <li :class='[item.hasChildren?"has-children":""]'>
                                        <a :href="row.route" class="nav-link">{{row.name}}</a>
                                        <ul v-show="row.hasChildren" class="dropdown">
                                            <template v-for="(r,j) in row" :key="j">
                                                <li><a :href="r.route" class="nav-link">{{r.name}}</a></li>
                                            </template>
                                            
                                        </ul>
                                    </li>

                                </template>

                                
                            </ul>
                        </li>

                    </template>
                   
                </ul>
                <ul class="js-clone-nav d-none mt-1 d-lg-inline-block site-menu float-right">
                    <template v-for="(item,index) in data.auth" :key="index">
                        <li :class="item.class"><a :href="item.route">{{item.name}}</a></li>
                    </template>
                    
                    
                </ul>
                <a href="#" class="burger ml-auto float-right site-menu-toggle js-menu-toggle d-inline-block dark d-lg-none" data-toggle="collapse" data-target="#main-navbar">
                    <span></span>
                </a>
            </div>
        </div>
    </nav>
</template>
<script setup>
    const data={
        title:"Launch",
        auth:[
            {
                name:"Sign in",
                class:"cta-button-outline",
                route:"/"
            },
            {
                name:"Register",
                class:"cta-primary",
                route:"/"
            }
        ],
        menus:[
            {
                name:"Home",
                route:"#home-section",
                hasChildren:false,
            },
            {
                name:"Dropdown",
                route:"#",
                hasChildren:true,
                children:[{
                    name:"Testimonials",
                    route:"#testimonials-section",
                    hasChildren:false,
                    
                },
                {
                    name:"Menu Two",
                    route:"#",
                    hasChildren:true,
                    children:[
                        {
                            name:"Sub Menu One",
                            route:"#"
                        },
                        {
                            name:"Sub Menu Two",
                            route:"#"
                        },
                    ]
                    
                },{
                    name:"Menu Three",
                    route:"#",
                    hasChildren:false,
                    
                }]
            },
            {
                name:"Feature",
                route:"#features-section",
                hasChildren:false,
            },
            {
                name:"Pricing",
                route:"#pricing-section",
                hasChildren:false,
            },
            {
                name:"About",
                route:"#about-section",
                hasChildren:false,
            },
            {
                name:"Contact",
                route:"#contact-section",
                hasChildren:false,
            }
        ]

    }
</script>