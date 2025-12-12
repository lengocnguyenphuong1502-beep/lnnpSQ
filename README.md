<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bài 17 – Nhóm 4 Lớp 12 Anh</title>
<style>
body {
  font-family: 'Poppins', sans-serif;
  background: #FFF4B7 url('https://www.transparenttextures.com/patterns/cubes.png');
  margin: 0;
}
header {
  background: linear-gradient(135deg, #000B58, #003161);
  color: white;
  text-align: center;
  padding: 40px 20px;
}
h1 {margin: 0; font-size: 36px;}
h2 {color: #000B58;}
section {
  background: white;
  margin: 20px auto;
  width: 90%;
  max-width: 900px;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 6px 15px rgba(0,0,0,0.15);
  transition: 0.3s;
}
section:hover {transform: translateY(-5px);}
.details {display: none; margin-top: 15px; opacity: 0; transition: .2s;}
button {
  background: #006A67;
  color: white;
  padding: 10px 16px;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  transition: 0.3s;
  font-weight: 600;
}
button:hover {background: #003161; transform: scale(1.05);} 
fieldset {margin-bottom: 15px; border-radius: 8px;}
iframe {border-radius: 12px; border: 2px solid #003161;}
nav.topmenu {
  width:100%;
  background:#003161cc;
  backdrop-filter: blur(4px);
  position:fixed;
  top:0;
  left:0;
  padding:12px 25px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  z-index:100;
}
nav.topmenu a {
  color:white;
  text-decoration:none;
  font-weight:600;
  margin-right:18px;
  transition:.25s;
}
nav.topmenu a:hover {color:#FFD93D; transform: translateY(-2px);} 
</style>
<script>
function toggle(id){
  var box=document.getElementById(id);
  if(box.style.display==='block'){
    box.style.opacity=0;
    setTimeout(()=>{ box.style.display='none'; },200);
  } else {
    box.style.display='block';
    setTimeout(()=>{ box.style.opacity=1; },10);
  }
}
function bounceScroll(targetID){
  const el = document.getElementById(targetID);
  if (!el) return;
  el.scrollIntoView({ behavior: 'smooth', block: 'start' });
  setTimeout(() => {
    el.style.transition = 'transform 0.45s cubic-bezier(0.30, 2.0, 0.45, 1), box-shadow 0.45s ease';
    el.style.transform = 'scale(1.18)';
    el.style.boxShadow = '0 0 45px #ffe47a, 0 0 75px #FFD93D';
    setTimeout(() => {
      el.style.transform = 'scale(1.06)';
      el.style.boxShadow = '0 0 25px #FFD93D';
      setTimeout(() => {
        el.style.transform = 'scale(1)';
        el.style.boxShadow = '0 0 0 transparent';
      }, 220);
    }, 420);
  }, 500);
}
</script>
</head>
<body>
<nav class="topmenu">
  <div>
    <a href="https://daisubinta.github.io/Nhom4tin12anh.github.io/">⬅ Quay lại</a>
    <a href="javascript:bounceScroll('luyentap-section')">Luyện tập</a>
    <a href="javascript:bounceScroll('vd1-section')">Vận dụng 1</a>
    <a href="javascript:bounceScroll('vd2-section')">Vận dụng 2</a>
  </div>
</nav>
<br><br><br>
<header>
  <h1>Nhóm 4 – Lớp 12 Anh</h1>
  <h2 style="font-size:52px; color:#FFD93D; text-shadow:0 5px 14px rgba(0,0,0,0.55); letter-spacing:2px;">BÀI 17: CÁC MỨC ƯU TIÊN CỦA BỘ CHỌN</h2>
</header>

<!-- =================== BÀI 17 =================== -->
<section id="luyentap-section">
<h2>1. Luyện tập</h2>
<button onclick="toggle('luyentap')">Hiện / Ẩn bài làm</button>
<div id="luyentap" class="details">
<p><b>Đề bài:</b> Phân biệt hai bộ chọn CSS sau.</p>
<h3>Luyện tập 1 trang 101</h3>
<p><b>Giải thích sự khác nhau giữa hai định dạng sau:</b></p>
<p><code>#p123 + p</code> và <code>h2#p123 + p</code></p>
<p><b>Lời giải:</b></p>
<ul>
<li><b>#p123 + p</b> chọn phần tử &lt;p&gt; đứng liền sau phần tử có ID <b>p123</b>.</li>
<li><b>h2#p123 + p</b> chọn phần tử &lt;p&gt; đứng liền sau phần tử &lt;h2&gt; có ID <b>p123</b>.</li>
</ul>
</div>
</section>

<section id="vd1-section">
<h2>2. Luyện tập 2</h2>
<button onclick="toggle('vd1')">Hiện / Ẩn bài làm</button>
<div id="vd1" class="details">
<p><b>Đề bài:</b> Viết CSS để định dạng tên riêng theo yêu cầu.</p>
<h3>Định dạng tên riêng bằng CSS</h3>
<p>CSS cần dùng:</p>
<pre>.name {
  font-style: italic;
  border: 1px solid #000;
  padding: 2px;
  display: inline-block;
}</pre>
</div>
</section>

<section id="vd2-section">
<h2>3. Vận dụng 1 & 2</h2>
<button onclick="toggle('vd2')">Hiện / Ẩn bài làm</button>
<div id="vd2" class="details">
<p><b>Đề bài:</b> Liệt kê và giải thích một số pseudo-class và pseudo-element.</p>
<h3>Vận dụng 1 – Một số pseudo-class</h3>
<ul>
<li><b>:hover</b> – kích hoạt khi di chuột.</li>
<li><b>:active</b> – kích hoạt khi nhấn giữ.</li>
<li><b>:focus</b> – khi phần tử được chọn.</li>
<li><b>:nth-child()</b> – chọn phần tử theo vị trí.</li>
</ul>
<h3>Vận dụng 2 – Một số pseudo-element</h3>
<ul>
<li><b>::before</b> – thêm nội dung trước.</li>
<li><b>::after</b> – thêm nội dung sau.</li>
<li><b>::first-line</b> – định dạng dòng đầu tiên.</li>
</ul>
</div>
</section>

</body>
</html>
