<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>辛亚楠同学请注意</title>
<style>
* { margin: 0; padding: 0; box-sizing: border-box; }
body {
  font-family: "PingFang SC", "Microsoft JhengHei", sans-serif;
  background: linear-gradient(135deg, #e3f2fd 0%, #f3e5f5 50%, #fce4ec 100%);
  min-height: 100vh;
  min-height: 100dvh;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  padding: 20px;
  padding-bottom: 60px;
  overflow-y: auto;
}
.card {
  background: rgba(255,255,255,0.92);
  backdrop-filter: blur(10px);
  border-radius: 24px;
  box-shadow: 0 8px 32px rgba(0,0,0,0.08);
  padding: 36px 28px;
  max-width: 460px;
  width: 100%;
  text-align: center;
  margin-top: 10px;
}
.avatar {
  width: 80px;
  height: 80px;
  background: linear-gradient(135deg, #90caf9, #ce93d8);
  border-radius: 50%;
  margin: 0 auto 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 40px;
  animation: float 3s ease-in-out infinite;
}
@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-8px); }
}
h1 {
  color: #37474f;
  font-size: 1.6rem;
  margin-bottom: 4px;
}
.subtitle {
  color: #78909c;
  font-size: 0.9rem;
  margin-bottom: 24px;
}
.date-box {
  background: linear-gradient(90deg, #e8f5e9, #e3f2fd);
  border-radius: 14px;
  padding: 12px 20px;
  margin-bottom: 24px;
  color: #546e7a;
  font-size: 0.95rem;
}

.check-list {
  display: flex;
  flex-direction: column;
  gap: 12px;
  margin-bottom: 24px;
}
.check-item {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 20px;
  background: #fafafa;
  border-radius: 16px;
  border: 2px solid transparent;
  cursor: pointer;
  transition: all 0.3s ease;
  text-align: left;
}
.check-item:hover {
  background: #f5f5f5;
  transform: translateX(4px);
}
.check-item.done {
  background: #e8f5e9;
  border-color: #a5d6a7;
}
.check-item.done .check-text {
  color: #2e7d32;
  text-decoration: line-through;
}
.check-left {
  display: flex;
  align-items: center;
  gap: 12px;
}
.check-emoji {
  font-size: 28px;
}
.check-text {
  color: #455a64;
  font-size: 1rem;
}
.check-circle {
  width: 24px;
  height: 24px;
  border-radius: 50%;
  border: 2px solid #bdbdbd;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.3s ease;
  font-size: 14px;
  color: transparent;
}
.check-item.done .check-circle {
  background: #66bb6a;
  border-color: #66bb6a;
  color: white;
}

.progress-box {
  background: #fff8e1;
  border-radius: 16px;
  padding: 18px;
  margin-bottom: 20px;
}
.progress-label {
  color: #f57f17;
  font-size: 0.9rem;
  margin-bottom: 10px;
  font-weight: bold;
}
.progress-bar-bg {
  background: #ffe0b2;
  border-radius: 10px;
  height: 12px;
  overflow: hidden;
}
.progress-bar-fill {
  background: linear-gradient(90deg, #ffb74d, #ff9800);
  height: 100%;
  border-radius: 10px;
  width: 0%;
  transition: width 0.6s cubic-bezier(0.34, 1.56, 0.64, 1);
}
.progress-text {
  color: #e65100;
  font-size: 0.85rem;
  margin-top: 8px;
}

.tip-box {
  background: #f3e5f5;
  border-radius: 14px;
  padding: 16px;
  margin-bottom: 20px;
  color: #6a1b9a;
  font-size: 0.9rem;
  line-height: 1.7;
  text-align: left;
}
.tip-box::before {
  content: '💡 ';
}

.stamp {
  display: none;
  margin-top: 20px;
  animation: stampIn 0.5s cubic-bezier(0.34, 1.56, 0.64, 1) forwards;
}
@keyframes stampIn {
  0% { transform: scale(2); opacity: 0; }
  100% { transform: scale(1); opacity: 1; }
}
.stamp-text {
  display: inline-block;
  border: 3px solid #e53935;
  color: #e53935;
  padding: 8px 24px;
  border-radius: 8px;
  font-size: 1.2rem;
  font-weight: bold;
  transform: rotate(-5deg);
}

.sleep-warning {
  display: none;
  position: fixed;
  top: 0; left: 0; right: 0; bottom: 0;
  background: rgba(0,0,0,0.6);
  z-index: 9999;
  justify-content: center;
  align-items: center;
  padding: 20px;
}
.sleep-warning.show {
  display: flex;
}
.sleep-card {
  background: white;
  border-radius: 24px;
  padding: 36px 28px;
  text-align: center;
  max-width: 360px;
  width: 100%;
  animation: popIn 0.4s ease;
}
.sleep-card .big-emoji {
  font-size: 64px;
  margin-bottom: 16px;
}
.sleep-card h2 {
  color: #37474f;
  margin-bottom: 12px;
}
.sleep-card p {
  color: #78909c;
  margin-bottom: 24px;
  line-height: 1.6;
}
.sleep-btn {
  background: #5c6bc0;
  color: white;
  border: none;
  padding: 14px 36px;
  border-radius: 30px;
  font-size: 1rem;
  cursor: pointer;
  transition: all 0.3s;
}
.sleep-btn:hover {
  background: #3f51b5;
  transform: translateY(-2px);
}

@keyframes popIn {
  0% { transform: scale(0.8); opacity: 0; }
  100% { transform: scale(1); opacity: 1; }
}

@media (max-width: 480px) {
  .card { padding: 28px 20px; }
  h1 { font-size: 1.4rem; }
  .check-item { padding: 14px 16px; }
}
</style>
</head>
<body>

<div class="card">
  <div class="avatar">👩‍⚕️</div>
  <h1>辛亚楠同学</h1>
  <p class="subtitle">今日健康打卡请查收</p>

  <div class="date-box" id="dateBox">加载中…</div>

  <div class="check-list">
    <div class="check-item" onclick="toggleCheck(this)">
      <div class="check-left">
        <span class="check-emoji">💧</span>
        <span class="check-text">喝够 8 杯水</span>
      </div>
      <div class="check-circle">✓</div>
    </div>
    <div class="check-item" onclick="toggleCheck(this)">
      <div class="check-left">
        <span class="check-emoji">🚶</span>
        <span class="check-text">今天动了动（哪怕散步）</span>
      </div>
      <div class="check-circle">✓</div>
    </div>
    <div class="check-item" onclick="toggleCheck(this)">
      <div class="check-left">
        <span class="check-emoji">🥗</span>
        <span class="check-text">没把奶茶当水喝</span>
      </div>
      <div class="check-circle">✓</div>
    </div>
    <div class="check-item" onclick="toggleCheck(this)">
      <div class="check-left">
        <span class="check-emoji">😴</span>
        <span class="check-text">昨晚 12 点前睡了</span>
      </div>
      <div class="check-circle">✓</div>
    </div>
  </div>

  <div class="progress-box">
    <div class="progress-label">今日健康指数</div>
    <div class="progress-bar-bg">
      <div class="progress-bar-fill" id="progressFill"></div>
    </div>
    <div class="progress-text" id="progressText">0% — 开始打卡吧！</div>
  </div>

  <div class="tip-box" id="tipBox">
    多喝水能促进代谢，皮肤也会变好哦～
  </div>

  <div class="stamp" id="stamp">
    <div class="stamp-text">今日打卡完成 ✓</div>
  </div>
</div>

<!-- 熬夜弹窗 -->
<div class="sleep-warning" id="sleepWarning">
  <div class="sleep-card">
    <div class="big-emoji">🌙</div>
    <h2>该睡觉啦</h2>
    <p>辛亚楠同学<br>现在已经是晚上了<br>放下手机，去睡觉<br>熬夜会掉头发还会变胖哦</p>
    <button class="sleep-btn" onclick="closeSleepWarning()">知道了，这就去睡</button>
  </div>
</div>

<script>
// 显示日期
const now = new Date();
const month = now.getMonth() + 1;
const day = now.getDate();
const weekdays = ['日','一','二','三','四','五','六'];
document.getElementById('dateBox').innerText = `${month}月${day}日 周${weekdays[now.getDay()]} · 健康打卡`;

// 打卡切换
function toggleCheck(el) {
  el.classList.toggle('done');
  updateProgress();
}

// 更新进度
function updateProgress() {
  const items = document.querySelectorAll('.check-item');
  const done = document.querySelectorAll('.check-item.done');
  const percent = Math.round((done.length / items.length) * 100);

  document.getElementById('progressFill').style.width = percent + '%';

  const texts = [
    '0% — 开始打卡吧！',
    '25% — 迈出了第一步 💪',
    '50% —  halfway there！',
    '75% — 就剩一个啦',
    '100% — 今天超棒！🎉'
  ];
  document.getElementById('progressText').innerText = texts[done.length];

  // 全部完成显示印章
  const stamp = document.getElementById('stamp');
  if (done.length === items.length) {
    stamp.style.display = 'block';
  } else {
    stamp.style.display = 'none';
  }
}

// 每日小贴士
const tips = [
  "多喝水能促进代谢，皮肤也会变好哦～",
  "饭后站立 15 分钟，比想象中有效",
  "早睡一小时，第二天效率翻倍",
  "别跷二郎腿，你的脊椎会感谢你",
  "饿了先喝水，有时候只是渴了",
  "周末补觉不能替代规律作息",
  "少吃一口不会死，多吃一口会胖",
  "站起来走走，眼睛也需要休息",
  "不要因为无聊而吃东西",
  "坚持 21 天就能养成一个习惯"
];
const tipIndex = (now.getFullYear() * 365 + now.getMonth() * 31 + now.getDate()) % tips.length;
document.getElementById('tipBox').innerText = tips[tipIndex];

// 熬夜检测：晚上 11 点后弹窗
const hour = now.getHours();
if (hour >= 23 || hour < 5) {
  setTimeout(() => {
    document.getElementById('sleepWarning').classList.add('show');
  }, 1500);
}

function closeSleepWarning() {
  document.getElementById('sleepWarning').classList.remove('show');
}
</script>

</body>
</html>
