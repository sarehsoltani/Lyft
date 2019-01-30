<template>
  <div class="body">
      <div class="header">
        <div class="logo container p-3 pt-5 mb-5 col-12">
          <a href="https://www.lyft.com/drive-with-lyft"><img src="../assets/lyft-logo-png-4.png"></a>
        </div>
      <div class="SignUp container col-12 mt-5 ">
        <h1 id="header"> {{message}}</h1>
        <p> {{msg1}}</p>
        <p> Let's start with your phone number - we'll text you a code to verify your phone.</p>
        <div class="mb-3">
          <input type="radio" class="select" id="hasCar" name="drone" value="hasCar" checked>
          <label class="p-3 mr-3" for="hasCar"> I have a car</label>
          <input type="radio" class="select" id="need" name="drone" value="need">
          <label class="p-3" for="need">I need a car</label>
        </div>
        <input type="text" name="phone" lang="en"  id="phone" placeholder="Mobile Phone Number" class="mb-3 radius border ">
        <input type="checkbox" class="ml-5 mr-2" id="agreeToTerms" name="agreeToTerms" lang="en" value="on">
        <label class="m-1">I agree to Lyft’s Terms of Service</label>
        <div>
          <button type="button" class="btn mt-4 mb-2">Next</button>
          <p class="m-3 mt-4 mb-5">Already applied?<br>
            Check the status of your application here.
          </p>
        </div>
      </div>
    </div>
    <div class="Introduce container mr-5 mb-5 mt-5">
      <h3 class="col-12 mb-4">What is Lyft?</h3>
      <p class="col-7">Lyft matches drivers with passengers who request rides through our smartphone app, and passengers pay automatically through the app.</p>
      <br>
      <p class="col-7 ">Whether you’re trying to offset costs of your car, cover this month’s bills, or fund your dreams, Lyft will get you there. So, go ahead. Be your own boss.</p>
      <br>
      <h3 class="col-12 mt-5 mb-5">Why Lyft?</h3>
      <div class="d-flex flex-row">
        <div class="col-4">
          <img src="https://cdn.lyft.com/brochure/drive-for-lyft-tip.2f3fb8aa.svg" alt="Keep your tips" class="_3HIEj7 text-bold m-y-m" data-reactid="126">
          <h6 class="mb-4">Keep Your Tips</h6>
          <p>Earn tips from your passengers and keep the whole amount — they’re yours.</p>
        </div>
        <div class="col-4">
          <img src="https://cdn.lyft.com/brochure/drive-for-lyft-pay.90278969.svg" alt="Make more money" class="_3HIEj7 text-bold m-y-m" data-reactid="131">
          <h6 class="mb-4">Make More Money</h6>
          <p>With increased Prime Time pricing during peak hours, you make more with Lyft.</p>
        </div>
        <div class="col-4">
          <img src="https://cdn.lyft.com/brochure/drive-for-lyft-community.a243fe20.svg" alt="Best community" class="_3HIEj7 text-bold m-y-m" data-reactid="136">
          <h6 class="mb-4">Best Community</h6>
          <p>The Lyft community is full of awesome, friendly people — passengers and drivers alike.</p>
        </div>
      </div>
    </div>
    <div class="wrapper mt-5" style="position: relative;height: 700px">
      <div class="App" style=""> </div>
      <div  class="IPhone row h-100 col-3" >
        <slick ref="slick" :options="slickOptions">
        <img class="col-11 ml-4 w-50x " id="one" value="One" v-model="selected" style="margin-top:98px;" src="https://cdn.lyft.com/brochure/walkthrough-01.81a701e8.jpg">
        <img class="col-11 ml-4 w-51" id="two" value="two" v-model="selected" style="margin-top:98px;" src="https://cdn.lyft.com/brochure/walkthrough-02.e7359c27.jpg">
        <img class="col-11 ml-4 w-51" id="three" value="three" v-model="selected" style="margin-top:98px;" src="https://cdn.lyft.com/brochure/walkthrough-03.3e63b376.jpg">
        <img class="col-11 ml-4 w-51" id="four" value="four" v-model="selected" style="margin-top:98px;" src="https://cdn.lyft.com/brochure/walkthrough-04.6b5f9a19.jpg">
        </slick>
          <div style="background-size:50%;background-image:url(https://cdn.lyft.com/brochure/walkthrough-01.81a701e8.jpg);" class="_2VXdTo _1GXO7I _3fkLet _2VXUlm" title="In-app screenshot of driver mode" data-reactid="170"></div>
      </div>
      <h3 class="col-4 ml-5 p-4">How Lyft Driving Works</h3>
      <span>{{ selected }}</span>
    </div>
    <div class="content mt-5">
      <div class="d-flex p-5">
        <div class="col-md-offset-2 mr-4 mt-5 p-5">
          <img  src="https://cdn.lyft.com/brochure/drive-for-lyft-shield.88213cf8.png" alt="Lyft insurance protection shield" class="_5nJMsT _2HGDap center-block m-y-m" data-reactid="195">
        </div>
        <div class="col-md-6 mt-5 p-1">
          <h3>Lyft Insurance Protection</h3>
          <p class="pr-1">Lyft provides additional insurance policies,
            at no cost to the driver. We worked with leading insurance
            carriers to provide various coverages including:
            commercial auto liability insurance up to $1M
            occurrence, contingent comprehensive and collision
            insurance for drivers who carry comprehensive and collision
            coverage on their personal auto policy, and coverage for bodily
            injury caused by uninsured/underinsured motorists when you are engaged
            in a ride. If you already carry commercial insurance or personal coverage
            providing specific coverage for ridesharing, Lyft’s policy will continue
            to be excess to your insurance coverage. Please note, the above coverage
            may be modified to comply with local regulations or state laws. Our policy
            is available in all states in the U.S., except for those rides originating
            in New York City with a TLC (Taxi and Limousine Commission) driver.<br><a href="#">Get information about our insurance policies.</a></p>
        </div>
      </div>
      <div class="d-flex p-5">
        <div class="col-md-offset-2 mr-4 mt-3 p-5">
          <img src="https://cdn.lyft.com/brochure/drive-for-lyft-five-stars.ab6c1047.png" alt="Five star rating" class="_5nJMsT _2HGDap center-block m-y-m" data-reactid="201">
        </div>
        <div class="col-md-6 mt-5 p-1">
          <h3>Passenger Ratings</h3>
          <p class="pr-1">Drivers rate passengers after each ride, so you’ve always got a say. We also require passengers to provide valid credit card information for identity verification purposes.</p>
        </div>
      </div>
    </div>
    <div class="container mt-5 p-5">
      <h3 class="row h-100 justify-content-center p-5">Frequently Asked Questions</h3>
      <hr class="col-7 mt-5">
      <div class="container col-7 Question d-flex flex-column justify-content-center">
        <h4 class="pt-5 pr-5 pl-5">I already have a job, so can I just drive a few hours in my off-time?</h4>
        <p class="pr-5 pl-5">Absolutely. You choose when you drive. Some drivers make more than $800 just driving Friday nights and weekends.</p>
        <hr class="col-11 mt-5">
      </div>
      <div class="container col-7 Question d-flex flex-column justify-content-center">
        <h4 class="pt-5 pr-5 pl-5">How do I get paid?</h4>
        <p class="pr-5 pl-5">Drivers get paid for every trip on a per minute and mile basis. Money is deposited into your account each week automatically, or you can cash out instantly with Express Pay.</p>
        <hr class="col-11 mt-5">
      </div>
      <div class="container col-7 Question d-flex flex-column justify-content-center">
        <h4 class="pt-5 pr-5 pl-5">Is Lyft safe?</h4>
        <p class="pr-5 pl-5">Our community’s safety is our top priority. We run extensive background checks on drivers, provide up to $1M commercial automobile liability policy, and designed numerous safety features into our app. Passengers must provide a valid credit card and phone number for identity verification purposes. Drivers and passengers also rate each other at the end of a ride, so that we’re always upholding our high community standards.</p>
        <hr class="col-11 mt-5">
      </div>
      <div class="container col-7 Question d-flex flex-column justify-content-center">
        <h4 class="pt-5 pr-5 pl-5">What are Lyft’s requirements?</h4>
        <p class="pr-5 pl-5">You must be at least 21 and own an iPhone or Android phone. As part of our approval process, you’ll undergo a DMV check, plus a national and county background check. This will require a Social Security number, in addition to an in-state driver’s license that is at least a year old. Learn more about our background check standards on our <a href="#">Safety page</a>, and our comprehensive driver requirements in the <a href="#">Help Center.</a></p>
        <hr class="col-11 mt-5">
      </div>
      <div class="container col-7 Question d-flex flex-column justify-content-center">
        <a href="#" class="pr-5 pl-5">See more commonly asked questions</a>
      </div>
      <div class="container row h-100 justify-content-center mt-5 p-5">
      <button type="button" class="btn">Apply Now</button>
      </div>
    </div>
    <hr>
    <div class="footer mt-5 mb-3 p-3 row h-100 justify-content-center">
      <p class="p-3">Interested in driving for Lyft?</p>
      <button type="button" class="btn ml-5 mr-4">No, Thanks</button>
      <button type="button" class="btn1">Yes</button>
    </div>
  </div>
</template>

<script>
  import Slick from 'vue-slick'
  export default {
    components: {
      Slick,
    },
    props: {
      images: Array,
    },
    data () {
      return {
        message: 'Drive toward what matters.',
        msg1: 'Sign up to drive',
        slickOptions: {
          arrows: false,
	        autoplay: true,
          autoplaySpeed: 500,
          fade: true,
          fadeSpeed: 100,
          dots: true,
          infinite: true,
        },
      };
    },
    methods: {
      next() {
        this.$refs.slick.next();
      },

      prev() {
        this.$refs.slick.prev();
      },
    }
}
</script>

<style>
  @import "../../node_modules/slick-carousel/slick/slick.css";
  @import "https://maxcdn.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css";
  @import "https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css";
  @import "https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css";
  @import "https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css";

div {
  overflow: hidden;
}

.header{
  background-color: rgb(119, 94, 240);
}

.logo img{
  width: 80px;
}

input::placeholder{
  color: whitesmoke;
  font-size: 0.7em;
  font-style: italic;
}

label {
  font-size: 1.5rem;
  font-weight: 300;
  color: whitesmoke;
  font-family: Calibri;
}

.SignUp{
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  color: white;
}

.SignUp p{
  font-size: 1.9rem;
  font-weight: 500;
  color: white;
  font-family: Calibri;
}

.SignUp .select{
  display: inline-flex;
  vertical-align: middle;
  align-items: center;
  justify-content: center;
  -webkit-appearance: none;
  border: 2px solid #ac9af5;
  border-radius: 20px;
  width: 30px;
  height: 30px;
  background-color: rgb(119, 94, 240);
  position: relative;
}

.SignUp .select:checked:after {
  content: " ";
  position: absolute;
  background: #fff;
  border-radius: 20px;
  width: 20px;
  height: 20px;
  border-color: #785ef0;
  border: 1px solid #785ef0;
}

.SignUp #phone {
  background: #5646c0;
  border: none;
  border-top: 2px solid #41358f;
  color: #fff;
  padding-top: 1.2rem;
  padding-bottom: 1.2rem;
  padding-left: 1.25rem;
  font-size: 1.9rem;
  border-radius: 10px;
}

.SignUp #agreeToTerms{
  display: inline-flex;
  vertical-align: middle;
  align-items: center;
  justify-content: center;
  -webkit-appearance: none;
  border: 3px solid #ac9af5;
  border-radius: 1px;
  width: 30px;
  height: 30px;
  background-color: rgb(119, 94, 240);
  position: relative;
}

.SignUp #agreeToTerms:checked:after {
  content: " ";
  position: absolute;
  background: #fff;
  border-radius: 1px;
  width: 20px;
  height: 20px;
  border: 1px solid #785ef0;
}

.IPhone{
  position: absolute;
  top:0;
  background-image:url(https://cdn.lyft.com/brochure/phone@1x.c7273ad8.png);
  background-size: contain;
  background-position: center;
  background-repeat: no-repeat;
  margin-left: 500px;
  height: 630px;
  width: 350px;
}

h1{
  font-size: 5em;
  font-weight: bold;
}

h3{
  font-size: 3.4em;
  font-weight: bold;
}

h6{
  font-size: 1.8rem;
  font-weight: bold;
}

h4{
  font-size: 2em;
  font-weight: bold;
}

.Introduce p {
  font-size: 1.7rem;
  font-weight: 300;
  color: #373a3c;
  font-family: Calibri;
}

.Introduce img{
  width: 11rem;
  height: 11rem;
}

.App{
  background-image: url(https://cdn.lyft.com/brochure/bg_img.e12d60d0.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 500px;
}

.content{
  background-color: whitesmoke;
}

.content img{
  width: 13rem;
  height: 13rem;
}

.content p{
  font-size: 1.7rem;
  font-weight: 300;
  color: #373a3c;
  font-family: Calibri;
}

.content a{
  text-decoration: solid;
}

.Question p{
  font-size: 1.7rem;
  font-weight: 500;
  color: #373a3c;
  font-family: Calibri;
}

.btn1{
  min-width: 200px!important;
  height: 56px;
  border-radius: 100px;
  box-shadow: 0 6px 0 0 rgba(17,17,31,.4);
  background-color: #4a148c;
  border: 2px solid #11111f;
  color: white!important;
  text-decoration: none!important;
  line-height: 2rem;
  font-weight: 700;
}

.btn{
  min-width: 200px!important;
  height: 56px;
  border-radius: 100px;
  box-shadow: 0 6px 0 0 rgba(17,17,31,.4);
  background-color: #fff;
  border: 2px solid #11111f;
  color: #11111f!important;
  text-decoration: none!important;
  line-height: 2rem;
  font-weight: 700;
}

.footer p{
  font-size: 2rem;
  font-weight: bold;
  color: #373a3c;
  font-family: Calibri;
}

.slick-dots {
  display: flex;
  justify-content: center;
  margin-top: 15vh;
  padding: 1rem 0;
  list-style-type: none;
}

.slick-dots	li {
  margin: 0 0.25rem;
}

.slick-dots	button {
  display: block;
  width: 1.2rem;
  height: 1.2rem;
  padding: 0;
  border: solid;
  border-radius: 100%;
  background-color: white;
  text-indent: -9999px;
}

.slick-dots	li.slick-active button {
  background-color: black;
}
</style>
