<template>
    <div class="carousel relative shadow-2xl bg-white" id="abstract">
        <div class="carousel-inner relative overflow-hidden w-full transition-transform">
        <!--Slide 1-->
            <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden="" checked="checked">
            <div class="carousel-item absolute opacity-0" style="height:80vh;">
                <div class="block h-full flex flex-row ml-32 mt-20 justify-left align-center self-center">
                    <img src="@/assets/img/screen_1.png" style="height:70%; width: auto; margin: 0 auto;"/>
                    <div class="mt-16 ">
                        <p class="mt-16 text-5xl text-black">Why ZeroPlastic?</p>
                        <p class="mt-12 text-xl text-black" style="margin-right: 20%">ZeroPlastic is a platform where businesses can finance people to collect plastic waste. In this way, companies can reduce their plastic footprint, jobs are created and the environment is safeguarded.</p>
                    </div>
                </div>
            </div>
            <label for="carousel-3" class="prev control-1 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
            <label for="carousel-2" class="next control-1 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label>
            
            <!--Slide 2-->
            <input class="carousel-open" type="radio" id="carousel-2" name="carousel" aria-hidden="true" hidden="">
            <div class="carousel-item absolute opacity-0" style="height:80vh;">
                <div class="block h-full flex flex-row ml-32 mt-20 justify-left align-center self-center">
                    <img src="@/assets/img/screen_2.png" style="height:70%; width: auto; margin: 0 auto;"/>
                    <div class="mt-16 ">
                        <p class="mt-16 text-5xl text-black">The user perspective</p>
                        <p class="mt-12 text-xl text-black" style="margin-right: 20%">Users of our platform are able to earn money and special offers from shops simply collecting plastic garbage around their city. Our contributions are backed by companies that are willing to offset their plastic emissions.</p>
                    </div>
                </div>
            </div>
            <label for="carousel-1" class="prev control-2 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
            <label for="carousel-3" class="next control-2 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label> 
            
            <!--Slide 3-->
            <input class="carousel-open" type="radio" id="carousel-3" name="carousel" aria-hidden="true" hidden="">
            <div class="carousel-item absolute opacity-0" style="height:80vh;">
                <div class="block h-full flex flex-row ml-32 mt-20 justify-left align-center self-center">
                    <img src="@/assets/img/screen_3.png" style="height:70%; width: auto; margin: 0 auto;"/>
                    <div class="mt-16 ">
                        <p class="mt-16 text-5xl text-black">Building the future of plastic waste picking</p>
                        <p class="mt-12 text-xl text-black" style="margin-right: 20%">We instruct our users to identify plastic garbage in images collected by our community. With this power, we're able to train deep learning algorithms that will enhance the state-of-the-art of the waste classification, in the near future.</p>
                    </div>
                </div>
            </div>
            <label for="carousel-2" class="prev control-3 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
            <label for="carousel-1" class="next control-3 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label>

            <!-- Add additional indicators for each slide-->
            <ol class="carousel-indicators">
                <li class="inline-block mr-3">
                    <label for="carousel-1" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
                </li>
                <li class="inline-block mr-3">
                    <label for="carousel-2" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
                </li>
                <li class="inline-block mr-3">
                    <label for="carousel-3" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
                </li>
            </ol>
            
        </div>
    </div>
</template>

<style>
			.carousel-open:checked + .carousel-item {
				position: static;
				opacity: 100;
			}
			.carousel-item {
				-webkit-transition: opacity 0.6s ease-out;
				transition: opacity 0.6s ease-out;
			}
			#carousel-1:checked ~ .control-1,
			#carousel-2:checked ~ .control-2,
			#carousel-3:checked ~ .control-3 {
				display: block;
			}
			.carousel-indicators {
				list-style: none;
				margin: 0;
				padding: 0;
				position: absolute;
				bottom: 2%;
				left: 0;
				right: 0;
				text-align: center;
				z-index: 10;
			}
			#carousel-1:checked ~ .control-1 ~ .carousel-indicators li:nth-child(1) .carousel-bullet,
			#carousel-2:checked ~ .control-2 ~ .carousel-indicators li:nth-child(2) .carousel-bullet,
			#carousel-3:checked ~ .control-3 ~ .carousel-indicators li:nth-child(3) .carousel-bullet {
				color: #2b6cb0;  /*Set to match the Tailwind colour you want the active one to be */
			}
		</style>
