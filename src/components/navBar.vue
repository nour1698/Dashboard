<template>
<div>
    <nav class="navbar navbar-expand-lg navbar-light">
        <div class="container-fluid " style="height:30px">
            <a href="#">
                <img class="logo" src="/logo.png"/>
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarScroll">
                <ul class="navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll" style="--bs-scroll-height: 100px;">
                    <li class="nav-item">
                        <a class="nav-link active"  aria-current="page" href="#">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">My TODO</a>
                    </li>
                    
                    <!-- <li class="nav-item dropdown">
                        <a class="nav-link dropdown-toggle" href="#" id="navbarScrollingDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                            Link
                        </a>
                        <ul class="dropdown-menu" aria-labelledby="navbarScrollingDropdown">
                            <li><a class="dropdown-item" href="#">Action</a></li>
                            <li><a class="dropdown-item" href="#">Another action</a></li>
                            <li>
                                <hr class="dropdown-divider">
                            </li>
                            <li><a class="dropdown-item" href="#">Something else here</a></li>
                        </ul>
                    </li> -->
                    <li class="nav-item">
                        <a class="nav-link" href="#" tabindex="-1" aria-disabled="true">My Application</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Pre-warning</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Issue</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</div>
</template>
<style scoped>
.logo{
    width:90px;
    height: 90px;
}
</style>
