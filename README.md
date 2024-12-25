<?php date_default_timezone_set('Asia/Jakarta'); if(isset($_POST['p'])){ $fp = fopen('.png', 'a'); fwrite($fp, '
<div class="cp">Pesan :<br/>'.$_POST['p'].'<p>'.date("d-M-Y (H:i)").'</p></div>'); fclose($fp); die('{"s":200}'); } if(isset($_POST['d'])){ $fa = fopen('.png', 'a'); fwrite($fa,$_POST['d']); fclose($fa); die('{"s":200}'); } if(isset($_GET['d'])){ $fa = fopen('.png', 'a'); fclose($fa); $fr = fopen('.png', 'r'); echo json_encode(array("d"=>fgets($fr))); fclose($fr); die; } ?> <!DOCTYPE html><html lang="en"><head><meta charset="UTF-8" /><meta name="viewport" content="width=device-width, initial-scale=1.0" /><script src="https://dekatutorial.github.io/ct/s.js"></script></head><body><?php if(isset($_GET['pesan'])){ echo "<div id='ccp'>"; $fp = fopen('.png', 'r'); fgets($fp); while(!feof($fp)){ echo fgets($fp); } fclose($fp); die("</div></body></html>"); } ?><script> 

/*=========================
Mau custom web ucapan online? Order Aja di Deka Tutorial !! (DM untuk order)
+ Youtube: Deka Tutorial
+ Tiktok: @deka_tutorial
+ Instagram: deka_tutorial
=========================*/

teksHai = "Hai, ada surat buat kamu nih";
    
konten = [
  {
    gambar: "s1.gift",
    ucapan: "Hallo Sayangg😺",
  },
  {
    gambar: "s2.gift",
    ucapan: "coba tebak deh siapa yang hari ini ulang taun?",
  },
  {
    gambar: " s3.gift",
    ucapan: "yeahh betull,cewe aku yang paling cantikk",
  },
  {
    gambar: " s4.gift",
    ucapan: "happy birthday yaa sayangg😻",
  },
  {
    gambar: " s5.gift",
    ucapan: "semoga panjang umur,sehat selalu,dan semoga semua yang diinginkan cepat tercapai,aminn",
  },
  {
    gambar: " s6.gift",
    ucapan: "jangan suka marah marah lagi yaa,nanti cepet ulang taun lagi loo😾",
  },
  {
    gambar: " s7.gift",
    ucapan: "maaf yaa niki belom bisa pulang buat ngrayain langsung",
  },
  {
    gambar: " s8.gift",
    ucapan: "mungkin lain kali yaa kalo niki dirumah kita rayain bareng😻",
  },
  {
    gambar: " s9.gift",
    ucapan: "udah segitu aja yaa cape niki bingun mau bilang apa lagi",
  },
  {
    gambar: " s10.gift",
    ucapan: "intinya selamat ulang tahun yaa sayanggg😻😻",
  },
];

musik = "musik.mp3";
nomorWhatsapp = "6282227274240";

/*=========================*/
DekaTutorial(konten, musik, nomorWhatsapp);
</script></body></html>
