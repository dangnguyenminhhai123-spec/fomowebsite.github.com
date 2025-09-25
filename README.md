<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>FOMO - Nỗi Sợ Bị Bỏ Lỡ</title>
<style>
  :root{
    --nav-bg:#0b2545;
    --accent:#123456;
    --card:#ffffff;
    --page:#f4f7fb;
    --text:#0d1b2a;
    --link-active-shadow: inset 0 -3px 0 #fff;
  }
  *{box-sizing:border-box}
  body{
    margin:0;
    font-family:"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
    background:var(--page);
    color:var(--text);
  }
  header{
    position:sticky;top:0;z-index:1000;
    background:var(--nav-bg);padding:12px 16px;
    box-shadow:0 2px 8px rgba(2,8,23,0.12);
    display:flex;align-items:center;justify-content:center;gap:28px;
  }
  .brand{color:#fff;font-weight:700;font-size:18px;margin-right:12px}
  nav{display:flex;gap:12px;align-items:center}
  .nav-link{color:#fff;text-decoration:none;padding:8px 12px;font-size:16px;border-radius:6px;cursor:pointer}
  .nav-link.active{box-shadow:var(--link-active-shadow);font-weight:600}
  .nav-link:hover{opacity:.95}
  .container{max-width:1100px;margin:28px auto;padding:0 20px}
  #home .title{font-size:60px;color:var(--accent);text-align:center;margin:10px 0 6px 0;font-weight:800}
  #home .subtitle{font-size:30px;text-align:center;margin:0 0 18px 0;color:var(--text)}
  .section-title{font-size:32px;color:var(--accent);text-align:center;margin-bottom:14px}
  .box{background:var(--card);border-radius:12px;padding:20px;margin:16px auto;max-width:900px;
       box-shadow:0 8px 20px rgba(12,34,60,0.06);border-left:6px solid var(--nav-bg)}
  .box h3{color:var(--nav-bg);margin-top:0}
  .box p,.box li{font-size:17px;line-height:1.6;color:#16364a}
  #quiz-form{max-width:900px;margin:0 auto}
  .question{background:var(--card);border-radius:10px;padding:14px 16px;margin-bottom:12px;
            box-shadow:0 6px 18px rgba(12,34,60,0.06);border-left:6px solid rgba(18,52,86,0.08)}
  .question p{margin:0 0 8px 0;font-weight:600}
  .options label{display:block;margin:6px 0;cursor:pointer}
  input[type=radio]{margin-right:10px}
  .actions{text-align:center;margin-top:14px}
  .btn{display:inline-block;background:var(--accent);color:#fff;padding:12px 22px;border-radius:10px;
       border:0;font-size:16px;cursor:pointer;box-shadow:0 8px 24px rgba(18,52,86,0.14)}
  .btn.secondary{background:#0b2545}
  .result{max-width:900px;margin:18px auto;padding:16px;border-radius:10px;background:#fff;
          box-shadow:0 8px 24px rgba(12,34,60,0.06)}
  .result h4{margin:6px 0;color:var(--accent)}
  @media(max-width:720px){
    #home .title{font-size:34px}
    .section-title{font-size:24px}
    .nav-link{font-size:14px;padding:6px 8px}
  }
</style>
</head>
<body>
<header>
  <div class="brand">FOMO - Nỗi sợ bị bỏ lỡ</div>
  <nav id="mainNav">
    <a class="nav-link active" data-target="home">Trang chủ</a>
    <a class="nav-link" data-target="gioithieu">Giới thiệu</a>
    <a class="nav-link" data-target="quiz">Khảo sát</a>
    <a class="nav-link" data-target="khampha">Khám phá</a>
    <a class="nav-link" data-target="thongke">Thống kê</a>
  </nav>
</header>
<main class="container">
  <!-- HOME -->
  <section id="home-section">
    <div id="home">
      <div class="title">FEAR OF MISSING OUT</div>
      <div class="subtitle">Nỗi sợ bị bỏ lỡ</div>
      <div class="box">
        <p>
          Trong kỷ nguyên số, nơi mỗi cú nhấp chuột có thể mở ra vô vàn thế giới, 
          nỗi sợ bị bỏ lỡ – <strong>FOMO (Fear of Missing Out)</strong> – đã trở thành một hiện tượng tâm lý phổ biến. 
          Theo nghiên cứu của <em>Przybylski và cộng sự</em> đăng trên <em>Computers in Human Behavior</em>, 
          FOMO được định nghĩa là một dạng lo âu xã hội xuất phát từ nỗi sợ rằng người khác đang có những trải nghiệm thú vị hơn bản thân mình. 
          Đây là cảm giác ám ảnh khi thấy mình bị bỏ lại phía sau trước nhịp sống sôi động của xã hội, đặc biệt trên các nền tảng mạng trực tuyến.
        </p>
        <p>
          Thực tế cho thấy, tỷ lệ người trải qua FOMO ngày càng gia tăng, nhất là ở giới trẻ. 
          Vậy, liệu bạn đã bao giờ tự hỏi: <strong>mình có đang là một trong số đó không?</strong> 
          Hãy cùng khám phá và tự đánh giá thông qua công cụ khảo sát tại trang web này của chúng mình nhé!
        </p>
      </div>
    </div>
  </section>

  <!-- GIỚI THIỆU -->
  <section id="gioithieu-section" style="display:none">
    <div class="section-title">GIỚI THIỆU VỀ TRANG WEB</div>
    <div class="box">
      <p><strong> Website này giúp học sinh:</strong>  
        <br>+ Hiểu rõ hơn về hội chứng FOMO (Fear of Missing Out – nỗi sợ bị bỏ lỡ).
        <br>+ Tham gia khảo sát mức độ FOMO để tự đánh giá bản thân.
        <br>+ Nhận biết nguyên nhân, biểu hiện và ảnh hưởng của FOMO đến cuộc sống học đường.
        <br>+ Khám phá các giải pháp, biện pháp phòng ngừa để sống tích cực, cân bằng hơn.
        <br><br>
        👉 Đây không chỉ là nơi học tập mà còn là không gian để các bạn tìm thấy sự đồng cảm và động lực thay đổi.
      </p>
    </div>
  </section>

  <!-- QUIZ -->
  <section id="quiz-section" style="display:none">
    <div class="section-title">KHẢO SÁT MỨC ĐỘ HỘI CHỨNG FOMO</div>

    <form id="quiz-form" aria-label="FOMO quiz form">
      <!-- Questions will be injected by JS -->
      <div id="questions-container"></div>

      <div class="actions">
        <button type="button" class="btn" id="submitBtn">Nộp bài</button>
        <button type="button" class="btn secondary" id="clearBtn" style="margin-left:12px">Đặt lại</button>
      </div>
    </form>

    <div id="result-area" style="display:none" class="result" aria-live="polite"></div>
  </section>

  <!-- KHÁM PHÁ -->
  <section id="khampha-section" style="display:none">
    <div class="section-title">KHÁM PHÁ</div>

    <div class="box">
      <h3>1. Nguyên nhân</h3>
      <p><strong>a) Nguyên nhân từ bản thân học sinh:</strong></p>
      <ul>
        <li>Tâm lý tuổi dậy thì: dễ so sánh bản thân với những thành tích mà bạn bè có được, nhạy cảm về mặt cảm xúc.</li>
        <li>Thiếu tự tin và bản lĩnh cá nhân: dễ bị cuốn theo đám đông, không xác định rõ giá trị bản thân.</li>
        <li>Thói quen sử dụng mạng xã hội quá mức: kiểm tra điện thoại liên tục, khó rời khỏi màn hình.</li>
        <li>Kỹ năng quản lý thời gian yếu: ưu tiên giải trí, cập nhật thông tin hơn là học tập, nghỉ ngơi.</li>
      </ul>
      <p><strong>b) Nguyên nhân từ môi trường xung quanh:</strong></p>
      <ul>
        <li>Áp lực từ bạn bè đồng trang lứa: thấy bạn bè tham gia sự kiện, trò chơi, hoạt động mới mà mình bỏ lỡ.</li>
        <li>Ảnh hưởng từ mạng xã hội: hình ảnh "lung linh", thông tin liên tục khiến học sinh cảm thấy mình bị bỏ lại.</li>
        <li>Gia đình ít quan tâm, định hướng: học sinh thiếu sự chia sẻ, dễ tìm niềm vui ở bên ngoài.</li>
        <li>Xã hội đề cao “thành tích” và “trải nghiệm”: khiến các em cho rằng phải tham gia mọi thứ mới không thua kém.</li>
      </ul>
    </div>

    <div class="box">
      <h3>2. Biểu hiện</h3>
      <ul>
        <li>Luôn kiểm tra tin nhắn, mạng xã hội liên tục để không bỏ lỡ thông tin.</li>
        <li>Cảm thấy lo lắng, bồn chồn khi không được tham gia cùng bạn bè.</li>
        <li>Dễ so sánh bản thân, sinh ra tự ti hoặc ghen tị.</li>
        <li>Bỏ bê học tập, nhiệm vụ để tham gia nhiều hoạt động không cần thiết.</li>
      </ul>
    </div>

    <div class="box">
      <h3>3. Biện pháp khắc phục dành cho học sinh mắc hội chứng FOMO</h3>
      <ul>
        <li>Xây dựng thói quen sử dụng mạng xã hội khoa học: đặt giới hạn thời gian online.</li>
        <li>Tăng cường sự tự tin: tham gia hoạt động thể thao, câu lạc bộ để khẳng định bản thân.</li>
        <li>Chia sẻ với gia đình, thầy cô, bạn bè: tìm sự đồng hành và hỗ trợ tinh thần.</li>
        <li>Rèn kỹ năng quản lý thời gian: phân bổ hợp lý giữa học tập, nghỉ ngơi, giải trí.</li>
      </ul>
    </div>

    <div class="box">
      <h3>4. Biện pháp phòng ngừa hội chứng FOMO cho học sinh</h3>
      <ul>
        <li>Tạo thói quen sống lành mạnh: ưu tiên hoạt động ngoài trời, giao tiếp trực tiếp thay vì theo dõi các trang mạng xã hội.</li>
        <li>Giáo dục kỹ năng sống và quản lý cảm xúc: giúp học sinh biết cách cân bằng, không lệ thuộc vào người khác.</li>
        <li>Gia đình quan tâm, định hướng thường xuyên: xây dựng môi trường gần gũi, lắng nghe con cái, giáo dục con cách điều chỉnh cảm xúc, lối suy nghĩ tuổi dậy thì.</li>
        <li>Nhà trường tổ chức hoạt động ngoại khóa tích cực giúp học sinh hiểu hơn về các vấn đề tâm lí thường gặp trong học đường, mang lại bầu không khí học tập, vui chơi khỏe mạnh, trong sáng.</li>
      </ul>
    </div>
  </section>
  <section id="thongke-section" style="display:none">
    <div class="section-title">TỔNG SỐ NGƯỜI THAM GIA KHẢO SÁT VÀ SỐ LIỆU THỐNG KÊ KẾT QUẢ KHẢO SÁT </div>
    <div class="box">
    <h3>Số lượt người đã vào trang web:</h3>
    <div id="visit-count" style="font-size:22px;color:#0b2545;margin-top:10px"></div>
    <h3>Số lượt người đã tham gia khảo sát:</h3>
    <div id="participant-count" style="font-size:22px;color:#123456;margin-top:10px"></div>
    <h3>Kết quả trung bình khảo sát (biểu đồ):</h3>
    <canvas id="pieChart" width="320" height="320" style="margin:20px auto;display:block;"></canvas>
    </div>
  
      
</main>
<script>
/* -----------------------
   Navigation: show/hide sections
   ----------------------- */
const navLinks = document.querySelectorAll('.nav-link');
const sections = {
  home: document.getElementById('home-section'),
  gioithieu: document.getElementById('gioithieu-section'),
  quiz: document.getElementById('quiz-section'),
  khampha: document.getElementById('khampha-section')
  ,thongke: document.getElementById('thongke-section')
 
  
};

function showSectionByKey(key){
  // hide all
  Object.values(sections).forEach(s => s.style.display = 'none');
  // show requested
  if(sections[key]) sections[key].style.display = 'block';
  // nav active
  navLinks.forEach(a => a.classList.remove('active'));
  const active = Array.from(navLinks).find(a => a.dataset.target === key);
  if(active) active.classList.add('active');
  // scroll - ensure header offset
  const top = (sections[key] || sections.home).offsetTop - (document.querySelector('header').offsetHeight + 8);
  window.scrollTo({ top, behavior: 'smooth' });
}

// attach nav events
navLinks.forEach(a=>{
  a.addEventListener('click', e=>{
    const key = a.dataset.target;
    showSectionByKey(key);
  });
});

// default show home
showSectionByKey('home');

/* -----------------------
   Quiz data (30 câu + 4 options)
   ----------------------- */
const quizQuestions = [
  { q: "1. Khi không thể tham gia một buổi tụ tập bạn bè, bạn thường cảm thấy:", o:[
    "A. Bình thường, không bận tâm",
    "B. Hơi tiếc nhưng nhanh quên",
    "C. Buồn bã, lo sợ bị bỏ rơi",
    "D. Rất khó chịu, không yên lòng"
  ]},
  { q: "2. Mỗi ngày, bạn kiểm tra mạng xã hội bao nhiêu lần?", o:[
    "A. Ít hơn 5 lần",
    "B. Khoảng 5–10 lần",
    "C. Hơn 10 lần",
    "D. Gần như liên tục"
  ]},
  { q: "3. Trước khi đi ngủ, bạn thường:", o:[
    "A. Tắt điện thoại sớm",
    "B. Chỉ lướt mạng một chút rồi ngủ",
    "C. Cứ lướt mạng đến khi mệt mới ngủ",
    "D. Thường thức khuya vì sợ bỏ lỡ tin tức"
  ]},
  { q: "4. Khi thấy bạn bè đăng ảnh đi chơi mà không có bạn, cảm giác thường đến đầu tiên là:", o:[
    "A. Bình thường",
    "B. Thấy tiếc nhẹ",
    "C. Thấy buồn và ghen tị",
    "D. Cảm giác hụt hẫng, lo lắng bị bỏ rơi"
  ]},
  { q: "5. Khi nhóm chat đang bàn sôi nổi về một sự kiện bạn chưa nghe đến, bạn sẽ:", o:[
    "A. Không quan tâm",
    "B. Đọc lướt cho biết",
    "C. Lập tức hỏi chi tiết để tham gia",
    "D. Lo lắng vì sợ mình là người duy nhất bỏ lỡ"
  ]},
  { q: "6. Bạn có bao giờ tham gia một hoạt động mà bản thân không thích, chỉ vì sợ lạc lõng?", o:[
    "A. Chưa bao giờ",
    "B. Ít khi",
    "C. Khá thường xuyên",
    "D. Hầu như luôn như vậy"
  ]},
  { q: "7. Khi thấy người khác đạt thành tích nổi bật (học tập, sự nghiệp…), bạn thường:", o:[
    "A. Chỉ vui cho họ",
    "B. Có chút so sánh nhưng không lâu",
    "C. So sánh và cảm thấy tự ti",
    "D. Luôn nghĩ mình đang tụt lại phía sau"
  ]},
  { q: "8. Bạn có bao giờ cảm thấy bồn chồn nếu điện thoại không có kết nối mạng?", o:[
    "A. Không",
    "B. Thỉnh thoảng",
    "C. Thường xuyên",
    "D. Luôn luôn"
  ]},
  { q: "9. Nếu một ngày bạn không vào mạng xã hội, bạn sẽ:", o:[
    "A. Bình thường",
    "B. Hơi thiếu nhưng chấp nhận được",
    "C. Cảm thấy bất an",
    "D. Rất lo lắng, sợ bỏ lỡ nhiều thứ"
  ]},
  { q: "10. Khi bạn không được gắn thẻ trong ảnh chụp chung, bạn thường:", o:[
    "A. Không để ý",
    "B. Hơi tiếc một chút",
    "C. Thắc mắc tại sao",
    "D. Buồn bực, nghĩ rằng mình bị cố ý bỏ quên"
  ]},
  { q: "11. Trong lúc học/bận việc, bạn có thường bị thôi thúc mở điện thoại kiểm tra tin tức?", o:[
    "A. Không bao giờ",
    "B. Đôi khi",
    "C. Khá thường xuyên",
    "D. Liên tục, khó kiềm chế"
  ]},
  { q: "12. Khi có một xu hướng mới trên TikTok/Facebook, bạn thường:", o:[
    "A. Không quan tâm",
    "B. Xem cho biết",
    "C. Thử làm theo để hòa nhập",
    "D. Cảm thấy bắt buộc phải tham gia để không bị tụt hậu"
  ]},
  { q: "13. Bạn có từng đăng bài/ảnh chỉ để chứng minh rằng mình cũng đang vui vẻ như người khác?", o:[
    "A. Chưa bao giờ",
    "B. Thỉnh thoảng",
    "C. Khá thường xuyên",
    "D. Gần như luôn vậy"
  ]},
  { q: "14. Khi không nhận được lượt like hoặc comment mong đợi, bạn thường:", o:[
    "A. Không quan tâm",
    "B. Có chút tiếc",
    "C. Thấy buồn, thất vọng",
    "D. Nghĩ rằng mình không được coi trọng"
  ]},
  { q: "15. Nếu bỏ lỡ một buổi học thêm/hoạt động ngoại khóa, bạn thường nghĩ:", o:[
    "A. Không vấn đề gì",
    "B. Hơi lo lắng một chút",
    "C. Sợ mình sẽ thua kém bạn bè",
    "D. Rất căng thẳng, ám ảnh chuyện bỏ lỡ"
  ]},
  { q: "16. Khi bạn bè lập nhóm riêng mà không mời mình, bạn thường:", o:[
    "A. Không quan tâm",
    "B. Nghĩ rằng chắc họ có lý do",
    "C. Cảm thấy bị loại trừ",
    "D. Rất buồn, khó chịu, lo lắng mất bạn"
  ]},
  { q: "17. Bạn thường kiểm tra thông báo trên điện thoại khi nào?", o:[
    "A. Lâu lâu mới xem",
    "B. Khi rảnh",
    "C. Gần như mỗi giờ",
    "D. Liên tục, kể cả lúc đang làm việc khác"
  ]},
  { q: "18. Khi thấy người khác đi du lịch, bạn thường:", o:[
    "A. Chỉ ngắm cho vui",
    "B. Thấy thích nhưng không bận tâm nhiều",
    "C. Ước mình cũng được đi",
    "D. Cảm giác hụt hẫng, tiếc nuối, so sánh bản thân"
  ]},
  { q: "19. Bạn có từng đồng ý tham gia một nhóm chat chỉ để không bỏ lỡ thông tin, dù không thích nhóm đó?", o:[
    "A. Không bao giờ",
    "B. Thỉnh thoảng",
    "C. Khá thường xuyên",
    "D. Luôn như vậy"
  ]},
  { q: "20. Trong một ngày, bạn dành bao nhiêu thời gian cho mạng xã hội?", o:[
    "A. Dưới 1 giờ",
    "B. 1–2 giờ",
    "C. 3–4 giờ",
    "D. Trên 5 giờ"
  ]},
  { q: "21. Khi không kịp tham gia một thử thách online nổi tiếng, bạn cảm thấy:", o:[
    "A. Bình thường",
    "B. Hơi tiếc",
    "C. Tự trách mình",
    "D. Lo lắng bị tụt lại phía sau"
  ]},
  { q: "22. Nếu bạn bè không trả lời tin nhắn ngay, bạn thường:", o:[
    "A. Kiên nhẫn chờ",
    "B. Có chút sốt ruột",
    "C. Nghĩ rằng mình bị lờ đi",
    "D. Rất lo lắng, liên tục kiểm tra"
  ]},
  { q: "23. Khi thấy thông tin nóng hổi mà mình chưa biết, bạn thường:", o:[
    "A. Không quan tâm",
    "B. Tìm hiểu khi rảnh",
    "C. Tìm ngay lập tức",
    "D. Lo sợ mình là người cuối cùng biết"
  ]},
  { q: "24. Bạn có hay mở điện thoại ngay khi vừa thức dậy để kiểm tra tin tức không?", o:[
    "A. Không bao giờ",
    "B. Thỉnh thoảng",
    "C. Khá thường xuyên",
    "D. Hầu như ngày nào cũng vậy"
  ]},
  { q: "25. Khi phải lựa chọn giữa nghỉ ngơi và tham gia một buổi đi chơi, bạn thường:", o:[
    "A. Chọn nghỉ ngơi",
    "B. Tùy tâm trạng",
    "C. Dù mệt vẫn cố đi",
    "D. Luôn chọn đi vì sợ bị bỏ lỡ"
  ]},
  { q: "26. Bạn có hay cảm thấy cuộc sống của mình kém thú vị hơn khi nhìn mạng xã hội của người khác?", o:[
    "A. Không bao giờ",
    "B. Thỉnh thoảng",
    "C. Khá thường xuyên",
    "D. Luôn cảm thấy vậy"
  ]},
  { q: "27. Khi một người bạn đăng ảnh với nhóm khác mà không có bạn, bạn thường:", o:[
    "A. Vui cho họ",
    "B. Thấy hơi chạnh lòng",
    "C. Nghĩ rằng mình không còn quan trọng",
    "D. Rất buồn, khó ngủ vì suy nghĩ"
  ]},
  { q: "28. Bạn có từng dùng mạng xã hội ngay cả khi đang tham gia hoạt động ngoài đời (ăn uống, xem phim)?", o:[
    "A. Không",
    "B. Hiếm khi",
    "C. Khá thường xuyên",
    "D. Luôn như vậy"
  ]},
  { q: "29. Bạn có thường đăng bài với kỳ vọng nhận được nhiều lượt like?", o:[
    "A. Không bao giờ",
    "B. Đôi lúc có",
    "C. Thường xuyên",
    "D. Luôn mong đợi điều đó"
  ]},
  { q: "30. Bạn có thường xuyên mở điện thoại mà không có lí do rõ ràng?", o:[
    "A. Rất hiếm",
    "B. Đôi khi",
    "C. Khá thường xuyên",
    "D. Gần như luôn làm vậy"
  ]}
];

/* Render questions */
const questionsContainer = document.getElementById('questions-container');
quizQuestions.forEach((item, idx) => {
  const div = document.createElement('div');
  div.className = 'question';
  div.innerHTML = `<p>${item.q}</p>`;
  const optionsHtml = item.o.map((opt, i) => {
    return `<label><input type="radio" name="q${idx}" value="${i+1}"> ${opt}</label>`;
  }).join('');
  div.innerHTML += `<div class="options">${optionsHtml}</div>`;
  questionsContainer.appendChild(div);
});

/* Submit logic: check unanswered, compute score, show level + advice */
const submitBtn = document.getElementById('submitBtn');
const clearBtn = document.getElementById('clearBtn');
const resultArea = document.getElementById('result-area');

submitBtn.addEventListener('click', ()=>{
  // collect answers
  const unanswered = [];
  let total = 0;
  for(let i=0;i<quizQuestions.length;i++){
    const sel = document.querySelector(`input[name="q${i}"]:checked`);
    if(!sel) unanswered.push(i+1);
    else total += parseInt(sel.value,10);
  }

  if(unanswered.length){
    alert("Bạn chưa trả lời hết câu hỏi. Vui lòng trả lời các câu: " + unanswered.join(", "));
    // scroll to first unanswered question:
    const first = document.querySelector(`input[name="q${unanswered[0]-1}"]`);
    if(first){
      first.scrollIntoView({behavior:'smooth', block:'center'});
    }
    return;
  }

  // Classification thresholds (total min 30, max 120)
  // We'll use: 30-50 low, 51-85 medium, 86-120 high
  let levelText = "";
  let advice = "";
  if(total <= 50){
    levelText = "Mức độ FOMO: Thấp";
    advice = "Bạn kiểm soát tốt xu hướng FOMO. Tiếp tục duy trì thói quen lành mạnh: cân bằng thời gian online và offline, và giữ mối quan hệ trực tiếp với bạn bè.";
  } else if(total <= 85){
    levelText = "Mức độ FOMO: Trung bình";
    advice = "Bạn có dấu hiệu FOMO. Hãy thử giảm thời gian lướt mạng, đặt giới hạn thông báo, và dành thời gian cho hoạt động ngoại khóa, giao tiếp trực tiếp.";
  } else {
    levelText = "Mức độ FOMO: Cao";
    advice = "FOMO đang khá ảnh hưởng. Nên tìm sự hỗ trợ: trò chuyện với gia đình hoặc thầy cô, thử các kỹ thuật quản lý thời gian và cân nhắc tư vấn tâm lý nếu cần.";
  }

  // Short tips (3 bullets) based on level
  let tips = [];
  if(total <= 50){
    tips = [
      "Giữ thói quen cân bằng: tiếp tục hạn chế thông báo không cần thiết.",
      "Duy trì hoạt động ngoài đời và tương tác trực tiếp.",
      "Theo dõi cảm xúc, nghỉ ngơi đúng giờ."
    ];
  } else if(total <= 85){
    tips = [
      "Đặt thời gian cố định cho mạng xã hội (ví dụ: 30–60 phút/ngày).",
      "Tập thói quen tắt thông báo vào giờ học/ngủ.",
      "Tham gia ít nhất 1 hoạt động ngoại khóa/tuần."
    ];
  } else {
    tips = [
      "Nói chuyện với người thân hoặc giáo viên bạn tin tưởng.",
      "Thử kỹ thuật 'digital detox' (ít nhất 1 ngày/tuần không dùng mạng xã hội).",
      "Cân nhắc tìm hỗ trợ chuyên gia tâm lý nếu cảm xúc ảnh hưởng lớn."
    ];
  }

  // Show results
  resultArea.style.display = 'block';
  resultArea.innerHTML = `
    <h4>Kết quả khảo sát</h4>
    <p><strong>Tổng điểm:</strong> ${total} / 120</p>
    <p><strong>${levelText}</strong></p>
    <p><em>${advice}</em></p>
    <div style="margin-top:10px">
      <strong>Lời khuyên ngắn:</strong>
      <ul>
        ${tips.map(t => `<li>${t}</li>`).join('')}
      </ul>
    </div>
  `;

  // Scroll to result
  resultArea.scrollIntoView({behavior:'smooth', block:'center'});
});

/* Clear - reset form */
clearBtn.addEventListener('click', ()=>{
  const inputs = document.querySelectorAll('#quiz-form input[type="radio"]');
  inputs.forEach(i => i.checked = false);
  resultArea.style.display = 'none';
});

/* Accessibility: allow Enter key to submit when focus in quiz form */
document.getElementById('quiz-form').addEventListener('keydown', (e)=>{
  if(e.key === 'Enter'){
    e.preventDefault();
    submitBtn.click();
  }
});
</script>
<script>
// Lấy số lượt truy cập và hiển thị
fetch('/api/visits')
  .then(res => res.json())
  .then(data => {
    const el = document.getElementById('visit-count');
    if(el && data.count !== undefined) {
      el.textContent = `Số lượt truy cập trang web: ${data.count}`;
    }
  });

// Lấy số lượt người tham gia khảo sát và hiển thị
fetch('/api/participants')
  .then(res => res.json())
  .then(data => {
    const el = document.getElementById('participant-count');
    if(el && data.count !== undefined) {
      el.textContent = `Số lượt người đã tham gia khảo sát: ${data.count}`;
    }
  });

// Nhúng Chart.js từ CDN và vẽ biểu đồ quạt tròn kết quả khảo sát
const chartScript = document.createElement('script');
chartScript.src = 'https://cdn.jsdelivr.net/npm/chart.js';
document.head.appendChild(chartScript);

chartScript.onload = function() {
  fetch('/api/stats')
    .then(res => res.json())
    .then(data => {
      const dist = data.distribution || {Low:0, Moderate:0, High:0};
      const ctx = document.getElementById('pieChart').getContext('2d');
      new Chart(ctx, {
        type: 'pie',
        data: {
          labels: ['Thấp', 'Trung bình', 'Cao'],
          datasets: [{
            data: [dist.Low, dist.Moderate, dist.High],
            backgroundColor: ['#4caf50','#ff9800','#f44336'],
            borderColor: '#fff',
            borderWidth: 2
          }]
        },
        options: {
          plugins: {
            legend: {
              display: true,
              position: 'bottom',
              labels: {
                font: {size: 16}
              }
            },
            title: {
              display: true,
              text: 'Phân phối mức độ FOMO',
              font: {size: 18}
            }
          }
        }
      });
    });
};
</script>
</body>
</html>
  
