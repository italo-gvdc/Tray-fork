
<template>

<header id="header" class="fixed-top d-flex align-items-center">
    <div class="container">
        <div class="header-container d-flex align-items-center justify-content-between">
            <div class="logo">
                <h1 class="logo-text">
                    SneakerWorld
                </h1>
            </div>
        </div>

        <nav id="navbar" class="navbar d-flex align-items-center">
            <ul class="d-flex list-unstyled mb-0">
                <li class="mx-3">
                    <a class="nav-link highlight" href="/cad">
                        Cadastre-se
                    </a>
                </li>
                <li class="mx-3">
                    <a class="nav-link highlight" href="/com">
                        Compra
                    </a>
                </li>
                <li class="mx-3">
                    <a class="nav-link" href="/">
                        Home
                    </a>
                </li>
            </ul>
            <i class="bi bi-list mobile-nav-toggle" style="font-size: 1.5rem; color: #333; cursor: pointer;"></i>
        </nav>
    </div>
</header>



    
<section id="hero" class="d-flex align-items-center justify-content-center position-relative" style="height: 100vh; overflow: hidden;">
    <img src="../assets/tenisnovo.jpg" alt="Imagem" class="img-fluid position-absolute w-100 h-100" style="object-fit: cover; z-index: -1;">
    
    <div class="overlay" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0, 0, 0, 0.5);"></div>
    
    <div class="container text-center position-relative" data-aos="fade-in" data-aos-delay="200" style="z-index: 1;">
        <h1 style="font-size: 3.5rem; font-weight: bold; color: white; text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.7);">Sua Loja Online de Tênis</h1>
        <h2 style="font-size: 2rem; font-weight: 300; color: white; margin-bottom: 30px; text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.7);">Experiência de compra incrível</h2>
        <a href="/com" class="btn btn-primary btn-lg" style="font-size: 1.5rem; padding: 15px 30px; border-radius: 50px; background-color: #ff4500; border: none;">Explore os Produtos</a>
    </div>
</section>



<section id="clients" class="fixed-bottom d-flex" style="background-color: white; padding-top: 5px !important; padding-bottom: 5px !important;">
    <div class="container">
    <div class="row">
        <div class="col-lg-2 col-md-4 col-6 d-flex align-items-center" data-aos="zoom-in" data-aos-delay="100">
            <a href="/com?brand=Adidas">
                <img src="../assets/client-1.png" class="img-fluid" alt="Imagem">
            </a>
        </div>

        <div class="col-lg-2 col-md-4 col-6 d-flex align-items-center" data-aos="zoom-in" data-aos-delay="200">
            <a href="/com?brand=Nike">
                <img src="../assets/client-2.png" class="img-fluid" alt="Imagem">
            </a>
        </div>

        <div class="col-lg-2 col-md-4 col-6 d-flex align-items-center" data-aos="zoom-in" data-aos-delay="300">
            <a href="/com?brand=Lacoste">
                <img src="../assets/client-3.png" class="img-fluid" alt="Imagem">
            </a>
        </div>

        <div class="col-lg-2 col-md-4 col-6 d-flex align-items-center" data-aos="zoom-in" data-aos-delay="400">
            <a href="/com?brand=Puma">
                <img src="../assets/client-4.png" class="img-fluid" alt="Imagem">
            </a>
        </div>

        <div class="col-lg-2 col-md-4 col-6 d-flex align-items-center" data-aos="zoom-in" data-aos-delay="500">
            <a href="/com?brand=NB">
                <img src="../assets/client-5.png" class="img-fluid" alt="Imagem">
            </a>
        </div>

        <div class="col-lg-2 col-md-4 col-6 d-flex align-items-center" data-aos="zoom-in" data-aos-delay="600">
            <a href="/com?brand=Vans">
                <img src="../assets/client-6.png" class="img-fluid" alt="Imagem">
            </a>
        </div>
    </div>
</div>
</section>



<a href="#" class="back-to-top d-flex align-items-center justify-content-center"><i class="bi bi-arrow-up-short"></i></a>
</template>

<script>
    export default {
        methods: {
            closeWelcomeDiv() {
                document.getElementById('welcome-div').style.display = "none"
            }
        }
    }
</script>

<style>

/* Logo styling */
.logo-text {
    font-family: 'Roboto', sans-serif;
    font-size: 2.5rem;
    font-weight: 600;
    color: #333;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    margin: 0;
}

/* Navbar styling */
#navbar {
    background-color: transparent;
}

.nav-link {
    font-family: 'Roboto', sans-serif;
    font-size: 1rem;
    color: #333;
    text-transform: uppercase;
    letter-spacing: 1px;
    font-weight: 500;
    text-decoration: none; /* Remove underline */
}

.nav-link:hover {
    color: #ff6600; /* Cor de destaque ao passar o mouse */
}

.highlight {
    color: #ff6600; /* Destaque para links importantes */
}

/* Container styling */
.header-container {
    background-color: #f4f4f4;
    padding: 15px 0;
}

/* Mobile menu icon */
.mobile-nav-toggle {
    font-size: 1.5rem;
    color: #333;
    cursor: pointer;
}

/* Spacing for nav items */
ul.d-flex.list-unstyled.mb-0 li {
    margin: 0 15px; /* Espaçamento horizontal entre os itens */
}



</style>