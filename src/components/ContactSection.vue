<template>
    <div class="untree_co-section" id="contact-section">
        <div class="container">
            <div class="row mb-4">
                <div class="col-12 text-center">
                    <h2 class="heading">Get In Touch</h2>
                    <p>Far from the countries Vokalia and Consonantia</p>
                </div>
            </div>
            <div class="row">
                <div class="col-lg-7">
                    <form class="contact-form">
                        <div class="row">
                            <div class="col-6">
                                <div class="form-group">
                                    <label class="" for="fname">First name</label>
                                    <input type="text" class="form-control" id="fname">
                                </div>
                            </div>
                            <div class="col-6">
                                <div class="form-group">
                                    <label class="" for="lname">Last name</label>
                                    <input type="text" class="form-control" id="lname">
                                </div>
                            </div>
                        </div>
                        <div class="form-group">
                            <label class="" for="email">Email address</label>
                            <input type="email" class="form-control" id="email">
                        </div>
                        <div class="form-group">
                            <label class="" for="message">Message</label>
                            <textarea name="" class="form-control" id="message" cols="30" rows="5"></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary">Send Message</button>
                    </form>
                </div>
                <div class="col-lg-4 ml-auto">
                    <h3 class="h5 mb-4">Contact Info</h3>
                    <address class="text-black d-flex"><span class="mt-1 icon-room mr-2"></span><span>{{data.address}}</span></address>
                    <ul class="list-unstyled ul-links mb-4">
                        <li><a href="#" class="d-flex"><span class="mt-1 icon-phone mr-2"></span><span>{{data.phoneOne}}</span></a></li>
                        <li><a href="#" class="d-flex"><span class="mt-1 icon-phone mr-2"></span><span>{{data.phoneTwo}}</span></a></li>
                        <li><a href="#" class="d-flex"><span class="mt-1 icon-envelope mr-2"></span><span><span class="__cf_email__" data-cfemail="167f787079567b6f72797b777f783875797b">{{data.email}}</span></span></a></li>
                        <li><a :href="data.domain" target="_blank" class="d-flex"><span class="mt-1 icon-globe mr-2"></span><span>{{data.domain}}</span></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
    const data={
        address:"43 Raymouth Rd. Baltemoer, London 3910",
        phoneOne:"+1(123)-456-7890",
        phoneTwo:"+1(123)-456-7890",
        email:"info@mydomain.com",
        domain:"https://Colorlib.com/",

    }
</script>
