# MBDeveloperProject

PROJE: Mercedes Benz Developers, / Connected Vehicle API'sini kullanan bir Uygulama

TANIM: Mercedes Benz (MB Developers)'in sagladagi / Connected Vehicle API'sinden bilgi çekmek suretiyle
sanal aracimizin kapilarini kilitlemek/kilidini açmak ve kapilarin genel kilit ve açik/kapali olma durumlarini 
göstermek gibi operasyonlari yapabilen bir uygulama.

KULLANILAN TEKNOLOJILER VE SEBEPLERI:
	1-) Angular Framework, zira bunun bir Web uygulamasi olmasi kullanim kolayligi ve tasinabilirlik açisindan en mantikli
seçim olarak gözüküyordu, ve web uygulamasi gelistirmek için Angular framework'ün (ve CLI) oldukça uygun ve tasarimi kolay bir teknoloji oldugu söylenebilir.

	2-) Angular IDE: Gerekli componentlarin (table, button, etc.) entegrasyonu ve kullanicinin isini kolaylastiran arayüzü ile
oldukçta kullanisli ve gelistiricinin isini kolaylastiran bir tool

	3-) JavaScript: Backend ile web üzerinden konusmak ve real-time client-side HTML Component güncelleme gibi olaylari basariyla
gerçeklestiren, ve syntax olarak da tercih ettigim bir dil.

	4-) Node JS: Web uygulamamızı serve etmek (yahut ayakta tutmak) için web sunucu olarak kullandığımız, JS bazlı bir
teknoloji, özellikle bunu kullanma sebebimiz ise hem Angular ile, hem de uygulamayı geliştirmek için tercih ettiğimiz dille
(JavaScript) iyi bir sinerjisinin olması, ve Angular'da kurulması gereken birçok paketi kuran ana modülün (npm) bu teknolojinin
belkemiği olması

PROJENIN ANA YAPISI: Proje bir web uygulamasi olup, esas olarak 2 ana modülden olusmakta:
1- HTML kismi, burada tasarladigimiz table ve buttonlarin fontunu, seklini, yerlerini ayarliyoruz ve 2. modüldeki (TS modülü)
kullandigimiz variablelari bu tablo ve buttonlara bind ediyoruz (yani bagliyoruz)

2- TS (TypeScript) kismi, bu kisim Angular frameworküne özel bir structure, burada API üzerinden token kullanarak data çekme,
araç kilitleme/kilit açma gibi islemleri gerçeklestiriyoruz. Bu islemler HTTP üzerinden (ve custom headerlar) ile oluyor,
bunun için de HttpClient modülünü kullaniyoruz. 
