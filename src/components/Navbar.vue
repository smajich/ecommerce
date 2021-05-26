<template>
    <div>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">E-commerce</a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav me-auto">
                        <li class="nav-item text-center">
                            <router-link to="/" class="nav-link" aria-current="page">Home</router-link>
                        </li>
                        <li class="nav-item text-center">
                            <router-link to="/" class="nav-link" aria-current="page">Products</router-link>
                        </li>
                        <li class="nav-item text-center">
                            <router-link to="/about" class="nav-link">About</router-link>
                        </li>
                    </ul>
                    <form id="nav-search">
                        <input type="search" placeholder="Search">
                    </form>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
    export default {
        name: 'Navbar',
    }
</script>

<style scoped>
    a {
        color: #69C;
        text-decoration: none;
    }
    a:hover {
        color: #F60;
    }
    h1 {
        font: 1.7em;
        line-height: 110%;
        color: #000;
    }
    p {
        margin: 0 0 20px;
    }


    input {
        outline: none;
    }
    input[type=search] {
        -webkit-appearance: textfield;
        -webkit-box-sizing: content-box;
        font-family: inherit;
        font-size: 100%;
    }
    input::-webkit-search-decoration,
    input::-webkit-search-cancel-button {
        display: none;
    }


    input[type=search] {
        background: #ededed url(https://static.tumblr.com/ftv85bp/MIXmud4tx/search-icon.png) no-repeat 9px center;
        border: none;
        padding: 9px 10px 9px 32px;
        width: 55px;

        -webkit-border-radius: 10em;
        -moz-border-radius: 10em;
        border-radius: 10em;

        -webkit-transition: all .5s;
        -moz-transition: all .5s;
        transition: all .5s;
    }
    input[type=search]:focus {
        width: 130px;
        background-color: #fff;
        outline: none;

    }


    input:-moz-placeholder {
        color: #999;
    }
    input::-webkit-input-placeholder {
        color: #999;
    }

    /* Demo 2 */
    #nav-search input[type=search] {
        width: 15px;
        padding-left: 10px;
        color: transparent;
        cursor: pointer;
        background-color: #f8f9fa;
    }
    #nav-search input[type=search]:hover {
        background-color: #f8f9fa;
    }
    #nav-search input[type=search]:focus {
        width: 130px;
        padding-left: 32px;
        color: #000;
        background-color: #fff;
        cursor: auto;
    }
    #nav-search input:-moz-placeholder {
        color: transparent;
    }
    #nav-search input::-webkit-input-placeholder {
        color: transparent;
    }
</style>
