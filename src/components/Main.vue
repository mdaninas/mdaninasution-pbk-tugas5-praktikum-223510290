<template>
    <div class="row rowhp justify-evenly">
        <h1 class="hptit">Handphone</h1>
    </div>

    <div class="row isi justify-evenly">

        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Samsung</span>
            </div>
            <div class="gambar">
                <img src="../assets/samsung.png" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>OPPO</span>
            </div>
            <div class="gambar">
                <img src="../assets/oppo.png" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Vivo</span>
            </div>
            <div class="gambar">
                <img src="../assets/vivo.jpeg" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
    </div>
    <div class="row rowhp justify-evenly">
        <h1 class="hptit">Laptop</h1>
    </div>
    <div class="row isi justify-evenly">
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Asus</span>
            </div>
            <div class="gambar">
                <img src="../assets/asus.jpg" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Acer</span>
            </div>
            <div class="gambar">
                <img src="../assets/acer.jpg" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Msi</span>
            </div>
            <div class="gambar">
                <img src="../assets/msi.png" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
    </div>
    <div class="row rowhp justify-evenly">
        <h1 class="hptit">Sepatu</h1>
    </div>
    <div class="row isi justify-evenly">
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Adidas</span>
            </div>
            <div class="gambar">
                <img src="../assets/adidas.jpg" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Nike</span>
            </div>
            <div class="gambar">
                <img src="../assets/nike.jpg" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Converse</span>
            </div>
            <div class="gambar">
                <img src="../assets/converse.jpg" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
    </div>
    <div class="row rowhp justify-evenly">
        <h1 class="hptit">Outfit</h1>
    </div>
    <div class="row isi justify-evenly">
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Erigo</span>
            </div>
            <div class="gambar">
                <img src="../assets/erigo.jpg" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>Uniqlo</span>
            </div>
            <div class="gambar">
                <img src="../assets/uniqlo.png" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
        <div class="col-3 border bordiv">
            <div class="h5">
                <span>H&M</span>
            </div>
            <div class="gambar">
                <img src="../assets/h&m.png" alt="">
            </div>
            <div class="button">
                <q-btn round color="deep-orange" icon="shopping_cart" />
            </div>
        </div>
    </div>
    <div class="q-md">
        <q-carousel v-model="slide" transition-prev="slide-right" transition-next="slide-left" animated
            control-color="primary" class="rounded-borders">
            <q-carousel-slide name="style" class="column no-wrap flex-center fothit">
                <div class="q-mt-md text-center">
                    {{ Ori}}
                </div>
            </q-carousel-slide>
            <q-carousel-slide name="tv" class="column no-wrap flex-center fothit">
                <div class="q-mt-md text-center">
                    {{ ongkir}}
                </div>
            </q-carousel-slide>
            <q-carousel-slide name="layers" class="column no-wrap flex-center fothit">
        
                <div class="q-mt-md text-center">
                    {{ sampai }}
                </div>
            </q-carousel-slide>
            <q-carousel-slide name="map" class="column no-wrap flex-center fothit">
                <div class="q-mt-md text-center">
                    {{ Test }}
                </div>
            </q-carousel-slide>
        </q-carousel>
        <div class="row justify-center">
            <q-btn-toggle class="babutton" color="deep-orange" glossy v-model="slide" :options="[
                { label: 1, value: 'style' },
                { label: 2, value: 'tv' },
                { label: 3, value: 'layers' },
                { label: 4, value: 'map' }
            ]" />
        </div>
    </div>

</template>
<script>
import { ref } from 'vue'

export default {
    setup() {
        return {
            slide: ref('style'),
            Ori :"Barang Dijamin Original",
            sampai:"Dijamin Sampai Dalam 7 Hari",
            ongkir :"Free Ongkir Seluruh Indonesia",
            Test : "Lebih dari 1000K Testimoni"
        }
    }
}
</script>
<style scoped>
.babutton{
    display: flex;
    gap: 40px;
    background: rgb(0, 205, 255);
        background: linear-gradient(118deg, rgba(0, 205, 255, 1) 0%, rgba(255, 244, 0, 1) 26%, rgba(0, 249, 255, 1) 76%, rgba(255, 0, 0, 1) 100%);    width: 100%;
    align-items: center;
    justify-content: center;
    padding: 10px;
    border-radius: ;
}
.fothit{
    background-color: black;
    color: aliceblue;
    font-size: 150px;
    font-family: "Oswald", sans-serif;
        font-optical-sizing: auto;
        font-weight: 700;
        font-style: normal;
}
.h5{
    background-color: white;
    width: 100%;
    height: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 10px;
}
.rowhp {
    position: relative;
    color: white;
    width: 100%;
    background-color: black;
}

.rowhp::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    width: 100%;
    background-image: url(../assets/abcde.gif);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: 50% 90%;
    opacity: 0.5;
    z-index: 1;
}

.rowhp>* {
    position: relative;
    z-index: 2;
}


.isi{
    padding: 80px 0;
    background: rgb(0, 205, 255);
        background: linear-gradient(118deg, rgba(0, 205, 255, 1) 0%, rgba(255, 244, 0, 1) 26%, rgba(0, 249, 255, 1) 76%, rgba(255, 0, 0, 1) 100%);
        
}
.border {
    background-color: black;
    height: 400px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    border-radius: 40px;
}
img{
    object-fit: cover;
    height: 100%;
    width: 100%;
    border-radius: 40px;
   
}
.bordiv{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}
.gambar{
    height: 200px;
    width: 300px;
}
.hptit{
    font-family: "Poetsen One", sans-serif;
        font-weight: 400;
        font-style: normal;
}
span{
    font-family: "Oswald", sans-serif;
    font-size: 30px;
        font-optical-sizing: auto;
        font-weight: 600;
        font-style: normal;
}
</style>
