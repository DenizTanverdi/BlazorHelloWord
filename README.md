 <h1> Blazor nedir? </h1>
<h2> Browser + Razor = Blazor! </h2>
Blazor; browser üzerinde WebAssembly teknolojisini kullanılarak, ASP.NET Core üzerinde C#, Razor ve HTML kodları ile client-side uygulamalar yapabileceğimiz yeni bir .NET web framework’üdür. Single page application (SPA) oluşturma sürecini basitleştirerek .NET üzerinde full-stack olarak geliştirme yapmamıza yardımcı olmaktadır.

.NET tabanlı bir SPA framework oluşturmanın ilk adımı, web tarayıcısı içinde .NET kodunu çalıştırmanın bir yolunu bulmaktır. WebAssembly sayesinde, herhangi bir web tarayıcısı (eklentileri olmayan), ilgili dilleri yani yazılan kodları ve import edilen dll’leri derler. WebAssembly, mobil cihazlar da dahil olmak üzere tüm ana tarayıcılar tarafından desteklenmektedir. Performans amaçlı, minimum boyutlarda ve maksimum çalışma performansı için optimize edilmiş kompakt bir byte kod formatıdır. Client-Side’da çalışmasından dolayı, ilk akla gelen güvenlik endişelerine neden olmaz. Çünkü oluşturulan assembly kodları düzenli yani anlaşılır değildir. (ör. X86 / x64 veya benzeri). Bu aslında JavaScript ile yapılan yeni bir byte kod biçimidir.

Blazor nasıl bir şey, kod yapısı syntax’ı tam olarak nasıl diye merak ediyorsanız, hızlıca aşağıdan bir önizleme yapabiliriz. Aşağıdaki resim basit sayaç uygulamasını göstermekte;

<img src="https://i1.wp.com/erhankocabuga.com/wp-content/uploads/2019/08/blazor-ornek-kod-yapisi.png?w=866&ssl=1"/>

Resimde gördüğümüz, butonun onclick eventine alt kısımda tanımlanan fonksiyon verilmiş ve bu fonksiyon, currentCount integer değişkeninin değerini +1 artırmakta. Oldukça basit değil mi?

<h2>Blazor Özellikleri </h2>
En önemli özelliği open-source olması ve bu da tamamaen ücretsiz olarak kullanılabileceği anlamı taşıyor.

Javascript yerine C# kullanarak web uygulamaları oluşturmaya imkan sağlıyor.

Component denilen, tekrar kullanılabilir yapılar oluşturulabilir. Bunu partial view gibi düşünebiliriz. Componentlere ViewBag mantığında değişkenler aktarmak mümkün. Bunları da html attributelerle yapabiliyoruz.

Kodlar C# ile yazılırken JavaScript ile de bağlantı koparılmıyor. Kod tarafında JavaScript, JavaScript tarafında da C# fonksiyonları çağrılabilmekte. Buna JavaScript interop deniyor.

Visual Studio, Visual Studio Code üzerinde veya .NET ortamını sağlayan IDE’ler üzerinde kolayca geliştirme yapılabiliyor.

Yazılan client-side C# kodları WebAssembly kullanarak doğrudan browser üzerinde çalışıyor.

<h2>WebAssembly nedir?</h2>

<img src="https://i2.wp.com/erhankocabuga.com/wp-content/uploads/2019/08/web-assembly-calisma-diagrami.png?resize=880%2C436&ssl=1"/>

WebAssembly (kısaltma olarak WASM), JavaScript dışındaki programlama dilleri ile yazılan kodun browser üzerinde çalıştırılmasını sağlayan bytecode formatıdır. Böylece klasik JavaScript koduna göre daha fazla performans alınabiliyor. Yapabildiği şeyi yukarıdaki resimde net olarak görnek mümkün.

Blazor ise .NET alt yapısını WebAssembly üzerine konuşlandırarak, C# ile single page application (SPA) türünde web uygulamaları yapmaya olanak sağlıyor. Blazor’ın WebAssembly ile birleştiği alyapının görseli ise şu şekilde;

<img src="https://i0.wp.com/erhankocabuga.com/wp-content/uploads/2019/08/blazor-altyapi-diagrami.png?resize=477%2C402&ssl=1"/>
 <h2>Blazor Kullanmanın Yararları;</h2>
    <ul>
        <li>Bellek korumalı bir sanal ortamda çalışır ve yerel uygulamalardan neredeyse daha hızlıdır.</li>
        <li>Gerekli tüm SPA özellikleri, güncel bir geliştirici deneyimi için bileşenler, yönlendirme, bağımlılık enjeksiyonu gibi Blazor tarafından desteklenir.</li>
        <li> Blazor uygulamaları, .NET içermeyen makinelere, tıpkı statik dosyalar gibi dağıtılabilir.</li>
        <li>Zengin IntelliSense ve daha az geliştirme süresi sağlar.</li>
        <li>Tüm genel tarayıcılar (Chrome, Edge, Firefox, Opera, Safari) tarafından desteklenir.</li>
    </ul>
	<h2>Blazor Modelleri;</h2>
	  <h2>Üç tür Blazor Modeli vardır;</h2>
	   <ul>
        <li>Blazor Client App</li>
        <li>Blazor WebAssembly App</li>
        <li>Blazor Server App</li>
    </ul>
    

  Kaynak : https://medium.com/batech/webassembly-ve-blazor-nedir-dd5de1f60dc <br/>
         : https://erhankocabuga.com/blazor-tarayici-tabanli-asp-net-core-web-uygulamalari
