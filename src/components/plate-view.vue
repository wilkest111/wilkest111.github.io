<template>
    <div>
        <div class="col-md-4 col-sm-6 col-xs-6 col-xxs-12 fh5co-item-wrap">
            <div class="fh5co-item animate-box">
                <div style="position:relative;">
                    <a href="/ar.html?model=asset&scale=11"><img :src="item.image" class="fixed-height "
                                                                 :alt="item.alt"></a>
                    <a href="/ar.html?model=asset&scale=11">
                        <button type="button" class="btn btn-primary ar-icon"><i
                                class="fa-solid fa-vr-cardboard  fa-xl "></i></button>
                    </a>
                </div>

                <div class="row">
                    <div class="col-6 col-md-6 col-sm-6">
                        <h3 class="title">{{ item.title }}</h3>
                    </div>
                    <div class="col-6 col-md-6 col-sm-6">
                        <span class="fh5co-price title">$20<sup>.50</sup></span>
                    </div>
                </div>
                <p>{{
                    item.subtitle
                    }}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'PlateItem',
    props: {
        item: {
            required: false,
            default: {
                image: "/images/pizza.jpeg",
                alt: "margarita.png",
                title: "Margarita",
                subtitle: "Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza. Deliciuos margarita pizza",
                price: "20.50",
            }
        },
    },
    data() {
        return {
            img: "burger.png",
        }
    },
    methods: {
        changeText() {
        }
    }
}
</script>

<style>

.ar-icon i {
    color: white;
}

.ar-icon:hover i {
    color: black;
}

.ar-icon {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 65px;
    height: 35px;
    position: absolute;
    bottom: 15px;
    right: 15px;
}

.fixed-height {
    display: block;
    min-height: 280px;
    max-height: 280px;
    min-width: 100%;
    max-width: 100%;
}
.title{
    font-size: 35px;
}
</style>
