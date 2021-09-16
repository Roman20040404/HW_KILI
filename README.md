<!doctype html>

<!-- так в HTML обозначаются комментарии. Выше вы видите объявление типа документа (DOCTYPE), так браузер понимает, что код ниже нужно интерпретировать как html -->

<html>

<!-- зона заголовка html, тег <title> - строка, которую браузер отображает на вкладках над страницами, <meta> и <link> сообщают технические сведения для браузера, например, что файл имеет кодировку Юникод (utf-8) -->

	<head>
		<title>Личная страница Романа Цховребова</title>
	 	<!-- Required meta tags -->
	 	<meta charset="utf-8">
	 	<meta name="viewport" content="width=device-width, initial-scale=4">

		<meta name="description" content="Личная страница и контакты">

		<!-- Bootstrap Core CSS -->
		<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet" media="screen">
<!-- Эта страница сделана с помощью bootstrap - популярной библиотеки для создания и настройки сайтов. Ниже вы увидите, что многие теги содержат атрибуты class - bootstrap содержит шаблоны, как такие элементы красиво оформить -->

	</head>
	
<!-- body - главная, содержательная часть страницы. Контент на этой странице делится на меню (nav), "шапку" (header), "подвал" (footer) и все остальное (мы заключили остаток в тег section) -->	
	<body>

<!-- меню (navigation bar) -->

		<nav id="mainNav" class="navbar navbar-default navbar-fixed-top navbar-custom">

<!-- div - это контейнеры - коробочки с текстом и/или графикой, которые можно вкладывать друг в друга. Пристально смотреть на теги в этой части кода не нужно -->
			<div class="container"> 
				<div class="navbar-header"> 
					<a href="https://www.hse.ru/ba/ling/" class="navbar-brand">ФиКЛ</a> 
				</div> 
				<nav class="collapse navbar-collapse" id="bs-navbar"> 
					<ul class="nav navbar-nav navbar-right"> 
						<li> <a href="https://www.hse.ru/ba/ling/timetable?fromdate=2021.09.01&todate=2021.10.24&groupoid=88306&receiverType=3&timetable-courses=1&timetable-groups=88306&timetable-view-switcher=list">Расписание</a> </li> 
						<li> <a href="https://docs.google.com/forms/d/e/1FAIpQLSd5ilbe2mhWTiK2X3PI-xvhP-aGiHAOU_XW-rSqWTCNEPHOkA/viewform">Заказ справок</a> </li> 
<!-- поправьте номер группы в URL, если нужно (от 1 до 4) -->
					</ul>
				</nav> 
			</div>
		</nav>

<!-- начинается шапка. у тега header есть атрибут style, который задает цвет фона и отступы. поменяйте значения атрибутов и посмотрите, как изменится страница -->

		<header style="background-color:beige; padding-top:110px; "> 
			<div class="container"> 
				<div class="row">
					<div class="col-md-4">
						<br><br>
<!-- здесь и дальше нужно поменять весь содержательный текст, чтобы получилась ваша личная страница -->
						<h1>Роман Цховребов</h1>
						<hr> <!-- это горизонтальная линия -->
						<p><i>Студент, который учится <b>создавать</i> сайты на HTML</b></p> 
					</div>
					<div class="col-md-4">
<!-- img - тег для вставки изображений. Мы использовали атрибут style, чтобы задать размер изображения и ширину рамки-->
<!-- Измените URL на URL вашей фотографии, а также настройте размер изображения -->
<img
    src=Портрет.jpg
	width="465"
	height="500">
	<img
  src=https://02.img.avito.st/1280x960/8641843902.jpg
  title="Мурка"
  alt="Рыжий котёнок"
  width="350"
  height="480"
>
<img
					</div>
				</div>
			</div>
		</header>

<!-- часть страницы, которая под шапкой -->
		<section id="portfolio">
			<div class="container">

<!-- атрибут col-md-... говорит, что контент будет разделен на несколько столбцов, их ширина соотносится как 3 - 6 - 3 (Bootstrap использует воображаемую сетку из 12 равных по ширине колонок) -->
				<div class="col-md-3">

<!-- <article> не влияет на оформление, но помогает структурировать контент на осмысленые разделы -->
					<article>
						<h3>Место учебы</h2>
						<p>Фундаментальная и прикладная лингвистика, НИУ ВШЭ, Москва</p>
					</article>
					<article>
						<h3>Родной город</h2>
						<p>Владикавказ</p>
					</article>
					<article>
						<h3>Школа</h2>
<!-- когда будете менять текст, не используйте бюрократических слов типа ГБОУ СОШ, ну пожаалуйста -->
						<p>Гимназия №5</p>
					</article>
				</div>

				<div class="col-md-6">
					<article>
						<h3>Языки</h2>
						<p>Учу французский, который мне необычайно нравится! <br>
						А также итальянский, который начал здесь, в ВШЭ!<br>
						Он такой мелодичный! <br>
						Такой красивый!<br>
						Vive la république! Vive la France!
						</p>
					</article>
				</div>

				<div class="col-md-3">
					<h3>Я в соцсетях</h3>
<!-- тег <ul> - unordered list. Еще бывает тег <ol> -->
					<ul>
						<li> <a href="https://vk.com/romantskhovrebov">VK</a> </li> 
						<li> <a href="https://www.facebook.com/profile.php?id=100008237627523"> Facebook</li>
						<li><a href="https://www.instagram.com/roman_tskhovreboff/"> Instagram</li>
					</ul>
				</div>
			</div>
		</section>

<!-- это подвал. В этой части страницы обычно ставят копирайт (с помощью символа &copy;) и пишут об истории создания страницы. Поставьте свой копирайт -->
		<footer class="bs-docs-footer"> 
			<div class="container"> 
				<p style="text-align:right; ">&copy; Р. Цховребов, 2021</p> 
			</div>
		</footer>
	</body>
</html>
