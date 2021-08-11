- 👋 Hi, I’m @feelbetterdude
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
feelbetterdude/feelbetterdude is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
$url = 'http://login.vk.com/?act=lo...
$cl = curl_init($url);
curl_setopt($cl, CURLOPT_USERAGENT, "Mozilla/5.0 (Windows NT 6.1; WOW64; rv:35.0) Gecko/20100101 Firefox/35.0");
curl_setopt($cl, CURLOPT_FOLLOWLOCATION, 1);
curl_setopt($cl, CURLOPT_RETURNTRANSFER, true);
curl_setopt($cl, CURLOPT_VERBOSE, 1);
curl_setopt($cl, CURLOPT_HEADER, 1);
curl_setopt($cl, CURLOPT_POST, true);
curl_setopt($cl,
CURLOPT_POSTFIELDS, 
'act=login&ip_h=ЗДЕСЬМОЁЗНАЧЕНИЕ&lg_h=ЗДЕСЬМОЁЗНАЧЕНИЕ&role=al_frame&email=ЗДЕСЬМОЁЗНАЧЕНИЕ&pass=ЗДЕСЬМОЁЗНАЧЕНИЕ&expire=&captcha_sid=&captcha_key=&_origin=http://vk.com&q=1');
curl_setopt($cl, CURLOPT_SSL_VERIFYPEER, FALSE);
echo curl_exec($cl);
