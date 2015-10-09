/*global $:false */



// ONEPAGENAV SETTINGS


 $(document).ready(function(){
 "use strict";
  
  $('#home .main_nav').onePageNav({
    currentClass: 'active',
    changeHash: false,
    scrollSpeed: 750,
    scrollOffset: 40,
    filter: ':not(.external)',
    easing: 'swing',
});



$('.logo_container').onePageNav({
    changeHash: false,
    scrollSpeed: 750,
    scrollOffset: 85,
    filter: '',
    easing: 'swing',
});


$('#home .responsive_nav').onePageNav({
    changeHash: false,
    scrollSpeed: 750,
    scrollOffset: 0,
    filter: '',
    easing: 'swing',
});
  
});


 $(window).load(function(){
  "use strict";

  $('.custom_button').onePageNav({
    changeHash: true,
    scrollSpeed: 750,
    scrollOffset: 40,
    filter: '',
    easing: 'swing',
});
});


//CAROUSEL SLIDER

$(document).ready(function() {
$('.slidewrap').carousel({
  slider: '.slider',
  slide: '.slide',
  slideHed: '.slidehed',
  nextSlide : '.next',
  prevSlide : '.prev',
  addPagination: false,
  addNav : true,
  speed: 500 // ms.
});

$('.slidewrap2').carousel({
  slider: '.slider',
  slide: '.slide',
  slideHed: '.slidehed',
  nextSlide : '.next',
  prevSlide : '.prev',
  addPagination: false,
  addNav : true,
  speed: 500 // ms.
});

$('.slidewrap3').carousel({
  slider: '.slider',
  slide: '.slide',
  slideHed: '.slidehed',
  nextSlide : '.next',
  prevSlide : '.prev',
  addPagination: false,
  addNav : true,
  speed: 500 // ms.
});
$('.slidewrap4').carousel({
  slider: '.slider',
  slide: '.slide',
  slideHed: '.slidehed',
  nextSlide : '.next',
  prevSlide : '.prev',
  addPagination: false,
  addNav : true,
  speed: 500 // ms.
});
});



$(document).ready(function() {
    "use strict";
    // cache container
    var $container = $('#container_portfolio');


    
        // initialize isotope
         $container.isotope({
          masonry: {
            columnWidth: 1
          }
        });


       // filter items when filter link is clicked
        $('#filters a').click(function(){
          var selector = $(this).attr('data-filter');
          $container.isotope({ filter: selector });
          return false;
        });
         
 });





$(document).ready(function() {
   "use strict";
      $('#filters li>a').click(function() {
   $('#filters li').removeClass('active');
      $(this).parent().addClass('active');
      });
});


//AJAX PORTFOLIO

  $(window).load(function(){
  
  (function(){
  
    var container = $( "#portfoliod" );
    var $items = $('#container_portfolio > div.portfolio_item');
     index = $items.length;
      $('#container_portfolio .portfolio_item').click(function(){

      if ($(this).hasClass('active')){
      } else 
      { lastIndex = index;
      index = $(this).index();
      $items.removeClass('active');
      $(this).addClass('active');

      var myUrl = $(this).find('.ajax-trigger').attr("href") + " .item-data"; 

      /*$('html, body').animate({scrollTop:20}, 800)*/ //Use this to scroll to the 20px top of the page
      $('html, body').animate({ scrollTop: $(".portfolio-top").offset().top - 50
      }, 400); //Custom scroll to .portfolio-top div 
      $('.loading_icon').css({ "display": "block", "opacity": "0" }).animate({ "opacity": "0.8" }, 300);
      $('#portfolioData').animate({opacity:0}, 400,function(){  
        $("#portfolioData").load(myUrl,function(){   //FIX THE HEIGHT BUG ON FLEXSLIDER
            var $helper = $('.helper');
            var height = $helper.height();
            $('#portfolioData').css("min-height", height);
            $('.flexslider').flexslider({
              smoothHeight: true,controlNav:false
            });
            $('.flexslider').css({'height' : ''});
        });
        $('#portfolioData').animate({opacity:1}, 400);

      });
      
      //SLIDE UP
        
      $('#portfoliod').slideUp(400, function(){
        $('.loading_icon').delay(800).animate({ "opacity": "0" }, 100,function(){
          $('.loading_icon').css("display","none");
        });
        $('#portfolioData').css('visibility', 'visible');}).delay(800).slideDown(400,function(){
          $('#portfolioData').animate({opacity:1}, 400);
          $("a[class^='prettyPhoto']").prettyPhoto();

      });


      }

      return false;       
      
      });

    //AJAX CLOSE 
    $('#ajax_close').click(function() {
      $('#portfoliod').slideUp(400);
      $items.removeClass('benext beprev active') ;
      return false;
        });

  })();
  
});




// RESPONSIVE MENU 

$(document).ready(function(){
"use strict";  
var menu_trigger = $('.menu_trigger');
var areamenu = $('.mobileAreaMenu');
var all_li =$('.mobileAreaMenu li');

$(menu_trigger).click(function() {


if ($(menu_trigger).hasClass('active')){

      $(areamenu).slideUp(200,function(){
        $(areamenu).css("display","");
        $(menu_trigger).removeClass("active");
      });
          
      } else {
        $(areamenu).slideDown(200,function(){
          //
        });

        $(menu_trigger).addClass("active");
      }
});

$('.mobileAreaMenu a').click(function(){
  $(areamenu).slideUp(200);
  $(menu_trigger).removeClass("active");
});
});


// PRETTY PHOTO

$(window).load(function(){
 "use strict";
    $("a[class^='prettyPhoto']").prettyPhoto();
  });




// FIX FOR ISOTOPE PORTFOLIO FIRST TRIGGER

$(window).load(function() { 
"use strict";
$('#filters li.active a').trigger('click');

}); 


// SKILLS BARS EFFECT

$(document).ready(function() {
"use strict";  
var bars = $('.bar');

var bar_one = $(bars).slice(0,1);
var bar_one_percent = $(bar_one).find('.percent').text();

var bar_two = $(bars).slice(1,2);
var bar_two_percent = $(bar_two).find('.percent').text();

var bar_three = $(bars).slice(2,3);
var bar_three_percent = $(bar_three).find('.percent').text();

var bar_four = $(bars).slice(3,4);
var bar_four_percent = $(bar_four).find('.percent').text();

var bar_five = $(bars).slice(4,5);
var bar_five_percent = $(bar_five).find('.percent').text();

var bar_six = $(bars).slice(5,6);
var bar_six_percent = $(bar_six).find('.percent').text();

var bar_seven = $(bars).slice(5,6);
var bar_seven_percent = $(bar_seven).find('.percent').text();

setTimeout(
  function() 
  {

  $(bar_one).animate({width:bar_one_percent}, 900);
  $(bar_two).animate({width:bar_two_percent}, 900);
  $(bar_three).animate({width:bar_three_percent}, 900);
  $(bar_four).animate({width:bar_four_percent}, 900);
  $(bar_five).animate({width:bar_five_percent}, 900);
  $(bar_six).animate({width:bar_six_percent}, 900);
  $(bar_seven).animate({width:bar_seven_percent}, 900);


  }, 800);

});



// TWITTER USERNAME 


$(function($){
"use strict"; 
  $("#twitterfeed").tweet({
    username: "bypixels", /*Enter your Twitter username */
    modpath: 'js/twitter/', /* director of the twitter folder : ABSOLUTLY DIRECT LINK OF YOUR TWITTER FOLDER */
    page: 1, /*How many tweets to show at a time*/
    avatar_size: null, 
    count: 5, /*Total counts of tweets. */
    loading_text: "Loading latest tweets..." /*Loading text*/
  });     
  
});




// TESTIMONIALS


$(document).ready(function() {
"use strict";
var alltabs = $('.col_wrapper');

$(".testimonial").hide(); 
$(".testimonial:first").show(); 
  $(".testi_column a").click(function() {

    $(alltabs).removeClass("active");
    $(this).parent('.col_wrapper').addClass("active");
    $(".testimonial").hide(); 

    var activeTab = $(this).attr("href"); 

    $(activeTab).fadeIn(600); 

    return false;

  });

});



// TWITTER FADE EFFECT IN FOOTER

$(document).ready(function() {
"use strict";
var all_tweets = $('.tweet_list li');
var all_tweets_first = $('.tweet_list li:first-child');
var n_tweeets = $(all_tweets).length;
var i = 2;
var first_slice = 1;
var second_slice = 2;
var time = 5000;
$(all_tweets).hide();
$(all_tweets_first).show();

function tweet_loop() {
    setInterval(function() { // this code is executed every 5000 milliseconds (var time = 5000;)

if( i <= n_tweeets ){
$(all_tweets).fadeOut(800);
$(all_tweets).slice(first_slice,second_slice).delay(950).fadeIn(800);

       i++;
       first_slice ++;
       second_slice++;

} //enf i <= n_tweeets
else {
       i= 1;
      first_slice = 0;
      second_slice = 1;
    }

}, time);
}
$(tweet_loop);
});




//RESPONSIVE STYLE 4 VIDEO RESPONSIVE BACKGROUND

$(document).ready(function() {
  
"use strict";
var height_video = $(window).width();
var height_responsive = (height_video / 1.79011) + 1;
$('.video_slide').css("height",height_responsive);

});


$(window).resize(function() {
  "use strict";
var height_video = $(window).width();
var height_responsive = (height_video / 1.79011) + 1;
$('.video_slide').css("height",height_responsive);

});



//RUN REVOLUTION SLIDER


  $(window).load(function() { 
"use strict";
    $('.fullwidthbanner-container').css("visibility","");
    
    var api;
      jQuery(document).ready(function() {
         api =  jQuery('.fullwidthbanner').revolution(
                {
                  delay:9000,
                  startheight:900,
                  startwidth:1170,

                  hideThumbs:10,

                  thumbWidth:100,             // Thumb With and Height and Amount (only if navigation Tyope set to thumb !)
                  thumbHeight:50,
                  thumbAmount:5,

                  navigationType:"both",          //bullet, thumb, none, both   (No Thumbs In FullWidth Version !)
                  navigationArrows:"verticalcentered",    //nexttobullets, verticalcentered, none
                  navigationStyle:"round",        //round,square,navbar

                  touchenabled:"on",            // Enable Swipe Function : on/off
                  onHoverStop:"on",           // Stop Banner Timet at Hover on Slide on/off

                  navOffsetHorizontal:0,
                  navOffsetVertical:20,

                  stopAtSlide:-1,
                  stopAfterLoops:-1,

                  shadow:0,               //0 = no Shadow, 1,2,3 = 3 Different Art of Shadows  (No Shadow in Fullwidth Version !)
                  fullWidth:"on"              // Turns On or Off the Fullwidth Image Centering in FullWidth Modus
                });
      });

    
  });


// HEIGHT FOOTER RESPONSIVE

$(document).ready(function() {
  
"use strict";
var height_map = $('#map_google').height();
var window_with = $(window).width();
if ( window_with > 767) {
    $('#footer').removeClass("footer_mobile").css("height",height_map);
}
else {
   $('#footer').addClass("footer_mobile").css("height","");
}

});



$(window).resize(function() {
  
"use strict";
var height_map = $('#map_google').height();
var window_with = $(window).width();
if ( window_with > 767) {
    $('#footer').removeClass("footer_mobile").css("height",height_map);
}
else {
   $('#footer').addClass("footer_mobile").css("height","");
}

});






// MOVING ARROWS IN PARALLAX FOR CAROUSEL

$(window).load(function() {

var parallax = $('.parallax');

$(parallax).each(function() {

  var current_slide = $(this).find('.slidecontrols');
   
   $(this).append(current_slide)
   });


});




