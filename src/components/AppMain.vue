<script>
import Blogs from '../data/blogs.json'
import cardsBlog from './cardsBlog.vue';
import courses from '../data/courses.json'
import cardsCourses from './cardsCourses.vue';
export default {
    components: {
        cardsBlog,
        cardsCourses
    },
    data () {
        return {
            Blogs,
            courses
        }
    }
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

        <div class="bg-col-5">

            <!-- learn about section -->
            <section class="padding-jumbo">
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
                        <div class="col-8 offset-2 p-4 stats">
                            <ul class="list-unstyled d-flex justify-content-around">
                                <li>
                                    <strong class="color-2 d-flex justify-content-center font-11">129+</strong>
                                    <p>ENROLLED LEANERS</p>
                                </li>
                                <li>
                                    <strong class="color-2 d-flex justify-content-center font-11">80</strong>
                                    <p>ENROLLED LEANERS</p>
                                </li>
                                <li>
                                    <strong class="color-2 d-flex justify-content-center font-11">4%</strong>
                                    <p>ENROLLED LEANERS</p>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </section>
    
            <!-- upgrade your skill section -->
            <section class="mt-5">
                <div class="container">
                    <div class="row g-0">
                        <div class="col-7 position-relative skills">
                            <img src="../assets/img/stock-full-hd-11-670x450.jpg" alt="">
                            <img src="../assets/img/maxcoach-shape-07.png" alt="">
                            <img src="../assets/img/maxcoach-shape-05.png" alt="">
                            <img src="../assets/img/icon-youtube-play.png" alt="">
                            <svg xmlns="http://www.w3.org/2000/svg" width="200" height="202"><path class="elementor-shape-fill" d="M139.374 198.088c16.328 8.906 51.35-1.087 58.304-39.038 7.15-39.022-13.182-40.052-9.633-54.248 14.243-21.15 16.782-48.14 2.028-64.387-36.503-38.024-45.629 7.604-76.048-20.28C101.727 7.837 83.1-6.735 56.23 3.405 18.239 17.74 27.33 47.659 27.33 69.313c0 7.624-24.216 21.957-26.87 41.573-3.346 24.734 12.168 57.29 26.87 68.443 23.322 26.363 59.318 20.28 75.541 11.154 13.931-7.836 25.35 1.52 36.503 7.605z"/></svg>
                        </div>
                        <div class="col-5 d-flex flex-column justify-content-center">
                            <h6>HOW WE WORK</h6>
                            <strong class="font-11">Upgrade Your <br> Skills <span class="color-2 no-bold">Upgrade <br> Your Life</span></strong>
                            <p>Opening up more opportunities in front of you to get the ticket to more enjoyable door in life. Getting equipped with new skills for new sets of insights into your career. <br> MaxCoach accompany learners in every stage of learning.</p>
                            <a href="#" class="text-decoration-none text-black"><strong>Download free guidebook &#8594;</strong></a>
                        </div>
                    </div>
                </div>
            </section>
    
            <!-- latest online courses section -->
            <section>
                <div class="container padding-jumbo online-courses">
                    <div class="row">
                        <div class="col-12 text-center">
                            <h6>JOIN MAXCOACH AT BEST</h6>
                            <strong class="font-11">Latest Online <span class="color-2 no-bold">Courses</span></strong>
                        </div>
                    </div>
                    <div class="row mt-5">
                        <cardsCourses 
                            v-for="(card, index) in courses"
                            :key="index"
                            :img="card.img"
                            :price="card.price"
                            :title="card.title"
                            :lessons="card.lessons"
                            :students="card.students"
                        />
                    </div>
                    <div class="row mt-5">
                        <div class="col-12">
                            <div class="content"></div>
                        </div>
                    </div>
                </div>
            </section>
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none" height="100"><path class="elementor-shape-fill" d="M0 0v100h100V0Q50 200 0 0"/></svg>
        </div>

        <div class="bg-col-6">

            <!-- Testimonials section -->
            <section class="testimonials">
                <div class="container mt-5">
                    <div class="row g-0 position-relative">
                        <div class="col-5">
                            <h6>TESTIMONIALS</h6>
                            <strong class="font-11">Why Do People <br> <span class="color-2 no-bold">*Hearts*</span> Us?</strong>
                            <p>seeking for verbals of our service quality? Find them here. Everything is transparent and straightforward for your sense of justification.</p>
                            <a href="#" class="text-decoration-none text-black"><strong>View all &#8594;</strong></a>
                        </div>
                        <div class="col-7 behind-text p-5">
                            <h4>Professional team of specialists anmd passionate mentors at reach</h4>
                            <p class="fs-5">i need to get a certification for english proficiency and MaxCoach is my best choice. their tutors are smart and professional when dealing with students.</p>
                            <div class="d-flex pt-5">
                                <img src="../assets/img/testimonial-avata-01.jpg" alt="" class="rounded-circle">
                                <div class="pt-3 ps-4">
                                    <h6>MADLEY PONDOR</h6>
                                    <p>/IT Specialist</p>
                                </div>
                            </div>
                        </div>
                        <div class="col-7 behind-index p-5">
                            <h4 class="font-4">The MaxCoach team works really hard to ensure high level of quality </h4>
                            <p class="fs-5">i am happy with their arrangement of lessons and subjects. they Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis rem sit magni libero voluptatum voluptatem exercitationem unde amet fuga! Minus, vero fugiat eius consequuntur autem error commodi deserunt nisi pariatur. Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil, placeat velit. Error amet atque qui incidunt fugit nostrum culpa minus, nihil molestias, labore, est consequatur vel accusantium blanditiis aspernatur aperiam? Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ad, odio est, quaerat quisquam praesentium magnam totam perferendis sint optio vitae laborum labore repellendus</p>
                            <div class="d-flex pt-5">
                                <img src="../assets/img/testimonial-avata-02.jpg" alt="" class="rounded-circle">
                                <div class="pt-3 ps-4">
                                    <h6>MINA HOLLACE</h6>
                                    <p>/Freelancer</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
    
            <!-- here to transform you section -->
            <section>
                <div class="container transform">
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
        </div>

        <!-- latest from our blogs section -->
        <section>
            <div class="container mt-5">
                <div class="row">
                    <div class="col-12 text-center">
                        <h6 class="font-2">READ FOR MORE JOYMENT</h6>
                        <strong class="font-11">Latest from <span class="color-2 no-bold">Our Blogs</span></strong>
                    </div>
                </div>
                <div class="row mt-5">
                    <cardsBlog 
                        v-for="(card, index) in Blogs"
                        :key="index"
                        :img="card.img"
                        :profession="card.profession"
                        :title="card.title"
                        :date="card.date"
                        :views="card.views"
                    />
                </div>
            </div>
        </section>

        <!-- news letter section -->
        <section class="margin-y-1">
            <div class="container">
                <div class="row mt-5">
                    <div class="col-12 d-flex align-items-center flex-column text-center position-relative letter">
                        <strong class="font-11">Subscribe <span class="color-2 no-bold">Newsletters</span></strong>
                        <p>enter your email address to register to uor newsletter subscription <br> delivered on a regular basis</p>
                        <div>
                            <form class="d-flex">
                                <input class="form-control rounded-end-0 border-0 color-6 py-2" type="search" placeholder="Enter your email" aria-label="Search">
                                <button class="btn bg-col-2 text-white rounded-start-0 border-start-0 rounded-end px-3" type="submit">Subscribe</button>
                            </form>
                        </div>
                        <img src="../assets/img/maxcoach-shape-02.png" alt="">
                        <img src="../assets/img/maxcoach-shape-09.png" alt="">
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

    .padding-jumbo {
        padding-top: 180px;
    }

    .stats {
        margin-top: 100px;
    }

    .skills {
        img:nth-child(1) {
            border-radius: 5px;
        }
        img:nth-child(2) {
            position: absolute;
            bottom: -6rem;
            right: 4rem;
            z-index: -1;
        }
        img:nth-child(3) {
            position: absolute;
            top: 3rem;
            left: -7rem;
            z-index: -1;
        }
        img:nth-child(4) {
            position: absolute;
            top: 12rem;
            left: 18rem;
        }
        svg {
            position: absolute;
            top: -5rem;
            left: -6rem;
            z-index: -5;
            width: 100%;
            margin-top: -1px;
        }
        .elementor-shape-fill {
        fill: #eeeeee; 
        }
    }

    .letter {
        form {
            input {
                width: 500px;
            }
        }
        img:nth-of-type(1) {
            position: absolute;
            top: 2rem;
            right: 7rem;
        }
        img:nth-of-type(2) {
            position: absolute;
            top: -5rem;
            right: 7rem;
        }
    }

    .testimonials {
        margin-top: 300px;
    }

    .behind-text {
        box-shadow: 0 0px 40px rgba(0, 0, 0, 0.151);
        background-color: #fff;
        img {
            width: 80px;
        }
    }
    .behind-index {
        box-shadow: 0 0 40px rgba(0, 0, 0, 0.151);
        position: absolute;
        top: -10rem;
        right: 5rem;
        z-index: -5;
        max-width: 600px;
        background-color: #fff;
        opacity: 0.5;
        img {
            width: 80px;
        }
    }

    .transform {
        margin-top: 300px;
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

    svg {
        display: block;
        width: 100%;
        margin-top: -1px;
    }
    .elementor-shape-fill {
        fill: #fff; 
    }

    .color-2 {
        color: $color-2;
    }
    .color-6 {
        background-color: $color-6;
    }

    .bg-col-2 {
        background-color: $color-2;
    }
    .bg-col-5 {
        background-color: $color-5;
        position: relative;
        z-index: -10;
    }

    .font-1 {
        font-size: $font-1;
    }

    .font-2 {
        font-size: $font-2;
    }
    .font-3 {
        font-size: $font-3;
    }

    .font-11 {
        font-size: $font-11;
    }

    .font-10 {
        font-size: $font-10;
    }

    .margin-y-1 {
        margin: 100px 0;
    }
</style>