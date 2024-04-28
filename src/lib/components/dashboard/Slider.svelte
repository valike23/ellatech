 <script lang="ts">
    import { onMount } from "svelte";
 let win: any = {};
    onMount(()=>{
        win = window;
       win.$('.hero-slider').slick({
    infinite: true,
    fade: true,
    dots: false,
    prevArrow: '<button class="slick-prev"><i class="fa fa-angle-left"></i></button>',
    nextArrow: '<button class="slick-next"><i class="fa fa-angle-right"></i></button>',
    responsive: [
        {
        breakpoint: 992,
            settings: {
                dots: true,
                arrows: false,
            }
        },
    ]
});
    })
 </script>
 
 
 <div class="hero-section section position-relative">
        <div class="hero-slider section">

            <!--Hero Item start-->
            <div class="hero-item" style="background-image: url(/assets/images/slider/oilring1.jpeg)">
                <div class="container">
                    <div class="row">
                        <div class="col-12">

                            <!--Hero Content start-->
                            <div class="hero-content-2">

                                <h2>Welcome to</h2>
                                <h1>EllaTech.</h1>
                                <p>Ellatech Engineering services LTD, provides a full range of 
                                    services that cut across Oil & Gas,Petrolchemical and allied 
                                    industries for core industrial sectors.
                                </p>
                                <a href="/" class="btn">explore now</a>

                            </div>
                            <!--Hero Content end-->

                        </div>
                    </div>
                </div>
            </div>
            <!--Hero Item end-->
            <!--Hero Item start-->
            <div class="hero-item" style="background-image: url(/assets/images/slider/team.jpeg)">
                <div class="container">
                    <div class="row">
                        <div class="col-12">

                            <!--Hero Content start-->
                            <div class="hero-content-2">

                                <h2>Since 2013</h2>
                                <h1>We Build The Trust.</h1>
                                <p>
                                    Over  the  years, we have  rendered tailor-made solutions 
                                     that meets the wildest imagination of our clients. With  our 
                                      cutting-edge methods  of  service  for  effective  and  
                                      on-time delivery  plus 
                                     our  management  and production /maintenance  system
                                     that is in line with our philosophy of minimizing costs 
                                     while maximizing quality,   we   have   achieved 
                                       cost-effective  results   for   our   clients.
                                </p>
                                <a href="/" class="btn">explore now</a>

                            </div>
                            <!--Hero Content end-->

                        </div>
                    </div>
                </div>
            </div>
            <!--Hero Item end-->

        </div>
    </div>