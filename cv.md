## **Aliaksandr Tsimashenka**

*Telephone number:* +375291883714  
*E-mail:* tihonec84@mail.ru  
[GitHub](https://github.com/tihonec84)  

### **Summary**

Novice web-developer.Confident knowledge of HTML,CSS. 

### **Skills**

**Programming languages and technologies**: HTML,CSS,Java,PHP,MySQL.  
**Programming practices**: Training projects, freelanse projects, code review.
**Frameworks and Libraries**: Bootstrap3(4), JQuery, CMS-Modx Evolution.  
**Tools**: PHP Storm, Sublime Text3, Eclipse, Intellij IDEA.  
**Other skills**: Photoshop,Figma,Blisk,Open Server.
### **Code Examples**

```
(function ($) {

 $(document).ready(function () {
        // PROGRESS BAR
        var $progress = $('.about__skills--bar');
        $progress.eq(0).animate({width:"90%"}, 7000);
        $progress.eq(1).animate({width:"95%"}, 7000);
        $progress.eq(2).animate({width:"50%"}, 7000);
        $progress.eq(3).animate({width:"85%"}, 7000);
        $('.about__skills--number').delay(7000).fadeIn(1500);

    });
 
    // SLIDER
    $(document).ready(function() {
        $('.home__carousel').slick({
            initialSlide: 1,
            dots: true,
            speed: 800,
            fade: true,
            slide: 'div',
            arrows: true,
            prevArrow: '.carousel__arrow--prev',
            nextArrow: '.carousel__arrow--next',
            dotsClass: 'slick-dots carousel__dots',

        });
        $('.home__carousel--slider').click(function next() {
            $('.home__carousel').slick('slickNext');
        });
    });

    // ISOTOPE
    $(document).ready(function () {
        var $pictures = $('.home__isotope').isotope({
            itemSelector: '.home__isotope--el',
            masonry: {
                gutter: 45,
                horizontalOrder: true
            }
        });

        $('.home__group').on( 'click', 'button', function() {
            var filterValue = $(this).attr('data-filter');
            $pictures.isotope({ filter: filterValue });
            $('.home__group').find('.home__group--active').removeClass('home__group--active');
            $(this).addClass('home__group--active');
        });
        function getItemElement() {
            var $item = $('<div class="col-xs-3 home__isotope--el wordpress" ' +
                'data-big="./img/home/img6.png"><img src="./img/home/img6.png">' +
                '<div class="mask"><span class="mask__zoom">+</span>\n' +
                '</div></div>');
            return $item;
        };
        function getItemElement1() {
            var $item1 = $('<div class="col-xs-3 home__isotope--el mobile-app" ' +
                'data-big="./img/home/img4.png"><img src="./img/home/img4.png"><div class="mask">\n' +
                '<span class="mask__zoom">+</span>\n' +
                '</div></div>');
            return $item1;
        };
        function getItemElement2() {
            var $item2 = $('<div class="col-xs-3 home__isotope--el webdesign" ' +
                'data-big="./img/home/img2.png"><img src="./img/home/img2.png"><div class="mask">\n' +
                '<span class="mask__zoom">+</span>\n' +
                '</div></div>');
            return $item2;
        };
        $('.home__isotope--append').on( 'click', function() {
            var $items = getItemElement().add( getItemElement1() ).add( getItemElement2() );
            $pictures.append( $items )
                .isotope( 'appended', $items );
            console.log('Added 3 images');
            $('.home__isotope--el').pan();
        });
        $('.home__isotope--el').pan();  
     });
```
### **Experience**

**Freelance**
 (06.2019 - now).

### **Education**

**Sukhoi P.O. Gomel State Technical University**,Gomel,Belarus;   
Electricity Power Department;
  
### **Courses**

**Courses Software Development** IT-Class, Gomel, 09.2015 - 08.2017.
**Web Application Development with Java** Epam Training Center, Gomel, 11.2018 - 03.2019.  
**HtmlAcademy** [htmlacademy](https://htmlacademy.ru/profile/id1040235).

### **English**
Pre-Intermediate (A2).