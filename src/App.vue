<template>
    <div>
        <div id="page">
            <nav class="fh5co-nav" role="navigation">
                <!-- <div class="top-menu"> -->
                <div class="container">
                    <div class="row">
                         <div class="col-xs-12 text-center logo-wrap">
                            <div id="fh5co-logo"><a href="index.html">{{ company.companyName }}<span>.</span></a></div>
                        </div>
                        <div class="col-xs-12 text-center menu-1 menu-wrap">
                            <ul>
                                <li class="active"><a href="menu.html">Menu</a></li>
                                <!--                <li class="has-dropdown">-->
                                <!--                  <a href="gallery.html">Gallery</a>-->
                                <!--                  <ul class="dropdown">-->
                                <!--                    <li><a href="#">Events</a></li>-->
                                <!--                    <li><a href="#">Food</a></li>-->
                                <!--                    <li><a href="#">Coffees</a></li>-->
                                <!--                  </ul>-->
                                <!--                </li>-->
                            </ul>
                        </div>
                    </div>

                </div>
                <!-- </div> -->
            </nav>

            <header id="fh5co-header" class="fh5co-cover js-fullheight" role="banner"
                    style="background-image: url(images/background.jpeg);" data-stellar-background-ratio="0.5">
                <div class="overlay"></div>
                <div class="container">
                    <div class="row">
                        <div class="col-md-12 text-center">
                            <div class="display-t js-fullheight">
                                <div class="display-tc js-fullheight animate-box" data-animate-effect="fadeIn">
                                    <h1>See <em>Our</em> Menu</h1>
                                    <h2>Taste of <a href="http://freehtml5.co/" target="_blank">italian ingredients</a>
                                    </h2>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </header>

            <div id="fh5co-featured-menu" class="fh5co-section">
                <div class="container">
                    <div class="row">
                        <div class="col-md-12 fh5co-heading animate-box mb-9">
                            <h2>Main dishes</h2>
                        </div>
                        <PlateItem v-for="(plate, idx) in company.plates" :key="idx" :item="plate" ></PlateItem>
                    </div>
                </div>
            </div>

            <div id="fh5co-featured-testimony" class="fh5co-section">
                <div class="container">
                    <div class="row">
                        <div class="col-md-12 fh5co-heading animate-box">
                            <h2>Testimony</h2>
                            <div class="row">
                                <div class="col-md-6">
                                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis ab debitis
                                        sit itaque totam, a maiores nihil, nulla magnam porro minima officiis! Doloribus
                                        aliquam voluptates corporis et tempora consequuntur ipsam, itaque, nesciunt
                                        similique commodi omnis.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>


            <div id="fh5co-started" class="fh5co-section animate-box" style="background-image: url(images/hero_1.jpeg);"
                 data-stellar-background-ratio="0.5">
                <div class="overlay"></div>
                <div class="container">
                    <div class="row animate-box">
                        <div class="col-md-8 col-md-offset-2 text-center fh5co-heading">
                            <h2>Book a Table</h2>
                            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae enim quae vitae
                                cupiditate, sequi quam ea id dolor reiciendis consectetur repudiandae. Rem quam,
                                repellendus veniam ipsa fuga maxime odio? Eaque!</p>
                            <p><a href="reservation.html" class="btn btn-primary btn-outline">Book Now</a></p>
                        </div>
                    </div>
                </div>
            </div>

            <footer id="fh5co-footer" role="contentinfo" class="fh5co-section">
                <div class="container">
                    <div class="row row-pb-md">
                        <div class="col-md-4 fh5co-widget">
                            <h4>Tasty</h4>
                            <p>Facilis ipsum reprehenderit nemo molestias. Aut cum mollitia reprehenderit. Eos cumque
                                dicta adipisci architecto culpa amet.</p>
                        </div>
                        <div class="col-md-2 col-md-push-1 fh5co-widget">
                            <h4>Links</h4>
                            <ul class="fh5co-footer-links">
                                <li><a href="#">Home</a></li>
                                <li><a href="#">Portfolio</a></li>
                                <li><a href="#">Blog</a></li>
                                <li><a href="#">About</a></li>
                            </ul>
                        </div>

                        <div class="col-md-2 col-md-push-1 fh5co-widget">
                            <h4>Categories</h4>
                            <ul class="fh5co-footer-links">
                                <li><a href="#">Landing Page</a></li>
                                <li><a href="#">Real Estate</a></li>
                                <li><a href="#">Personal</a></li>
                                <li><a href="#">Business</a></li>
                                <li><a href="#">e-Commerce</a></li>
                            </ul>
                        </div>

                        <div class="col-md-4 col-md-push-1 fh5co-widget">
                            <h4>Contact Information</h4>
                            <ul class="fh5co-footer-links">
                                <li>198 West 21th Street, <br> Suite 721 New York NY 10016</li>
                                <li><a href="tel://1234567920">+ 1235 2355 98</a></li>
                                <li><a href="mailto:info@yoursite.com">info@yoursite.com</a></li>
                                <li><a href="http://https://freehtml5.co">freehtml5.co</a></li>
                            </ul>
                        </div>

                    </div>

                    <div class="row copyright">
                        <div class="col-md-12 text-center">
                            <p>
                                <small class="block">&copy; 2016 Free HTML5. All Rights Reserved.</small>
                                <small class="block">Designed by <a href="http://freehtml5.co/" target="_blank">FreeHTML5.co</a>
                                    Demo Images: <a href="http://unsplash.co/" target="_blank">Unsplash</a></small>
                            </p>
                            <p>
                            <ul class="fh5co-social-icons">
                                <li><a href="#"><i class="icon-twitter2"></i></a></li>
                                <li><a href="#"><i class="icon-facebook2"></i></a></li>
                                <li><a href="#"><i class="icon-linkedin2"></i></a></li>
                                <li><a href="#"><i class="icon-dribbble2"></i></a></li>
                            </ul>
                            </p>
                        </div>
                    </div>

                </div>
            </footer>
        </div>
    </div>
</template>

<script>
import PlateItem from "@/components/plate-view.vue";


export default {
    name: 'App',
    components: {
        PlateItem
    },
    data() {
        return {
            company: defaultCompany()
        }
    },
    mounted() {
        this.loadCompany();
    },
    methods: {
        loadCompany() {
            fetch("localhost:8080/fake")
                .then(response => {
                    console.log(response);
                })
                .catch(error => {
                    console.log(error);
                    this.company = defaultCompany();
                })
        },
    }
}

function defaultPlates() {
    return [
        {
            id: 1,
            image: "images/pizza.jpeg",
            title: 'Margarita',
            subtitle: 'Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza',
            model3D: '',
        },
        {
            id: 2,
            image: 'burger.png',
            title: 'Max burger',
            subtitle: 'Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza',
            model3D: '',
        },
        {
            id: 3,
            image: 'burger.png',
            title: 'Max burger',
            subtitle: 'Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza',
            model3D: '',
        },
        {
            id: 4,
            image: 'beer.png',
            title: 'Beer',
            subtitle: 'Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza',
            model3D: '',
        }
    ]
}

function defaultCompany(){
    return {
        companyName: "Italian restaurant",
        plates: defaultPlates()
    }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
}

h1 {
    font-family: Montserrat;
    font-size: 60px;
    color: whitesmoke;
}

p {
    font-family: Cinzel;
    font-size: 28px;
    color: whitesmoke;
}
</style>
