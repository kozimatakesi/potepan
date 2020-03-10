$(function(){
    $('.index-btn').click(function(){
        $('.active').removeClass('active');
        $('.color-change').removeClass('color-change').html('<img src="https://camp.potepan.com/wp-content/themes/potepancamp/assets/images/btn-slide-control-default.png">');
        var clickedIndex = $('.index-btn').index($(this));
        $('.slide').eq(clickedIndex).addClass('active');
        $('.index-btn').eq(clickedIndex).addClass('color-change');
        $('.color-change').html('<img src="https://camp.potepan.com/wp-content/themes/potepancamp/assets/images/btn-slide-control-click.png">');
    });

    $('.change-btn').click(function(){
        var slideIndex = $('.slide').index($('.active'));
        var $displaySlide = $('.active');
        $displaySlide.removeClass('active');
        var $colorOrange = $('.color-change');
        $colorOrange.removeClass('color-change').html('<img src="https://camp.potepan.com/wp-content/themes/potepancamp/assets/images/btn-slide-control-default.png">');
        if($(this).hasClass('next-btn')){
            if(slideIndex == 2){
                $('.slide').eq(0).addClass('active');
                $('.index-btn').eq(0).addClass('color-change');
                $('.color-change').html('<img src="https://camp.potepan.com/wp-content/themes/potepancamp/assets/images/btn-slide-control-click.png">');
            } else {
                $displaySlide.next().addClass('active');
                $colorOrange.next().addClass('color-change');
                $('.color-change').html('<img src="https://camp.potepan.com/wp-content/themes/potepancamp/assets/images/btn-slide-control-click.png">');
            }
        } else {
            if(slideIndex == 0){
                $('.slide').eq(2).addClass('active');
                $('.index-btn').eq(2).addClass('color-change');
                $('.color-change').html('<img src="https://camp.potepan.com/wp-content/themes/potepancamp/assets/images/btn-slide-control-click.png">');
            }
            else {
                $displaySlide.prev().addClass('active');
                $colorOrange.prev().addClass('color-change');
                $('.color-change').html('<img src="https://camp.potepan.com/wp-content/themes/potepancamp/assets/images/btn-slide-control-click.png">');
            }
        }
    });

    $('.move-top-btn').click(function(){
        $('html, body').animate({scrollTop:0});
    });

    $('.course-hover').click(function(){
        var id = $(this).attr('href');
        var position = $(id).offset().top;
        $('html, body').animate({
            'scrollTop': position 
          }, 500);
    });

});
