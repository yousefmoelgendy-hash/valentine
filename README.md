<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Cairo&family=Pacifico&display=swap" rel="stylesheet">

<title>Happy Valentine ❤️</title>

<style>

body{
margin:0;
font-family:Cairo, sans-serif;
background:linear-gradient(180deg,#ff4d6d,#ff8fa3);
min-height:100vh;
display:flex;
align-items:center;
justify-content:center;
}

/* قلوب خفيفة في الخلفية */
body::before{
content:"❤️ ❤️ ❤️ ❤️ ❤️ ❤️ ❤️";
position:fixed;
font-size:42px;
opacity:.12;
animation:float 25s linear infinite;
}

@keyframes float{
from{transform:translateY(100vh)}
to{transform:translateY(-120vh)}
}

.card{
background:white;
width:90%;
max-width:500px;
border-radius:30px;
padding:30px 25px 35px;
text-align:center;
box-shadow:0 20px 40px rgba(0,0,0,.25);
animation:fade .8s ease;
max-height:85vh;
overflow:auto;
}

@keyframes fade{
from{opacity:0;transform:translateY(20px)}
to{opacity:1;transform:translateY(0)}
}

.title{
font-family:Pacifico,cursive;
color:#ff4d6d;
font-size:36px;
margin-bottom:10px;
}

.from{
color:#c9184a;
font-weight:bold;
font-size:18px;
margin-top:-8px;
margin-bottom:5px;
}

input{
width:85%;
padding:14px;
border-radius:30px;
border:2px solid #ffd1dc;
outline:none;
font-size:16px;
margin-top:15px;
}

button{
width:90%;
padding:15px;
border-radius:30px;
border:none;
background:#ff4d6d;
color:white;
font-size:18px;
margin-top:20px;
cursor:pointer;
transition:.3s;
}

button:hover{transform:scale(1.05)}

.message{
display:none;
color:#c9184a;
line-height:2;
font-size:18px;
text-align:right;
}

.heart{font-size:55px;margin-bottom:10px}

</style>
</head>

<body>

<!-- صفحة الباسورد -->
<div class="card" id="login">
<div class="heart">❤️</div>

<div class="title">Happy Valentine</div>
<div class="from">From Youssef to Mayer ❤️</div>

<p>اكتبي الباس ي اغلي حد في دنيتي</p>

<input type="password" id="password" placeholder="Password">
<button onclick="checkPassword()">فتح الرسالة</button>
</div>

<!-- الرسالة -->
<div class="card message" id="msg">
<div class="heart">💌</div>

<p>

كل عيد حب وانت احب واحده في الدنيا دي لقلبي وكل سنه كد وانتي اجمل واحده في الدنيا في عيوني رغم احنا مبقناش زي الاول ما بعض بس مهما كان معروف ان ميار دي اكتر واحده يوسف حبها في دنيته وانتي بنوتي ونور عيني الي بموت فيها والله ❤️<br><br>

علاقتنا كانت الفتره الاخيره ايوه م احسن حاجه بس كفايه ان احنا عملنا اجمل ذكريات في بعض مكنتش اتمني نكون ذكري في حياه بعض واحتمال هنكون ذكري علشان كنتي قايله هتبعدي بس ان شاء الله ربنا هيقربك ليا ويرب تفضلي محافظه ع نفسك في غيابي وان شاء الله لو لينا خير في بعض يرب يرجعنا احسن من الاول ويبعد عننا اي عين واي شخص نفسه علاقتنا تنتهي واحسن happy Valentine day وان شاء الله تالت واحد واحنا مع بعض وان شاء الله رمضان كمان هيكون التالت لينا وان شاء الله ربنا يكتب لينا في حياه بعض <br><br>

انا متردد فشخ ان ابعتلك الكلام دا وحاسس ان ردت فعلك هتكون م كويسه بس ان شاء الله خير <br><br>

وتاني مره اجمل واحلي عيد حب ي بنوتي🫀🫵🏻

</p>

</div>

<script>

const correctPassword="262024"; // غيره للباسورد اللي انت عايزه

function checkPassword(){
const input=document.getElementById("password").value;

if(input===correctPassword){
document.getElementById("login").style.display="none";
document.getElementById("msg").style.display="block";
}else{
alert("اول مره نمسك ايد بعض افتكريي");
}
}

</script>

</body>
</html>
