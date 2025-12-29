---
title: PimaX Pro
layout: default
---

<style>
/* ===== BUTTON TRONG TUẦN ===== */
.week-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 6px;
}

.week-btn {
  display: inline-flex;
  align-items: center;
  gap: 8px;

  padding: 10px 18px;
  border-radius: 10px;

  background: #ffffff;
  border: 2px solid #cfcfcf;

  color: #777;
  font-weight: 700;
  font-size: 18px;
  text-decoration: none;

  transition: all 0.25s ease;
}

.week-btn i {
  font-size: 16px;
  color: inherit;
}

/* Hover */
.week-btn:hover {
  background: #d83b6a;
  border-color: #d83b6a;
  color: #ffffff;

  box-shadow: 0 8px 20px rgba(216, 59, 106, 0.45);
  transform: translateY(-2px);
}

.week-btn,
.week-btn:hover {
  text-decoration: none !important;
}
.math-box {
  border: 2px solid #444;
  border-radius: 12px;
  padding: 16px 18px;
  background: #fafafa;
  margin: 20px 0;
  font-size: 16px;
}

/* PHẦN BÀI TOÁN */
.problem {
  margin-bottom: 12px;
}

/* SOLUTION */
.solution-box summary {
  cursor: pointer;
  font-weight: 600;
  color: #333;
  list-style: none;
  display: flex;
  align-items: center;
  gap: 10px;
}

/* bỏ mũi tên mặc định */
.solution-box summary::-webkit-details-marker {
  display: none;
}

.solution-box summary::after {
  content: "▼";
  margin-left: auto;
  transition: transform 0.25s ease;
}

.solution-box[open] summary::after {
  transform: rotate(180deg);
}

.solution {
  margin-top: 12px;
  padding-left: 6px;
  border-left: 3px solid #555;
}

</style>
<style>
   .social-drive {
   background: #000000;
   }
   .register-box {
   max-width: 900px;
   margin: 50px auto;
   padding: 34px 32px;
   background: linear-gradient(135deg, #ffe6ef, #fff0f6);
   border-radius: 20px;
   text-align: center;
   box-shadow: 0 12px 28px rgba(0,0,0,0.12);
   }
   .register-box h2 {
   margin-top: 0;
   color: #d83b6a;
   font-size: 30px;
   font-weight: 900;
   }
   .register-box p {
   font-size: 18px;
   margin: 16px 0 28px;
   color: #333;
   }
   .register-box a {
   display: inline-block;
   padding: 14px 34px;
   background: #d83b6a;
   color: white;
   border-radius: 40px;
   font-size: 18px;
   font-weight: 700;
   text-decoration: none;
   transition: transform 0.25s ease, box-shadow 0.25s ease;
   }
   .register-box a:hover {
   transform: translateY(-3px);
   box-shadow: 0 10px 24px rgba(216,59,106,0.45);
   }
   .year-box {
   position: relative;
   max-width: 1100px;
   margin: 70px auto;
   padding: 60px 30px 40px;
   border: 3px solid #ec5b8c;
   border-radius: 20px;
   background: #fff7fa;
   }
   /* BOX "NĂM 2025" */
   .year-title {
   position: absolute;
   top: 0;
   left: 50%;
   transform: translate(-50%, -50%);
   padding: 14px 42px;
   background: #ec5b8c; /* giữ nguyên màu như bạn đang dùng */
   color: white;
   font-size: 32px;
   font-weight: 900;
   border-radius: 20px;
   white-space: nowrap;
   /* che đường viền đi qua chính giữa */
   z-index: 2;
   }
   .contest-title-box {
   display: block;
   width: fit-content;
   margin: 0px auto 32px;   /* hạ box xuống + căn giữa */
   padding: 14px 38px;
   background: #d83b6a;
   color: white;
   font-size: 26px;
   font-weight: 700;
   border-radius: 20px;
   text-align: center;
   box-shadow: 0 10px 30px rgba(216, 59, 106, 0.4);
   }
   .contest-box {
   max-width: 900px;
   margin: 40px auto;
   padding: 30px 28px;
   background: #ffe6ef;
   border-top: 8px solid #d83b6a;
   border-radius: 0px;
   font-family: -apple-system, BlinkMacSystemFont,
   "Segoe UI", Arial,
   "Helvetica Neue",
   "Noto Sans",
   "Liberation Sans",
   sans-serif;
   color: #333;
   line-height: 1.6;
   }
   .contest-box h2 {
   text-align: center;
   color: #d83b6a;
   margin-bottom: 25px;
   font-size: 28px;
   }
   .contest-box ol {
   padding-left: 22px;
   }
   .contest-box li {
   margin-bottom: 18px;
   }
   .contest-box ul {
   margin-top: 8px;
   padding-left: 20px;
   }
   .contest-box a {
   color: #d83b6a;
   font-weight: bold;
   text-decoration: none;
   }
   .contest-box a:hover {
   text-decoration: underline;
   }
   .score-formula {
   background: white;
   padding: 10px 16px;
   border-radius: 12px;
   margin: 10px 0;
   font-weight: bold;
   text-align: center;
   color: #d83b6a;
   }
   .reward-block {
   background: #fff;
   border-radius: 14px;
   padding: 16px 20px;
   margin-top: 10px;
   }
   .reward-block p {
   margin-top: 12px;
   font-weight: bold;
   }
</style>
<style>
   header.site-header {
   background: linear-gradient(135deg, #DB3B6D, #E57195) !important;
   border-bottom: none !important;
   }
   header.site-header a.site-title {
   color: white !important;
   font-size: 30px !important;
   font-weight: 900 !important;
   letter-spacing: 1px;
   }
   header.site-header a.site-title:hover {
   text-decoration: none;
   color: #fff0f6 !important;
   }
</style>
<style>
   .stage {
   background: linear-gradient(135deg, #DB3B6D, #E57195);
   color: white;
   padding: 32px;
   border-radius: 20px;
   text-align: center;
   margin-bottom: 45px;
   box-shadow: 0 10px 24px rgba(0,0,0,0.18);
   }
   .stage h1 {
   font-size: 44px;
   font-weight: 900;
   margin: 0;
   }
   .stage p {
   font-size: 18px;
   margin-top: 10px;
   }
   .week {
   background: #F9DFE8;
   padding: 22px 26px;
   border-radius: 16px;
   margin-bottom: 32px;
   box-shadow: 0 10px 24px rgba(0,0,0,0.18);
   }
   .week h2 {
   color: #d6336c;
   font-size: 30px;
   font-weight: 800;
   margin-top: 0;
   }
   .item {
   background: white;
   padding: 18px 22px;
   border-radius: 14px;
   margin: 16px 0;
   box-shadow: 0 4px 14px rgba(0,0,0,0.10);
   font-size: 18px;
   line-height: 1.7;
   }
   .item a {
   text-decoration: none;
   color: #ff3366;
   font-weight: bold;
   }
   .item a:hover {
   text-decoration: underline;
   }

  .week-clean {
  position: relative;
  background: #FAE2E9;
  box-shadow: 0 4px 14px rgba(0,0,0,0.10);
  border-radius: 32px;
  padding: 80px 36px 36px;
  margin: 40px 0;
}

    .week-badge {
  position: absolute;
  top: 0;
  left: 50%;
  transform: translate(-50%, -50%);

  display: inline-flex;
  align-items: center;
  gap: 12px;

  padding: 8px 28px;
  background: #FAE2E9;

  border: 2px solid #333;
  border-radius: 10px;

  font-size: 22px;
  font-weight: 800;
  letter-spacing: 1px;
  color: #333;
}

/* Icon lịch */
.week-badge i {
  font-size: 26px;
  color: #333;
}
  .week-badge {
  top: 50px;  /* mặc định là 0 */
}

</style>

<div class="year-box">
  <div class="year-title">
  <i class="fa-solid fa-calendar-check"></i> 2025$-$2026
  </div>

  <div class="stage">
    <h1>
      <i class="fa-solid fa-snowman"></i>
      Chặng 1$–$2025 WINTER
    </h1>
    <p> Diễn ra từ ngày 22/12/2025 </p>
  </div>

  <div class="week-clean">
     <div class="week-badge">
    <i class="fa-regular fa-calendar"></i>
    TUẦN 1
  </div>

    <!-- TEST 0 -->
    <div class="item">
      <div class="week-buttons">

        <a class="week-btn"
           href="https://drive.google.com/file/d/1H2CbP2u8Hlc3arnnkYC01jx4E8Mk-o1K/view?usp=drive_link"
           target="_blank" rel="noopener">
          <i class="fa-regular fa-file-lines"></i> TEST 0
        </a>

        <a class="week-btn"
           href="https://drive.google.com/file/d/1zEZQXB8WeTGvMpizUxK__h1Wg4whcP17/view?usp=drive_link"
           target="_blank" rel="noopener">
          <i class="fa-solid fa-pen"></i> BVT
        </a>

        <a class="week-btn"
           href="https://drive.google.com/file/d/1u2dE0N0Ay4g0ylwstJg4l6T_j_s3eHJ5/view?usp=drive_link"
           target="_blank" rel="noopener">
          <i class="fa-solid fa-play"></i> Solution
        </a>

        <a class="week-btn"
           href="https://docs.google.com/spreadsheets/d/1vtfoBgg8D5AyoK7CHxDtbjKM93db-22E/edit?usp=drive_link"
           target="_blank" rel="noopener">
          <i class="fa-solid fa-chart-column"></i> Ranking
        </a>

      </div>
    </div>

    <!-- TEST 1 -->
    <div class="item">
      <div class="week-buttons">

        <a class="week-btn"
           href="https://drive.google.com/file/d/1YYJmNPRncCEiXGx31lsOFcATeE_KYcY_/view?usp=drive_link"
           target="_blank" rel="noopener">
          <i class="fa-regular fa-file-lines"></i> TEST 1
        </a>

        <a class="week-btn"
           href="https://drive.google.com/file/d/1hzCNKgNaPXclUZ_OWSsFxd_fhjlfcz9j/view?usp=drive_link"
           target="_blank" rel="noopener">
          <i class="fa-solid fa-pen"></i> BVT
        </a>

        <a class="week-btn"
           href="https://drive.google.com/file/d/1N0Iildna80-oA_f18lFmUOcZfVnUu-8k/view?usp=drive_link"
           target="_blank" rel="noopener">
          <i class="fa-solid fa-play"></i> Solution
        </a>

        <a class="week-btn"
           href="https://docs.google.com/spreadsheets/d/1vtfoBgg8D5AyoK7CHxDtbjKM93db-22E/edit"
           target="_blank" rel="noopener">
          <i class="fa-solid fa-chart-column"></i> Ranking
        </a>

      </div>
    </div>

    <div class="math-box">
  <!-- PHẦN 1: BÀI TOÁN -->
  <div class="problem">
    <strong>Bài toán.</strong>
    <p>
      Tìm tất cả các số thực \(x\) thỏa mãn
      \[
        x^2 - 3x + 2 = 0.
      \]
    </p>
  </div>

  <!-- PHẦN 2: LỜI GIẢI -->
  <details class="solution-box">
    <summary>
      <i class="fa-solid fa-lightbulb"></i> Solution
    </summary>

    <div class="solution">
      <p>
        Ta có:
        \[
          x^2 - 3x + 2 = (x-1)(x-2).
        \]
        Do đó \(x = 1\) hoặc \(x = 2\).
      </p>
    </div>
  </details>
</div>


  </div>
</div>




<div class="contest-box">
   <div class="contest-title-box">
      <i class="fa-solid fa-bullhorn"></i>
      THỂ LỆ CUỘC THI
   </div>
   <ol>
      <li>
         <strong>Cấu trúc cuộc thi:</strong><br>
         Cuộc thi bao gồm <strong>3 chặng</strong> tương ứng với 3 đợt thi chính:
         <ul>
            <li>Chặng 1 – <strong>Winter 2025</strong></li>
            <li>Chặng 2 – <strong>Spring 2026</strong></li>
            <li>Chặng 3 – <strong>Summer 2026</strong></li>
         </ul>
      </li>
      <li>
         <strong>Lịch thi hàng tuần:</strong><br>
         Mỗi tuần thí sinh làm <strong>2 bài test</strong>:
         <ul>
            <li>
               <strong>Bài thi 1:</strong> 40 câu / 60 phút (40 điểm), cấu trúc TSA, 
               diễn ra vào <strong>thứ 2 hàng tuần</strong>.
            </li>
            <li>
               <strong>Bài thi 2:</strong> 10 câu / 30 phút (10 điểm), chủ yếu là bài toán khó,
               diễn ra vào <strong>thứ 6 hàng tuần</strong>.
            </li>
         </ul>
         <i class="fa-solid fa-hand-point-right"></i>
          Lưu ý: Thí sinh cần đăng kí tài khoản trước tại
         <a href="https://pimaxtsa.com" target="_blank" rel="noopener">pimaxtsa.com</a>.
      </li>
      <li>
         <strong>Cách tính điểm:</strong><br>
         Điểm mỗi tuần được tính theo công thức:
         <div class="score-formula">
            Điểm tuần = Điểm bài 1 + 1.5 × Điểm bài 2
         </div>
         Điểm của mỗi chặng là <strong>trung bình cộng điểm các tuần</strong> trong chặng đó.
      </li>
      <li>
         <strong>Phần thưởng:</strong>
         <div class="reward-block">
            <p><strong>a) Phần thưởng sau mỗi chặng (Top 3):</strong></p>
            <ul>
               <li><i class="fa-solid fa-trophy"></i> <strong>Nhà vô địch:</strong> 1.000.000 VNĐ + Khóa học toàn diện PimaX</li>
               <li><i class="fa-solid fa-medal silver"></i> <strong>Hai á quân:</strong> mỗi người 500.000 VNĐ + Khóa học toàn diện PimaX</li>
            </ul>
            <p><strong>b) Phần thưởng hàng tuần (Top 10):</strong></p>
            <ul>
               <li>
                  <i class="fa-solid fa-star"></i> <strong>Top 2:</strong> 100.000 VNĐ + 10 đề TSA kèm video chữa + giảm 40% học phí
               </li>
               <li>
                  <i class="fa-solid fa-bullseye"></i> <strong>Top 8 còn lại:</strong> 5 đề TSA kèm video chữa + giảm 30% học phí
               </li>
            </ul>
         </div>
      </li>
   </ol>
</div>
<div class="register-box">
   <h2><i class="fa-solid fa-pen-to-square"></i> ĐĂNG KÝ THAM GIA CUỘC THI</h2>
   <p>
      Thí sinh vui lòng đăng ký tài khoản và điền form trước khi tham gia
      các bài thi chính thức của PimaX TSABK Tournament. Thời gian đăng kí: Hết ngày 28/12/2025
   </p>
   <a href="https://docs.google.com/forms/d/1BGeWoQaCTOCkviJb8fbQ1kxnebybMEDUlZjp3HUO9ks/edit"
      target="_blank"
      rel="noopener">
   <i class="fa-solid fa-hand-point-right"></i> ĐI TỚI FORM ĐĂNG KÝ
   </a>
</div>
<style>
   .social-box {
   max-width: 900px;
   margin: 40px auto;
   padding: 22px 28px;
   background: #ffffff;
   border-radius: 22px;
   box-shadow: 0 12px 30px rgba(0,0,0,0.12);
   display: flex;
   justify-content: center;
   gap: 26px;
   }
   .social-box a {
   width: 64px;
   height: 64px;
   border-radius: 50%;
   display: flex;
   align-items: center;
   justify-content: center;
   font-size: 28px;
   color: white;
   text-decoration: none;
   transition: transform 0.25s ease, box-shadow 0.25s ease;
   }
   .social-box a:hover {
   transform: translateY(-4px) scale(1.08);
   box-shadow: 0 10px 22px rgba(0,0,0,0.25);
   }
   /* Màu từng mạng xã hội */
   .social-tiktok {
   background: #000000;
   }
   .social-facebook {
   background: #1877f2;
   }
   .social-web {
   background: linear-gradient(135deg, #d83b6a, #ff7aa2);
   }
</style>
<div class="social-box">
   <!-- TikTok -->
   <a href="https://www.tiktok.com/@pimaxghettoan"
      target="_blank"
      class="social-tiktok"
      aria-label="TikTok">
   <i class="fa-brands fa-tiktok"></i>
   </a>
   <!-- Facebook -->
   <a href="https://www.facebook.com/PimaXPro"
      target="_blank"
      class="social-facebook"
      aria-label="Facebook">
   <i class="fa-brands fa-facebook-f"></i>
   </a>
   <!-- Website -->
   <a href="https://pimaxtsa.com"
      target="_blank"
      class="social-web"
      aria-label="Website">
   <i class="fa-solid fa-globe"></i>
   </a>
   <a href="https://drive.google.com/drive/u/2/folders/1JP1dhqeJaR8ddZ8uVKL84s5GcJ9a5oPl"
      target="_blank"
      class="social-drive"
      aria-label="Google Drive">
   <i class="fa-brands fa-google-drive"></i>
   </a>
</div>
<style>
   .wrapper {
   max-width: 1400px !important;
   }
</style>
