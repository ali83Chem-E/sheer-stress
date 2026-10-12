# sheer-stress
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<title>فرمول‌های ویسکوزیته لامینار - مک کی</title>
<style>
  body {
    font-family: 'Tahoma', 'Vazirmatn', sans-serif;
    background: #f4f6f9;
    color: #222;
    margin: 20px;
    line-height: 1.8;
  }
  h1 {
    text-align: center;
    color: #1a3d6d;
    border-bottom: 3px solid #1a3d6d;
    padding-bottom: 10px;
  }
  h2 {
    background: #1a3d6d;
    color: #fff;
    padding: 10px 15px;
    border-radius: 8px;
    margin-top: 40px;
  }
  .conditions {
    background: #fff8e1;
    border-right: 5px solid #ffb300;
    padding: 10px 15px;
    border-radius: 6px;
    margin: 10px 0;
  }
  .conditions ul {
    margin: 5px 0;
    padding-right: 20px;
  }
  table {
    width: 100%;
    border-collapse: collapse;
    margin: 15px 0;
    background: #fff;
    box-shadow: 0 2px 6px rgba(0,0,0,0.08);
    border-radius: 8px;
    overflow: hidden;
  }
  th {
    background: #2c5f9e;
    color: #fff;
    padding: 10px;
    text-align: right;
    font-size: 15px;
  }
  td {
    padding: 10px 12px;
    border-bottom: 1px solid #e0e0e0;
    vertical-align: top;
  }
  tr:nth-child(even) td {
    background: #f9fbfd;
  }
  .formula {
    direction: ltr;
    text-align: center;
    font-family: 'Cambria Math', 'Times New Roman', serif;
    font-size: 17px;
    background: #eef4fb;
    padding: 6px 10px;
    border-radius: 5px;
    display: inline-block;
  }
  .note {
    background: #e8f5e9;
    border-right: 5px solid #43a047;
    padding: 10px 15px;
    border-radius: 6px;
    margin: 10px 0;
    font-size: 14px;
  }
  .warning {
    background: #ffebee;
    border-right: 5px solid #e53935;
    padding: 10px 15px;
    border-radius: 6px;
    margin: 10px 0;
    font-size: 14px;
  }
  .shape {
    background: #263238;
    color: #aed581;
    font-family: 'Courier New', monospace;
    direction: ltr;
    text-align: left;
    padding: 12px;
    border-radius: 6px;
    font-size: 13px;
    white-space: pre;
    overflow-x: auto;
  }
  .tag {
    display: inline-block;
    background: #ffb300;
    color: #333;
    padding: 2px 8px;
    border-radius: 4px;
    font-size: 12px;
    margin-right: 5px;
  }
</style>
</head>
<body>

<h1>📘 جدول کامل فرمول‌های ویسکوزیته لامینار (مک‌کی)</h1>

<div class="conditions">
  <strong>🔑 شرایط مشترک همه حالت‌ها:</strong>
  <ul>
    <li>جریان <b>لامینار</b></li>
    <li>جریان <b>پایا</b> (Steady State)</li>
    <li>سیال <b>نیوتونی</b></li>
    <li><b>بدون</b> گرادیان فشار اضافی</li>
    <li><b>بدون</b> اثر گرانش</li>
    <li><b>بدون</b> اثر گریز از مرکز</li>
  </ul>
</div>

<!-- ================= حالت ۱ ================= -->
<h2>۱️⃣ دو صفحه موازی (Couette Flow)</h2>

<div class="shape">
صفحه متحرک (V)  ──────────────────  z = B
                      ↑
                      |   سیال (μ)
                      |
صفحه ثابت       ──────────────────  z = 0
</div>

<div class="conditions">
  <strong>🔹 نحوه قرارگیری سیال:</strong>
  سیال بین دو صفحه موازی افقی قرار دارد. صفحه پایین ثابت است و صفحه بالایی با سرعت ثابت V در جهت x حرکت می‌کند.
</div>

<table>
  <tr>
    <th>کمیت</th>
    <th>فرمول</th>
    <th>توضیحات</th>
  </tr>
  <tr>
    <td>تنش برشی</td>
    <td><span class="formula">τ<sub>yx</sub> = μV / B</span></td>
    <td>V = سرعت صفحه متحرک، B = فاصله بین دو صفحه</td>
  </tr>
  <tr>
    <td>پروفیل سرعت</td>
    <td><span class="formula">v<sub>x</sub> = V·(y / B)</span></td>
    <td>پروفیل خطی — سرعت با فاصله از صفحه ثابت زیاد می‌شود</td>
  </tr>
  <tr>
    <td>نیروی روی صفحه</td>
    <td><span class="formula">F = τ × A</span></td>
    <td>A = سطح تماس سیال با صفحه</td>
  </tr>
</table>

<div class="note">
  💡 <b>نکته:</b> این ساده‌ترین حالت است و پایه ویسکومتر چرخشی محسوب می‌شود.
</div>

<!-- ================= حالت ۲ ================= -->
<h2>۲️⃣ لوله استوانه‌ای (Hagen-Poiseuille)</h2>

<div class="shape">
─────────────────────────────
→ → → → → → → → → → → → → →   جریان
─────────────────────────────
          R (شعاع)
</div>
<div class="conditions">
  <strong>🔹 نحوه قرارگیری سیال:</strong>
  سیال داخل یک لوله استوانه‌ای افقی به شعاع R قرار دارد و به دلیل اختلاف فشار (P₀ - P_L) در طول L جریان می‌یابد.
</div>

<table>
  <tr>
    <th>کمیت</th>
    <th>فرمول</th>
    <th>توضیحات</th>
  </tr>
  <tr>
    <td>تنش برشی</td>
    <td><span class="formula">τ<sub>rz</sub> = [(P₀-P_L) / 2L] · r</span></td>
    <td>تنش به صورت خطی با r زیاد می‌شود</td>
  </tr>
  <tr>
    <td>پروفیل سرعت</td>
    <td><span class="formula">v<sub>z</sub> = [(P₀-P_L) / 4μL] · (R² - r²)</span></td>
    <td>پروفیل سهمی — بیشینه در مرکز لوله</td>
  </tr>
  <tr>
    <td>سرعت ماکزیمم</td>
    <td><span class="formula">v<sub>max</sub> = (P₀-P_L)R² / 4μL</span></td>
    <td>در r = 0 (مرکز لوله)</td>
  </tr>
  <tr>
    <td>سرعت متوسط</td>
    <td><span class="formula">v‌ = v<sub>max</sub> / 2</span></td>
    <td>نصف سرعت ماکزیمم</td>
  </tr>
  <tr>
    <td>دبی حجمی</td>
    <td><span class="formula">Q = π(P₀-P_L)R⁴ / 8μL</span></td>
    <td>رابطه پوازی — بسیار مهم در مهندسی</td>
  </tr>
  <tr>
    <td>تنش روی دیواره</td>
    <td><span class="formula">τ<sub>w</sub> = (P₀-P_L)R / 2L</span></td>
    <td>در r = R</td>
  </tr>
</table>

<div class="warning">
  ⚠️ <b>شرط مرزی:</b> سرعت روی دیواره صفر است (No-Slip): v<sub>z</sub>(R) = 0
</div>

<!-- ================= حالت ۳ ================= -->
<h2>۳️⃣ دیسک دوار بین دو صفحه ثابت ⭐</h2>

<div class="shape">
صفحه ثابت بالا      ─────────────────  z = +h
                          ↑
                          |  سیال (μ)
                          |
دیسک دوار (Ω)      ══════════════════  z = 0
                          |
                          |  سیال (μ)
                          ↓
صفحه ثابت پایین    ─────────────────  z = -h
</div>

<div class="conditions">
  <strong>🔹 نحوه قرارگیری سیال:</strong>
  یک دیسک دوار در وسط قرار دارد و دو صفحه ثابت در بالا و پایین آن هستند. سیال در هر دو نیمه (بالا و پایین دیسک) قرار دارد. دیسک با سرعت زاویه‌ای Ω می‌چرخد.
</div>

<table>
  <tr>
    <th>کمیت</th>
    <th>فرمول</th>
    <th>توضیحات</th>
  </tr>
  <tr>
    <td>پروفیل سرعت (نیمه بالا)</td>
    <td><span class="formula">v<sub>θ</sub> = Ωr(1 - z/h)</span></td>
    <td>0 ≤ z ≤ h — خطی از دیسک به صفحه بالا</td>
  </tr>
  <tr>
    <td>پروفیل سرعت (نیمه پایین)</td>
    <td><span class="formula">v<sub>θ</sub> = Ωr(1 + z/h)</span></td>
    <td>-h ≤ z ≤ 0 — خطی از صفحه پایین به دیسک</td>
  </tr>
  <tr>
    <td>تنش برشی (یک طرف)</td>
    <td><span class="formula">τ<sub>zθ</sub> = μΩr / h</span></td>
    <td>تنش روی یک وجه دیسک</td>
  </tr>
  <tr>
    <td><b>تنش کل روی دیسک</b></td>
    <td><span class="formula">τ<sub>total</sub> = 2μΩr / h</span></td>
    <td>چون دیسک از دو طرف تنش می‌بیند، ضریب ۲ ظاهر می‌شود</td>
  </tr>
  <tr>
    <td>گشتاور روی دیسک</td>
    <td><span class="formula">T = πμΩR⁴ / h</span></td>
    <td>R = شعاع دیسک</td>
  </tr>
  <tr>
    <td>توان مصرفی</td>
    <td><span class="formula">P = T·Ω = πμΩ²R⁴ / h</span></td>
    <td>توان لازم برای چرخاندن دیسک</td>
  </tr>
</table>

<div class="note">
  💡 <b>نکته کلیدی:</b> این حالت پایه <b>ویسکومتر دیسکی</b> است. با اندازه‌گیری T و Ω می‌توان μ را پیدا کرد.
</div>

<!-- ================= حالت ۴ ================= -->
<h2>۴️⃣ دو دیسک موازی (ویسکومتر دیسکی)</h2>

<div class="shape">
دیسک دوار (Ω)   ══════════════════  z = B
                      ↑
                      |   سیال (μ)
                      |
دیسک ثابت       ──────────────────  z = 0
</div>

<div class="conditions">
  <strong>🔹 نحوه قرارگیری سیال:</strong>
  سیال فقط بین دو دیسک موازی قرار دارد. دیسک پایین ثابت است و دیسک بالایی با سرعت زاویه‌ای Ω می‌چرخد. (فقط یک طرف سیال وجود دارد)
</div>

<table>
  <tr>
    <th>کمیت</th>
    <th>فرمول</th>
    <th>توضیحات</th>
  </tr>
  <tr>
    <td>پروفیل سرعت</td>
    <td><span class="formula">v<sub>θ</sub> = Ωr·(z/B)</span></td>
<td>خطی از دیسک ثابت به دیسک دوار</td>
  </tr>
  <tr>
    <td>تنش برشی</td>
    <td><span class="formula">τ<sub>zθ</sub> = μΩr / B</span></td>
    <td>فقط یک طرف تنش وارد می‌شود</td>
  </tr>
  <tr>
    <td>گشتاور</td>
    <td><span class="formula">T = πμΩR⁴ / 2B</span></td>
    <td>نصف حالت دیسک بین دو صفحه</td>
  </tr>
</table>

<div class="warning">
  ⚠️ <b>تفاوت با حالت ۳:</b> اینجا فقط <b>یک طرف</b> دیسک سیال دارد، پس ضریب ۲ وجود ندارد.
</div>

<!-- ================= حالت ۵ ================= -->
<h2>۵️⃣ استوانه‌های هم‌محور (ویسکومتر کوئت)</h2>

<div class="shape">
      ┌─────────────┐
      │   استوانه  │
      │   خارجی    │
      │  ┌───────┐  │
      │  │ داخلی │  │
      │  │  (Ω)  │  │
      │  └───────┘  │
      └─────────────┘
      R₁ (داخلی), R₂ (خارجی)
</div>

<div class="conditions">
  <strong>🔹 نحوه قرارگیری سیال:</strong>
  سیال در فضای حلقوی بین دو استوانه هم‌محور قرار دارد. استوانه داخلی به شعاع R₁ با سرعت زاویه‌ای Ω می‌چرخد و استوانه خارجی به شعاع R₂ ثابت است.
</div>

<table>
  <tr>
    <th>کمیت</th>
    <th>فرمول</th>
    <th>توضیحات</th>
  </tr>
  <tr>
    <td>پروفیل سرعت</td>
    <td><span class="formula">v<sub>θ</sub> = Ar + B/r</span></td>
    <td>ترکیب خطی و هذلولی — نه خطی!</td>
  </tr>
  <tr>
    <td>تنش برشی</td>
    <td><span class="formula">τ<sub>rθ</sub> = -μr · d/dr(v<sub>θ</sub>/r)</span></td>
    <td>فرم کامل در مختصات استوانه‌ای</td>
  </tr>
  <tr>
    <td>گشتاور روی استوانه داخلی</td>
    <td><span class="formula">T = 4πμΩR₁²R₂²L / (R₂²-R₁²)</span></td>
    <td>L = طول استوانه</td>
  </tr>
</table>

<div class="note">
  💡 <b>نکته:</b> در حالت حدی R₂ → ∞ این حالت به دیسک دوار در سیال نامحدود تبدیل می‌شود.
</div>

<!-- ================= حالت ۶ ================= -->
<h2>۶️⃣ جریان فیلم نازک روی صفحه شیب‌دار</h2>

<div class="shape">
────────────────────────  ← سطح آزاد
← ← ← ← ← ← ← ← ← ← ←
← ← ← ← ← ← ← ← ← ← ←   سیال (μ)
← ← ← ← ← ← ← ← ← ← ←
════════════════════════  ← صفحه شیب‌دار (زاویه β)
</div>

<div class="conditions">
  <strong>🔹 نحوه قرارگیری سیال:</strong>
  یک لایه نازک سیال (ضخامت δ) روی صفحه‌ای با زاویه شیب β قرار دارد و به دلیل گرانش به سمت پایین جریان می‌یابد. سطح آزاد بدون تنش است.
</div>

<table>
  <tr>
    <th>کمیت</th>
    <th>فرمول</th>
    <th>توضیحات</th>
  </tr>
  <tr>
    <td>پروفیل سرعت</td>
    <td><span class="formula">v<sub>x</sub> = ρg·cosβ·(δ²-y²) / 2μ</span></td>
    <td>پروفیل سهمی — بیشینه در سطح آزاد</td>
  </tr>
  <tr>
    <td>سرعت ماکزیمم</td>
    <td><span class="formula">v<sub>max</sub> = ρg·cosβ·δ² / 2μ</span></td>
    <td>در y = 0 (سطح آزاد)</td>
  </tr>
  <tr>
    <td>سرعت متوسط</td>
    <td><span class="formula">v‌ = ρg·cosβ·δ² / 3μ</span></td>
    <td>یک‌سوم سرعت ماکزیمم</td>
  </tr>
  <tr>
    <td>دبی (عرض W)</td>
    <td><span class="formula">Q = ρg·cosβ·δ³·W / 3μ</span></td>
    <td>W = عرض فیلم</td>
  </tr>
  <tr>
    <td>تنش روی صفحه</td>
    <td><span class="formula">τ<sub>w</sub> = ρg·cosβ·δ</span></td>
    <td>در y = δ (روی صفحه)</td>
  </tr>
</table>

<div class="warning">
  ⚠️ <b>توجه:</b> در این حالت <b>گرانش</b> نیروی محرک است — استثنای شرایط مشترک!
</div>

<!-- ================= حالت ۷ ================= -->
<h2>۷️⃣ لایه مرزی روی صفحه تخت (Blasius)</h2>

<div class="shape">
        جریان آزاد (v∞)
→ → → → → → → → → → → →
─────────────────────────
│ لایه مرزی (δ)
│
└──────────────────────  ← صفحه تخت
</div>

<div class="conditions">
  <strong>🔹 نحوه قرارگیری سیال:</strong>
  سیال با سرعت v∞ روی یک صفحه تخت موازی با جریان حرکت می‌کند. لایه مرزی (δ) در نزدیکی صفحه تشکیل می‌شود و با x رشد می‌کند.
</div>

<table>
  <tr>
    <th>کمیت</th>
    <th>فرمول</th>
    <th>توضیحات</th>
  </tr>
  <tr>
    <td>ضخامت لایه مرزی</td>
    <td><span class="formula">δ ≈ 5√(μx / ρv∞)</span></td>
    <td>با جذر x رشد می‌کند</td>
  </tr>
  <tr>
    <td>تنش روی صفحه</td>
	<td><span class="formula">τ<sub>w</sub> = 0.332·ρv∞²·√(μ/ρv∞x)</span></td>
    <td>حل بلازیوس</td>
  </tr>
  <tr>
    <td>ضریب اصطکاک موضعی</td>
    <td><span class="formula">C<sub>f</sub> = 0.664 / √Re<sub>x</sub></span></td>
    <td>Re<sub>x</sub> = ρv∞x / μ</td>
  </tr>
</table>

<div class="note">
  💡 <b>نکته:</b> این حالت با حل عددی بلازیوس به دست آمده است (نه تحلیلی ساده).
</div>

<!-- ================= جدول مقایسه ================= -->
<h2>📊 جدول مقایسه سریع همه حالت‌ها</h2>

<table>
  <tr>
    <th>حالت</th>
    <th>محرک</th>
    <th>پروفیل سرعت</th>
    <th>تنش برشی</th>
  </tr>
  <tr>
    <td>۱. دو صفحه موازی</td>
    <td>حرکت صفحه</td>
    <td>خطی</td>
    <td><span class="formula">μV/B</span></td>
  </tr>
  <tr>
    <td>۲. لوله</td>
    <td>فشار</td>
    <td>سهمی</td>
    <td><span class="formula">ΔP·r / 2L</span></td>
  </tr>
  <tr>
    <td>۳. دیسک بین دو صفحه</td>
    <td>چرخش دیسک</td>
    <td>خطی</td>
    <td><span class="formula">2μΩr/h</span></td>
  </tr>
  <tr>
    <td>۴. دو دیسک</td>
    <td>چرخش دیسک</td>
    <td>خطی</td>
    <td><span class="formula">μΩr/B</span></td>
  </tr>
  <tr>
    <td>۵. استوانه هم‌محور</td>
    <td>چرخش استوانه</td>
    <td>Ar + B/r</td>
    <td><span class="formula">-μr·d/dr(v/r)</span></td>
  </tr>
  <tr>
    <td>۶. فیلم روی صفحه</td>
    <td>گرانش</td>
    <td>سهمی</td>
    <td><span class="formula">ρg·cosβ·δ</span></td>
  </tr>
  <tr>
    <td>۷. لایه مرزی</td>
    <td>جریان آزاد</td>
    <td>بلازیوس</td>
    <td><span class="formula">0.332·ρv∞²/√Re<sub>x</sub></span></td>
  </tr>
</table>

<!-- ================= الگوی نهایی ================= -->
<h2>🔑 الگوی اصلی همه فرمول‌ها</h2>

<div class="note" style="font-size:16px; text-align:center;">
  <span class="formula" style="font-size:20px;">τ = μ · (Δv / Δy)</span>
  <br><br>
  <b>همه فرمول‌های بالا فقط تطبیق این الگو با هندسه‌های مختلف هستند!</b>
</div>

<div class="warning">
  ⚠️ <b>هشدار نهایی:</b> اگر یکی از شرایط مشترک (لامینار، پایا، نیوتونی، بدون فشار، بدون گرانش، بدون گریز از مرکز) برقرار نباشد، این فرمول‌ها <b>معتبر نیستند</b> و باید از صفر حل کنید.
</div>

</body>
</html>















