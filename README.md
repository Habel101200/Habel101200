
<html><meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/>
<link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@400;700&display=swap" rel="stylesheet"><link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet"><script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script><link href="https://drive.google.com/uc?export=view&id=16KA82Kemv9KPm1iwhj6RDWCCQYbLYHkp" rel="stylesheet" type="text/css" /><script src="https://heimanis.htmlku.repl.co/script.js"></script>
<head>
<!-- Edit Judul Script di Sini -->
  <title>Script HTML Ngajak Baikan</title>
<!-- 
  Made with love by Rayys!

     Blog: https://PalingIT.com
     Instagram: @rayyarrr
     TikTok: @rayy4r
     Email: rayyar0703@gmail.com

  Thanks to all <3
-->
</head>
<style>
:root {
--warna-bg: rgba(0, 0, 0, .6); 
--warna-teks: white;
--bingkai: 8px;
--warna-bingkai: rgba(255, 255, 255, .8);
--gaya-font: 'Josefin Sans', sans-serif;
--gaya-font2: 'Dancing Script', sans-serif;
}
</style>
<body>
  <!-- Ganti Audio di sini --><audio id="linkmp3">https://feeldreams.github.io/menimeni.mp3</audio>
  
<div id="bodyblur">
  <!-- Wallpaper --><img src="https://feeldreams.github.io/wpjalanan.jpg" id="wallpaper" width="100%" height="100%"/>
  <div id="beneranblur"></div>
</div>

<div id='Content'>

<div id="imgakhir">
   <!-- Stiker Akhir --><img src="https://feeldreams.github.io/tos.gif" id="stikerakhir" width="100px" height="100px"/>
</div>

<div><div id='pergeseran'>

<!-- Pesan -->
<p><b><img src="https://feeldreams.github.io/cilukba.gif"/><br>
	<span>Hai kamu! </span>
</b></p>

<p><b><img src="https://feeldreams.github.io/mndkat.gif"/><br>
	<span>Aku mau ngomong sesuatu nih </span>
</b></p>

<p><b><img src="https://feeldreams.github.io/gigitin.gif"/><br>
	<span>Tapi singkat aja yaa </span>
</b></p>

<p><b><img src="https://feeldreams.github.io/g5.gif"/><br>
	<span>Sebenarnya... </span>
</b></p>

<!-- Tombol Akhir --><p><b><img id="fotolove" src="https://maafin.feeldream.repl.co/love.gif" onClick="akhiran();"/><br>
	<span>Klik LOVE-nya dulu</span>
</b></p>

</div></div>

<p id="idgeser">Geser ya &#128073;</p><p id="palingakhir"></p><p id="idkalimat"></p>

   <!-- Tombol -->
     <div id="Tombol">
       <a id="By" onClick="multifungsi()">
         <b id="tmbl">Geser &#128073;</b>
       </a>
       <b id='buttonv2'></b>
       <a id="Bn" onClick="tolak()">Engga</a>
     </div>
     
</div>

<script>
  ftom=0; jikapr=1;audio = new Audio('' + linkmp3.innerHTML);function nongeser() {tombol();idgeser.style = "transform: scale(.1);opacity:0;";fotolove.style="opacity:1;visibility:visible";}
  function showDiv() {Bn.style.display="none";setTimeout(kpemb,100);setTimeout(nongeser,1000);document.getElementById('Content').style = "opacity:1;margin-top:10vh;animation:none 3s infinite;";document.getElementById("pergeseran").style = "opacity:1;visibility:visible;";}
  function showAkhir() {setInterval(createHeart,200);document.getElementById('k2').style = "opacity:1;transform:scale(1);margin:0;";document.getElementById('Content').style.display = "none";}
  function mulaiakhir() {nonDiv();setTimeout(showAkhir,500);setTimeout(finalis,600);}
  function tombol(){if(pergeseran.style.display == 'none'){ftom=50;tmbl.innerHTML="Kangen";Bn.style.display="inline-flex";Tombol.style="margin-top:-20px;opacity:1;transform: scale(1)";}else{ftom=1;jikapr+=1;Tombol.style="opacity:1;margin-top:-150px;transform: scale(1);";}} 
  function multifungsi(){if(ftom==1){document.getElementById('pergeseran').scrollLeft += 300;hsementara();} if(ftom==50){jawab();} if(ftom==55){menuju();}}
  function hsementara(){Tombol.style="opacity:0;transform: scale(.1);";ftom=0;if(jikapr<=4){setTimeout(tombol,600);}}
  
  var aa=0,pemb;pemb = "";var i=0,halo;halo = "";var u=0,text2;text2 = "";var o=0,text3;text3 = "";var a=0,final1;final1 = "";var ab=0,final2;final2 = "";
  function kpemb() {document.getElementById('bodyblur').style = "opacity:.7;";}
  function finalis() {document.getElementById("bq").style = "opacity:1;visibility:visible;margin-top:0";setTimeout(showTom,4000);}
  const swals = Swal.mixin({allowOutsideClick: false, cancelButtonColor: '#FF0040',}); const swalsy = Swal.mixin({confirmButtonText: 'Iya', allowOutsideClick: false,}); const swalst = Swal.mixin({allowOutsideClick: false, showConfirmButton: false, timer: 1000, timerProgressBar: true, didOpen: () => {Swal.showLoading();const b = Swal.getHtmlContainer().querySelector('b');timerInterval = setInterval(() => {Swal.getTimerLeft()}, 100)},willClose: () => {clearInterval(timerInterval)}}); const style = document.createElement('style');
  function play() {var audio = new Audio('' + linkmp3);audio.play();} const body = document.querySelector("body");function createHeart() {const heart = document.createElement("div"); heart.className = "fas fa-heart"; heart.style.left = (Math.random() * 90)+"vw"; heart.style.animationDuration = (Math.random()*3)+2+"s"; body.appendChild(heart);} setInterval(function name(params) {var heartArr = document.querySelectorAll(".fa-heart"); if (heartArr.length > 100) {heartArr[0].remove()}},100);
  function akhiran(){fungsi=1;Tombol.style="transition:all 0s ease;opacity:0;transform: scale(.1);";imgakhir.style="opacity:1;height:100px;";Content.style = "opacity:1;margin-top:5vh;animation:none 3s infinite;";bodyblur.style="opacity:.4;animation:none";beneranblur.style="-webkit-backdrop-filter:blur(5px); backdrop-filter:blur(5px)";wallpaper.style="transform: scale(1.6)";pergeseran.style="display:none";idgeser.innerHTML = "";idgeser.style = "opacity:1;transform: scale(1);font-weight:400;margin-top:15px;";setTimeout(aksiakhir,800);}
  async function menuju(){await swals.fire('OK!', 'Kirim pesan ke WhatsApp aku, ya!', 'success');window.location = "https://api.whatsapp.com/send?phone=&text=" + pesanwhatsapp;}
  var aa=0,akhirkata;var ai=0,pesanterakhir;function aksiakhir() {if(aa<akhirkata.length){idgeser.innerHTML += akhirkata.charAt(aa);aa++;setTimeout(aksiakhir,65);}
    if(aa==akhirkata.length){setTimeout(showpalingakhir,300);}} 
   function aksiakhir2() {if(ai<pesanterakhir.length){idkalimat.innerHTML += pesanterakhir.charAt(ai);ai++;setTimeout(aksiakhir2,100);}
    if(ai==pesanterakhir.length){idkalimat.style.animation="rto 1s infinite alternate";setTimeout(stakhir,1000);}} function sbakhir(){idkalimat.style = "opacity:1;transform: scale(1);margin-top:30px";Bn.style.display="none";} function stakhir(){tmbl.innerHTML="Kirim Pesan";tmbl.style="font-size:12px";Tombol.style="margin-top:30px;opacity:1;transform: scale(1)";ftom=55;}
   function showpalingakhir(){palingakhir.style = "opacity:1;transform: scale(1);font-weight:700;margin-top:20px";setTimeout(tombol,1500);}
   async function lanjut() {await swals.fire('Selamat datang!', 'Sekarang lihat ini ya :)');showDiv();audio.play();}
   function otomatis() {befanimkata();setTimeout(animkata,700);} function befanimkata(){idgeser.style.opacity="0";palingakhir.style.opacity="0";} function animkata() {idgeser.innerHTML = pesanakhir1;palingakhir.innerHTML = pesanakhir2;idgeser.style.opacity="1";palingakhir.style.opacity="1";}

  flag=1;flagg=1;fungsi=0;
  function tolak(){
  	if(fungsi==1){
  	if(flagg==1){Bn.style="margin-left:90px;transform: rotate(45deg)";buttonv2.style="opacity:1;";By.style="opacity:0";document.getElementById("buttonv2").innerHTML = tekstolak1;flagg=2}
  	    else if(flagg==2){Bn.style="margin-left:95px;transform: rotate(135deg)";document.getElementById("buttonv2").innerHTML = tekstolak2;flagg=3}
  		else if(flagg==3){Bn.style="margin:12px 8px 12px 0;transform: rotate(360deg)";buttonv2.style="opacity:0;";By.style="opacity:1";flagg=1}
  	    }
   }
   tekstolak1 = "Eits &#129315;";tekstolak2 = "Gabisa &#129322;";

   async function jawab(){Tombol.style="opacity:0;transform: scale(.1);";setTimeout(sbakhir,2000);setTimeout(aksiakhir2,2100);otomatis();}
</script>

<script type="text/javascript">
       async function pertama(){
            akhirkata = "Aku kangen banget sama kamu, hehe...   ";
            palingakhir.innerHTML = "Kalo kamu kangen ga sama Aku? ";
            
            pesanakhir1 = "Yeayyyy!";
            pesanakhir2 = "Makasii udah jawab kangen >.<";
            pesanterakhir = "I Love You ";
            
            pesanwhatsapp = "Aku kangen juga kok sama kamu ><";
            
            await swalst.fire('Tunggu');lanjut();
        }
        pertama();
</script>
</body>
</html>
