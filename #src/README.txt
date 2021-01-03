Есть возможность соединять html фаилы через @@include('_fileName.html')  

если есть шрифты в форматах отличающихся от .ttf выполняем таск gulp otf2ttf

для создания svgSprite используем таск gulp svgSprite

добавляем классы изображениям
К примеру, у нас есть несколько картинок на странице:

<img src="image1.jpg" alt="">
<img src="image2.jpg" alt="">
<img src="image3.jpg" alt="">

Для того, что бы отложить их загрузку, нужно всего переделать их в такой вид:

<img data-src="image1.jpg" class="lazyload" alt="">
<img data-src="image2.jpg" class="lazyload" alt="">
<img data-src="image3.jpg" class="lazyload" alt="">

На этом все. Изображения уже будут загружаться постепенно.
