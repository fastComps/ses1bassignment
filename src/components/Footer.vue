<template>
    <footer class="row">
        <nav class="navbar navbar-toggleable-md navbar-light">
            <ul class="nav">
                <router-link :to="{ name: 'homeLink' }" tag="li"><a class="nav-link">Home</a></router-link>
                <router-link :to="{ name: 'aboutLink' }" tag="li"><a class="nav-link">About</a></router-link>
                <router-link :to="{ name: 'adminLink' }" tag="li"><a class="nav-link">Login</a></router-link>
            </ul>
        </nav>
    </footer>
</template>

<style>
    a {
        color: grey;
    }
    a:hover {
        color: black;
    }
</style>