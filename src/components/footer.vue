<script>

export default {

}

</script>

<template>
    <div class="bg-footer">
        <div class="container d-flex">
            <img src="/img/dc-logo-bg.png" class="logo-bg" alt="">
            <div class="w-10">
                <h4>DC COMICS</h4>
                <ul>
                    <li>
                        characters
                    </li>
                    <li>
                        comics
                    </li>
                    <li>
                        movies
                    </li>
                    <li>
                        tv
                    </li>
                    <li>
                        games
                    </li>
                    <li>
                        videos
                    </li>
                    <li>
                        news
                    </li>
                </ul>
                <h4 class="mt-2">Shop</h4>
                <ul>
                    <li>
                        Shop DC
                    </li>
                    <li>
                        Shop DC Collectibles
                    </li>
                </ul>
            </div>
            <div class="w-10">
                <h4>DC</h4>
                <ul>
                    <li>
                        characters
                    </li>
                    <li>
                        comics
                    </li>
                    <li>
                        movies
                    </li>
                    <li>
                        tv
                    </li>
                    <li>
                        games
                    </li>
                    <li>
                        videos
                    </li>
                    <li>
                        news
                    </li>
                    <li>
                        news
                    </li>
                    <li>
                        news
                    </li>
                    <li>
                        news
                    </li>
                    <li>
                        news
                    </li>
                </ul>
            </div>
            <div class="w-10">
                <h4>SITES</h4>
                <ul>
                    <li>
                        characters
                    </li>
                    <li>
                        comics
                    </li>
                    <li>
                        movies
                    </li>
                    <li>
                        tv
                    </li>
                    <li>
                        games
                    </li>
                    <li>
                        videos
                    </li>
                    <li>
                        news
                    </li>
                </ul>
            </div>
        </div>
    </div>
    <div class="bar-footer">
        <div class="container d-flex ">
            <div class="w-20">
                <button>
                    sign-up now
                </button>
            </div>
            <div class="w-80 justify-content-end d-flex align-items-center">
                <h4>follow us</h4>
                <img src="/img/footer-facebook.png" alt="">
                <img src="/img/footer-twitter.png" alt="">
                <img src="/img/footer-youtube.png" alt="">
                <img src="/img/footer-pinterest.png" alt="">
                <img src="/img/footer-periscope.png" alt="">
                <div>

                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.bg-footer {
    background-image: url('/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;



    .container {
        color: white;
        position: relative;

        .logo-bg {
            position: absolute;
            top: -60px;
            right: 20px;
            width: 30%;
            z-index: 1;
        }

        .w-10 {

            h4 {
                text-transform: uppercase;
                margin-bottom: 0.5em;
            }

            ul {
                list-style: none;

                li {
                    color: #545555;
                }
            }
        }
    }
}

.bar-footer {
    width: 100%;
    background-color: #313131;

    button {
        border: 1px solid #0379f1;
        background-color: transparent;
        color: white;
        padding: 0.5em 1em;
        text-transform: uppercase;
        font-weight: bold;
    }

    .w-80 {
        h4 {
            color: #0379f1;
            text-transform: uppercase;
            font-size: 0.8em;
        }

        img {
            width: 25px;
            margin-left: 1em;
        }

    }
}
</style>
