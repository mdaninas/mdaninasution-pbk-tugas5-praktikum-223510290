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
</template>

<style scoped>
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
    width: 1857px;
    background-color: black;
}

.rowhp::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
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
