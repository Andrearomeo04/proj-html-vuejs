<script>
export default {
    
}
</script>

<template>
    <div>
        <!-- jumbo section -->
        <section>
            <div class="jumbo p-5 d-flex justify-content-center align-items-center">
                <div class="container">
                    <div class="row">
                        <div class="col-12 d-flex align-items-center flex-column text-white">
                            <h2>Commence Business</h2>
                            <h1 class="pb-4 font-10">Distant Mentoring Program</h1>
                            <strong class="bg-white color-2 rounded px-5 py-3">Download free guidebook &#8594;</strong>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- learn about section -->
        <section class="margin-jumbo">
            <div class="container">
                <div class="row g-0">
                    <div class="col-4">
                        <h6>EVERYTHING IN MAXCOACH</h6>
                        <strong class="font-11">Learn About our <span class="color-2 fw-normal">Work Culture</span> at MaxCoach</strong>
                        <p class="pb-4 pt-2">spend some time to visit our website or head office and discover our current courses, enrollment procedure, and registration deadline. We're opening new classes every beginning of each month.</p>
                        <p>Have questions? <strong class="color-2">Get Free Guide &#8594;</strong></p>        
                    </div>
                    <div class="col-8 position-relative d-flex justify-content-end">
                        <img src="../assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="stock-full-hd-10">
                        <img src="../assets/img/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="">
                        <img src="../assets/img/maxcoach-shape-02.png" alt="">
                        <img src="../assets/img/maxcoach-shape-07.png" alt="">
                    </div>
                </div>
                <div class="row g-0">
                    <div class="col-6 offset-3 p-4">
                        <div class="content"></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- upgrade your skill section -->
        <section>
            <div class="container">
                <div class="row g-0">
                    <div class="col-7">
                        <div class="content"></div>
                    </div>
                    <div class="col-5">
                        <div class="content"></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- latest online courses section -->
        <section>
            <div class="container mt-5">
                <div class="row">
                    <div class="col-12">
                        <div class="content"></div>
                    </div>
                </div>
                <div class="row mt-5">
                    <div class="col-4">
                        <div class="content"></div>
                    </div>
                    <div class="col-4">
                        <div class="content"></div>
                    </div>
                    <div class="col-4">
                        <div class="content"></div>
                    </div>
                </div>
                <div class="row mt-5">
                    <div class="col-12">
                        <div class="content"></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Testimonials section -->
        <section>
            <div class="container mt-5">
                <div class="row g-0">
                    <div class="col-5">
                        <div class="content"></div>
                    </div>
                    <div class="col-7">
                        <div class="content"></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- here to transform you section -->
        <section>
            <div class="container mt-5">
                <div class="row g-0">
                    <div class="col-7">
                        <div class="content"></div>
                    </div>
                    <div class="col-5">
                        <div class="content"></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- latest from our blogs section -->
        <section>
            <div class="container mt-5">
                <div class="row">
                    <div class="col-12">
                        <div class="content"></div>
                    </div>
                </div>
                <div class="row mt-5">
                    <div class="col-4">
                        <div class="content"></div>
                    </div>
                    <div class="col-4">
                        <div class="content"></div>
                    </div>
                    <div class="col-4">
                        <div class="content"></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- news letter section -->
        <section>
            <div class="container">
                <div class="row mt-5">
                    <div class="col-12">
                        <div class="content"></div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.content {
        width: 100%;
        height: 60px;
        background-color: blueviolet;
        border: 1px solid black;
    }

    .jumbo {
        background-image: url(../assets/img/home-3-hero-bg.jpg);
        background-size: cover;
        min-height: 650px;
    }

    .margin-jumbo {
        margin-top: 180px;
    }

    .col-8 {
        img:nth-child(2) {
            position: absolute;
            top: -5rem;
            right: -5rem;
            border-radius: 5px;
        }
        img:nth-child(3) {
            position: absolute;
            bottom: -5rem;
            right: 5rem;
        }
        img:nth-child(4) {
            position: absolute;
            top: -4rem;
            z-index: -1;
        }
    }

    .color-2 {
        color: $color-2;
    }

    .font-11 {
        font-size: $font-11;
    }

    .font-10 {
        font-size: $font-10;
    }
</style>