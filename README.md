# Android-Universal-Web-Content-Loader(UWCL)

###WHAT IS THIS :-

Universal Web Content loader is Native in App brower which help developers to embed web contents in there apps with just one line of code. Web contents can we of any type - youtube playlist, Facebook page, in App Google search or payUMoney payment trannsactions.
Универсальный загрузчик веб-контента является родным в App brower, который помогает разработчикам вставлять веб-контент в приложения только с одной строкой кода. Веб-контент мы можем любого типа-плейлист youtube, страница Facebook, в приложении Google search или payUMoney payment trannsactions.

### WHEN TO USE  :- 

If your app requires loading of web contents in your app and you dont want to waste your timing embedding webviews and writing webview and chrome clients.
Если ваше приложение требует загрузки веб-содержимого в вашем приложении, и вы не хотите тратить время на встраивание webviews и написание WebView и chrome клиентов.


###HOW TO USE :-

Usin this project is very simple :-
 - Drop this fragment in your UI package along with universal_web_view.xml and video_progress.xml.
 - Load web contents in your application with the help of just single line of code.
 - 
   This Fragment class supports all type of web content & can be used in many scenarios such as :-
   Usin этот проект очень прост :-
Семнадцать
- Поместите этот фрагмент в пакет пользовательского интерфейса вместе с universal_web_view.xml и video_progress.XML.
Восемнадцать
- Загрузите веб-содержимое в приложение с помощью всего одной строки кода.
Девятнадцать
- 
Двадцать
Этот класс фрагментов поддерживает все типы веб-материалов и может использоваться во многих сценариях, таких как :-

1) you can embed youtube playlist in your App. The UniversalWebContentLoader(UWCL) allow user to play Videos in portrait mode as well.
1) Вы можете встроить плейлист youtube в свое приложение. UniversalWebContentLoader (UWCL) позволяет пользователю воспроизводить видео в портретном режиме.

				getSupportFragmentManager()
						.beginTransaction()
						.add(R.id.frag_root,
								UniversalWebViewFragment.newInstance(
										YOU_TUBE_DEMO_URL, false)).commit();

2) You can use this fragment for payment gateway like PayUMoney.(*just a word of warning WebViews are not very secure ,feel free to share wisdom and make code better) ) 
2) Вы можете использовать этот фрагмент для платежного шлюза, такого как PayUMoney.(*просто слово предупреждения WebViews не очень безопасно ,не стесняйтесь делиться мудростью и делать код лучше) )

			getSupportFragmentManager()
								.beginTransaction()
								.add(R.id.frag_root,
										UniversalWebViewFragment.newInstance(
												PAYU_MONEY_URL, false))
								.commit();

3) Display your Facebook page in the App for latest news or load your twitter page for latest tweets.
3) отображение страницы Facebook в приложении для последних новостей или загрузить страницу twitter для последних твитов.
	getSupportFragmentManager()
						.beginTransaction()
						.add(R.id.frag_root,
								UniversalWebViewFragment.newInstance(
										FACEBOOK_DEMO_URL, false)).commit();


4) It also allow you to search contents in Google in your App.Just pass searchQuery and true in arguments to load search results.as shown in code below
4) Он также позволяет искать содержимое в Google в вашем приложении.Просто передайте searchQuery и true в аргументах для загрузки результатов поиска.как показано в коде ниже

						getSupportFragmentManager()
								.beginTransaction()
								.add(R.id.frag_root,
										UniversalWebViewFragment
												.newInstance(
														((EditText) findViewById(R.id.serach_edt))
																.getText()
																.toString(),
														true)).commit();
														
Attached sample will demostarte some of above use cases :-
Прикрепленный образец будет demostarte некоторые из вышеуказанных случаев использования :-

###Android Studio Project Screenshots

![Alt text](https://github.com/hiteshsahu/Android-Universal-Web-Content-Loader/blob/master/Art/studio_youtube.png "YouTube Sample")
![Alt text](https://github.com/hiteshsahu/Android-Universal-Web-Content-Loader/blob/master/Art/studio_fb.png "Facebool Example")
![Alt text](https://github.com/hiteshsahu/Android-Universal-Web-Content-Loader/blob/master/Art/studio_payu.png "payment Gateway Example")
![Alt text](https://github.com/hiteshsahu/Android-Universal-Web-Content-Loader/blob/master/Art/studio_google.png "payment Google Search Example")
![Alt text](https://github.com/hiteshsahu/Android-Universal-Web-Content-Loader/blob/master/Art/studio_oofline.png "Offline Example")

###Eclipse Project Screenshots

Eclipse project  is depricated



Copyright 2015 Hitesh Kumar Sahu

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
 
