<template>
    <div class="pricing5 py-5"  v-show="annually">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-md-8 text-center">
                    <!-- <h3 class="mb-3">{{title}}</h3> -->
                    <!-- <div class="switcher-box mt-4">
                        <div class="btn-group rounded-pill" data-toggle="buttons">
                            <label class="btn btn-outline-secondary btn-md active rounded-left">
                                <input type="radio" name="options" id="option1" checked @click="monthly"> Monthly
                            </label>
                            <label class="btn btn-outline-secondary rounded-right btn-md">
                                <input type="radio" name="options" id="option2" @click="annually"> Annually
                            </label>
                            <Monthly v-show="monthly" />
                            <Annually v-show="annually" />
                        </div>
                    </div> -->
                </div>
            </div>
            <div class="row text-center pricing-box">
                <div class="col-md-4">
                    <div class="card card-shadow border-0 mb-4"
                        style="background:url(https://www.wrappixel.com/demos/ui-kit/wrapkit/assets/images/pricing/p5-img1.jpg)no-repeat">
                        <div class="card-body">
                            <h6 class="text-white mt-3 mb-0">{{titreannually1}}</h6>
                            <h2 class="text-white mt-0 yearly">{{priceyear1}}</h2>
                            <ul class="general-listing">
                                <li class="py-3 d-block">
                                    <h6 class="subtitle font-weight-normal">{{stockageyear1}}</h6>
                                </li>
                                <li class="py-3 d-block">
                                    <h6 class="subtitle font-weight-normal">{{videoyear1}}</h6>
                                </li>
                                <li class="py-3 d-block">
                                    <h6 class="subtitle font-weight-normal">{{sendyear1}}</h6>
                                </li>
                            </ul>
                            <a class="btn btn-outline-success btn-md rounded-pill mb-3"
                                href="#f1"><span>{{button}}</span></a>
                        </div>
                    </div>
                </div>
                <div class="col-md-4 middle-box">
                    <div class="card card-shadow border-0 mb-4"
                        style="background:url(https://www.wrappixel.com/demos/ui-kit/wrapkit/assets/images/pricing/p5-img2.jpg)no-repeat">
                        <div class="card-body">
                            <h6 class="text-white mt-3 mb-0">{{titreyear2}}</h6>
                            <h2 class="text-white mt-0 yearly">{{priceyear2}}</h2>
                            <div class="star-plan mt-3"><img
                                    src="https://www.wrappixel.com/demos/ui-kit/wrapkit/assets/images/pricing/star.png"
                                    alt="wrapkit" />
                            </div>
                            <ul class="general-listing">
                                <li class="py-3 d-block">
                                    <h6 class="subtitle font-weight-normal">{{stockageyear2}}</h6>
                                </li>
                                <li class="py-3 d-block">
                                    <h6 class="subtitle font-weight-normal">{{videoyear2}}</h6>
                                </li>
                                <li class="py-3 d-block">
                                    <h6 class="subtitle font-weight-normal">{{sendyear2}}</h6>
                                </li>
                            </ul>
                            <a class="btn btn-success-gradiant btn-md text-white rounded-pill mb-3"
                                href="#f1"><span>{{button}}</span></a>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card card-shadow border-0 mb-4"
                        style="background:url(https://www.wrappixel.com/demos/ui-kit/wrapkit/assets/images/pricing/p5-img3.jpg)no-repeat">
                        <div class="card-body">
                            <h6 class="text-white mt-3 mb-0">{{titreyear3}}</h6>
                            <h2 class="text-white mt-0 yearly">{{priceyear3}}</h2>
                            <ul class="general-listing">
                                <li class="d-block py-3">
                                    <h6 class="subtitle font-weight-normal">{{stockageyear3}}</h6>
                                </li>
                                <li class="d-block py-3">
                                    <h6 class="subtitle font-weight-normal">{{videoyear3}}</h6>
                                </li>
                                <li class="d-block py-3">
                                    <h6 class="subtitle font-weight-normal">{{sendyear3}}</h6>
                                </li>
                            </ul>
                            <a class="btn btn-outline-success btn-md rounded-pill mb-3"
                                href="#f1"><span>{{button}}</span></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    // import Annually from './components/Annually.vue'
    // import Monthly from './components/Monthly.vue'
    export default {
        name: 'App',
        // components: {
        //     Annually,
        //     Monthly,
        // },
        // props: {
        //     titreannually1: String,
        //     titreannually2: String,
        //     titreannually3: String,
        //     priceyear1: String,
        //     priceyear2: String,
        //     priceyear3: String,
        //     stockageyear1: String,
        //     stockageyear2: String,
        //     stockageyear3: String,
        //     videoyear1: String,
        //     videoyear2: String,
        //     videoyear3: String,
        //     sendyear1: String,
        //     sendyear2: String,
        //     sendyear3: String,
        //     titremonthly1: String,
        //     titremonthly2: String,
        //     titremonthly3: String,
        //     pricemonth1: String,
        //     pricemonth2: String,
        //     pricemonth3: String,
        //     stockagemonth1: String,
        //     stockagemonth2: String,
        //     stockagemonth3: String,
        //     videomonth1: String,
        //     videomonth2: String,
        //     videomonth3: String,
        //     sendmonth1: String,
        //     sendmonth2: String,
        //     sendmonth3: String,
        //     button: String,

        // },
        methods: {
            month() {
                this.month = !this.month;
                this.year = !this.year;
            },
            annual() {
                this.month = !this.month;
                this.year = !this.year;
            }
        }
    }
</script>

<style>
    .pricing5 {
        font-family: "Montserrat", sans-serif;
        color: #8d97ad;
        font-weight: 300;
    }

    .pricing5 h1,
    .pricing5 h2,
    .pricing5 h3,
    .pricing5 h4,
    .pricing5 h5,
    .pricing5 h6 {
        color: #3e4555;
    }

    .pricing5 h5 {
        line-height: 22px;
        font-size: 18px;
    }

    .pricing5 .font-weight-medium {
        font-weight: 500;
    }

    .pricing5 .bg-light {
        background-color: #f4f8fa !important;
    }

    .pricing5 .subtitle {
        color: #8d97ad;
        line-height: 24px;
    }

    .pricing5 .card.card-shadow {
        -webkit-box-shadow: 0px 0px 30px rgba(115, 128, 157, 0.1);
        box-shadow: 0px 0px 30px rgba(115, 128, 157, 0.1);
    }

    .pricing5 .general-listing {
        margin: 90px 0 60px 0;
    }

    .pricing5 .card {
        background-size: 100% !important;
    }


    .pricing5 .pricing-box {
        margin-top: 120px;
    }

    .pricing5 .pricing-box .middle-box {
        margin-top: -75px;
    }

    .pricing5 .pricing-box .middle-box .general-listing {
        margin-top: 60px;
    }

    @media (max-width: 767px) {
        .pricing5 .pricing-box {
            margin-top: 40px;
        }

        .pricing5 .pricing-box .middle-box {
            margin-top: 0px;
        }
    }

    .pricing5 .btn-success-gradiant {
        background: #be8ff8;
        background: -webkit-linear-gradient(legacy-direction(to right), #2cdd9b 0%, #1dc8cc 100%);
        background: -webkit-gradient(linear, left top, right top, from(#2cdd9b), to(#1dc8cc));
        background: -webkit-linear-gradient(left, #2cdd9b 0%, #1dc8cc 100%);
        background: -o-linear-gradient(left, #2cdd9b 0%, #1dc8cc 100%);
        background: linear-gradient(to right, #2cdd9b 0%, #1dc8cc 100%);
    }

    .pricing5 .btn-success-gradiant:hover {
        background: #1dc8cc;
        background: -webkit-linear-gradient(legacy-direction(to right), #1dc8cc 0%, #2cdd9b 100%);
        background: -webkit-gradient(linear, left top, right top, from(#1dc8cc), to(#2cdd9b));
        background: -webkit-linear-gradient(left, #1dc8cc 0%, #2cdd9b 100%);
        background: -o-linear-gradient(left, #1dc8cc 0%, #2cdd9b 100%);
        background: linear-gradient(to right, #1dc8cc 0%, #2cdd9b 100%);
    }

    .pricing5 .btn-md {
        padding: 15px 45px;
        font-size: 16px;
    }

    .pricing5 .rounded-left {
        border-top-left-radius: 60px !important;
        border-bottom-left-radius: 60px !important;
    }

    .pricing5 .rounded-right {
        border-top-right-radius: 60px !important;
        border-bottom-right-radius: 60px !important;
    }

    .pricing5 .btn-outline-success {
        color: #2cdd9b;
        background-color: transparent;
        border-color: #2cdd9b;
    }

    .pricing5 .btn-outline-success:hover {
        background: #2cdd9b;
        border-color: #2cdd9b;
        color: #ffffff;
    }
</style>