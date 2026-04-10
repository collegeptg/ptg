<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>भारतीय संविधान प्रश्नोत्तरी</title>
<link href="https://fonts.googleapis.com/css2?family=Tiro+Devanagari+Hindi:ital@0;1&family=Baloo+2:wght@400;600;700;800&display=swap" rel="stylesheet">
<style>
  :root {
    --saffron: #FF6B1A;
    --deep-saffron: #E85D04;
    --green: #138808;
    --deep-green: #0a5c05;
    --navy: #1a1a5e;
    --gold: #F4C430;
    --light-gold: #fff8e7;
    --white: #ffffff;
    --bg: #f5f0e8;
    --correct: #138808;
    --wrong: #c0392b;
    --card-shadow: 0 8px 32px rgba(26,26,94,0.13);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'Baloo 2', 'Tiro Devanagari Hindi', sans-serif;
    background: var(--bg);
    min-height: 100vh;
    background-image:
      radial-gradient(circle at 10% 20%, rgba(255,107,26,0.08) 0%, transparent 50%),
      radial-gradient(circle at 90% 80%, rgba(19,136,8,0.08) 0%, transparent 50%);
  }

  /* HEADER */
  .header {
    background: linear-gradient(135deg, var(--navy) 0%, #2d2d8a 100%);
    color: white;
    padding: 18px 20px 14px;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  .header::before {
    content: '';
    position: absolute; top: 0; left: 0; right: 0;
    height: 5px;
    background: linear-gradient(90deg, var(--saffron) 33%, white 33%, white 66%, var(--green) 66%);
  }
  .header-ashoka {
    font-size: 2rem;
    margin-bottom: 4px;
  }
  .header h1 {
    font-size: 1.3rem;
    font-weight: 800;
    letter-spacing: 0.5px;
    text-shadow: 0 2px 8px rgba(0,0,0,0.3);
  }
  .header p {
    font-size: 0.82rem;
    opacity: 0.85;
    margin-top: 3px;
  }
  .tricolor-bar {
    height: 4px;
    background: linear-gradient(90deg, var(--saffron) 33%, white 33%, white 66%, var(--green) 66%);
    margin-top: 14px;
  }

  /* MAIN CONTAINER */
  .container {
    max-width: 600px;
    margin: 0 auto;
    padding: 16px 14px 40px;
  }

  /* STEP INDICATOR */
  .steps {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0;
    margin: 16px 0 20px;
  }
  .step-dot {
    width: 36px; height: 36px;
    border-radius: 50%;
    display: flex; align-items: center; justify-content: center;
    font-weight: 800; font-size: 0.95rem;
    border: 3px solid #ccc;
    background: white;
    color: #aaa;
    transition: all 0.3s;
    position: relative;
    z-index: 1;
  }
  .step-dot.active { border-color: var(--saffron); color: var(--saffron); background: #fff5f0; }
  .step-dot.done { border-color: var(--green); background: var(--green); color: white; }
  .step-line {
    flex: 1; height: 3px; background: #ddd; max-width: 80px;
    transition: background 0.3s;
  }
  .step-line.done { background: var(--green); }
  .step-label {
    display: flex; justify-content: space-around;
    font-size: 0.72rem; color: #888; margin-top: 4px;
    font-weight: 600;
  }

  /* CARD */
  .card {
    background: white;
    border-radius: 18px;
    padding: 24px 20px;
    box-shadow: var(--card-shadow);
    margin-bottom: 16px;
    border: 1.5px solid rgba(26,26,94,0.07);
  }
  .card-title {
    color: var(--navy);
    font-size: 1.1rem;
    font-weight: 800;
    margin-bottom: 18px;
    padding-bottom: 10px;
    border-bottom: 2px solid var(--light-gold);
    display: flex; align-items: center; gap: 8px;
  }

  /* FORM FIELDS */
  .field { margin-bottom: 16px; }
  .field label {
    display: block;
    font-size: 0.85rem;
    font-weight: 700;
    color: var(--navy);
    margin-bottom: 6px;
  }
  .field input, .field select {
    width: 100%;
    padding: 12px 14px;
    border: 2px solid #e0ddd5;
    border-radius: 10px;
    font-size: 0.95rem;
    font-family: 'Baloo 2', sans-serif;
    color: #333;
    background: #fafaf8;
    transition: border-color 0.2s, box-shadow 0.2s;
    outline: none;
    -webkit-appearance: none;
  }
  .field input:focus, .field select:focus {
    border-color: var(--saffron);
    box-shadow: 0 0 0 3px rgba(255,107,26,0.12);
    background: white;
  }

  /* BUTTONS */
  .btn {
    width: 100%;
    padding: 15px;
    border: none;
    border-radius: 12px;
    font-size: 1.05rem;
    font-weight: 800;
    font-family: 'Baloo 2', sans-serif;
    cursor: pointer;
    transition: all 0.2s;
    letter-spacing: 0.3px;
  }
  .btn-primary {
    background: linear-gradient(135deg, var(--saffron), var(--deep-saffron));
    color: white;
    box-shadow: 0 4px 16px rgba(255,107,26,0.35);
  }
  .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 6px 20px rgba(255,107,26,0.45); }
  .btn-primary:active { transform: translateY(0); }
  .btn-submit {
    background: linear-gradient(135deg, var(--green), var(--deep-green));
    color: white;
    box-shadow: 0 4px 16px rgba(19,136,8,0.35);
  }
  .btn-submit:hover { transform: translateY(-2px); }

  /* QUESTION CARD */
  .question-card {
    background: white;
    border-radius: 16px;
    padding: 20px 18px;
    box-shadow: var(--card-shadow);
    margin-bottom: 14px;
    border-left: 5px solid var(--saffron);
    transition: border-color 0.3s;
  }
  .question-card.answered { border-left-color: var(--navy); }
  .q-number {
    font-size: 0.72rem;
    font-weight: 800;
    color: var(--saffron);
    text-transform: uppercase;
    letter-spacing: 1px;
    margin-bottom: 6px;
  }
  .q-text {
    font-size: 1rem;
    font-weight: 700;
    color: var(--navy);
    line-height: 1.5;
    margin-bottom: 14px;
  }
  .options { display: flex; flex-direction: column; gap: 8px; }
  .option {
    display: flex; align-items: center; gap: 10px;
    padding: 11px 14px;
    border-radius: 10px;
    border: 2px solid #ece9e0;
    cursor: pointer;
    transition: all 0.18s;
    background: #fafaf8;
  }
  .option:hover { border-color: var(--saffron); background: #fff5f0; }
  .option input[type="radio"] { display: none; }
  .option-bubble {
    width: 22px; height: 22px; min-width: 22px;
    border-radius: 50%;
    border: 2px solid #ccc;
    display: flex; align-items: center; justify-content: center;
    font-size: 0.65rem;
    font-weight: 800;
    transition: all 0.18s;
    background: white;
    color: #999;
  }
  .option.selected { border-color: var(--navy); background: #f0f0ff; }
  .option.selected .option-bubble { border-color: var(--navy); background: var(--navy); color: white; }
  .option-text { font-size: 0.92rem; color: #333; font-weight: 600; line-height: 1.4; }

  /* RESULTS */
  .result-hero {
    background: linear-gradient(135deg, var(--navy), #2d2d8a);
    border-radius: 18px;
    padding: 28px 20px;
    text-align: center;
    color: white;
    margin-bottom: 16px;
    position: relative;
    overflow: hidden;
  }
  .result-hero::before {
    content: '';
    position: absolute; top: 0; left: 0; right: 0; height: 4px;
    background: linear-gradient(90deg, var(--saffron) 33%, white 33%, white 66%, var(--green) 66%);
  }
  .result-score {
    font-size: 4rem;
    font-weight: 800;
    color: var(--gold);
    line-height: 1;
    text-shadow: 0 0 20px rgba(244,196,48,0.5);
  }
  .result-total { font-size: 1rem; opacity: 0.8; margin: 4px 0 12px; }
  .result-msg { font-size: 1.1rem; font-weight: 700; }
  .result-grade {
    display: inline-block;
    padding: 4px 16px;
    border-radius: 20px;
    font-size: 0.85rem;
    font-weight: 800;
    margin-top: 10px;
  }
  .grade-a { background: var(--gold); color: var(--navy); }
  .grade-b { background: #27ae60; color: white; }
  .grade-c { background: var(--saffron); color: white; }
  .grade-d { background: #c0392b; color: white; }

  .participant-info-card {
    background: var(--light-gold);
    border-radius: 12px;
    padding: 14px 16px;
    margin-bottom: 16px;
    border: 1.5px solid var(--gold);
  }
  .participant-info-card p {
    font-size: 0.85rem;
    color: var(--navy);
    font-weight: 600;
    margin-bottom: 4px;
  }
  .participant-info-card span { font-weight: 800; }

  /* ANSWER KEY */
  .answer-card {
    background: white;
    border-radius: 14px;
    padding: 16px;
    margin-bottom: 10px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.06);
    border-left: 4px solid #ddd;
  }
  .answer-card.correct-ans { border-left-color: var(--correct); }
  .answer-card.wrong-ans { border-left-color: var(--wrong); }
  .ans-q { font-size: 0.88rem; font-weight: 700; color: var(--navy); margin-bottom: 8px; line-height: 1.4; }
  .ans-row { display: flex; flex-direction: column; gap: 4px; }
  .ans-label { font-size: 0.78rem; font-weight: 700; }
  .ans-value { font-size: 0.85rem; font-weight: 600; padding: 5px 10px; border-radius: 7px; }
  .your-ans { background: #ffeaea; color: var(--wrong); }
  .your-ans.correct-choice { background: #e8f8e8; color: var(--correct); }
  .correct-ans-val { background: #e8f8e8; color: var(--correct); }
  .tick { color: var(--correct); font-size: 1.1rem; }
  .cross { color: var(--wrong); font-size: 1.1rem; }

  /* PROGRESS BAR */
  .progress-wrap { margin-bottom: 18px; }
  .progress-info { display: flex; justify-content: space-between; font-size: 0.78rem; font-weight: 700; color: #888; margin-bottom: 5px; }
  .progress-bar { height: 6px; background: #e0ddd5; border-radius: 10px; overflow: hidden; }
  .progress-fill { height: 100%; background: linear-gradient(90deg, var(--saffron), var(--deep-saffron)); border-radius: 10px; transition: width 0.3s; }

  .section-label {
    font-size: 0.78rem;
    font-weight: 800;
    letter-spacing: 1.5px;
    color: var(--saffron);
    text-transform: uppercase;
    margin-bottom: 12px;
    margin-top: 4px;
  }
  .hidden { display: none !important; }
  .error-msg { color: var(--wrong); font-size: 0.82rem; margin-top: 8px; font-weight: 700; text-align: center; }
  .retake-btn { margin-top: 10px; background: var(--navy); color: white; box-shadow: 0 4px 16px rgba(26,26,94,0.3); }
</style>
</head>
<body>

<div class="header">
  <div class="header-ashoka">🪷</div>
  <h1>भारतीय संविधान प्रश्नोत्तरी</h1>
  <p>ऑनलाइन परीक्षा • 20 प्रश्न</p>
  <div class="tricolor-bar"></div>
</div>

<div class="container">

  <!-- STEP INDICATOR -->
  <div>
    <div class="steps" id="stepIndicator">
      <div class="step-dot active" id="dot1">1</div>
      <div class="step-line" id="line1"></div>
      <div class="step-dot" id="dot2">2</div>
      <div class="step-line" id="line2"></div>
      <div class="step-dot" id="dot3">✓</div>
    </div>
    <div class="step-label">
      <span>प्रतिभागी जानकारी</span>
      <span>प्रश्नोत्तरी</span>
      <span>परिणाम</span>
    </div>
  </div>

  <!-- STEP 1: PARTICIPANT DETAILS -->
  <div id="step1">
    <div class="card">
      <div class="card-title">🎓 प्रतिभागी की जानकारी भरें</div>
      <div class="field">
        <label>👤 प्रतिभागी का नाम *</label>
        <input type="text" id="pName" placeholder="अपना पूरा नाम लिखें" />
      </div>
      <div class="field">
        <label>🏫 महाविद्यालय / विद्यालय का नाम *</label>
        <input type="text" id="pCollege" placeholder="अपने महाविद्यालय का नाम लिखें" />
      </div>
      <div class="field">
        <label>📍 जिले का नाम *</label>
        <input type="text" id="pDistrict" placeholder="अपने जिले का नाम लिखें" />
      </div>
      <div id="step1Error" class="error-msg hidden">⚠️ कृपया सभी जानकारी भरें।</div>
      <br>
      <button class="btn btn-primary" onclick="goToStep2()">आगे बढ़ें — प्रश्नोत्तरी शुरू करें →</button>
    </div>
  </div>

  <!-- STEP 2: QUIZ -->
  <div id="step2" class="hidden">
    <div class="progress-wrap">
      <div class="progress-info">
        <span id="progressText">0 / 20 उत्तर दिए</span>
        <span id="progressPct">0%</span>
      </div>
      <div class="progress-bar"><div class="progress-fill" id="progressFill" style="width:0%"></div></div>
    </div>

    <div id="questionsContainer"></div>

    <div id="submitError" class="error-msg hidden">⚠️ कृपया सभी 20 प्रश्नों के उत्तर दें।</div>
    <br>
    <button class="btn btn-submit" onclick="submitQuiz()">📝 उत्तर जमा करें — परिणाम देखें</button>
  </div>

  <!-- STEP 3: RESULT -->
  <div id="step3" class="hidden">
    <div class="result-hero" id="resultHero">
      <div style="font-size:2.5rem;margin-bottom:8px;" id="resultEmoji">🏆</div>
      <div class="result-score" id="scoreDisplay">0</div>
      <div class="result-total">20 में से</div>
      <div class="result-msg" id="resultMsg"></div>
      <div class="result-grade" id="resultGrade"></div>
    </div>

    <div class="participant-info-card">
      <p>👤 नाम: <span id="r_name"></span></p>
      <p>🏫 महाविद्यालय: <span id="r_college"></span></p>
      <p>📍 जिला: <span id="r_district"></span></p>
      <p>📅 दिनांक: <span id="r_date"></span></p>
    </div>

    <div class="section-label">📋 उत्तर पुस्तिका</div>
    <div id="answerKey"></div>

    <button class="btn retake-btn" onclick="retake()">🔄 फिर से प्रयास करें</button>
  </div>

</div>

<script>
const questions = [
  { q: "भारतीय संविधान कब लागू हुआ?", opts: ["26 जनवरी 1947","26 जनवरी 1950","15 अगस्त 1947","2 अक्टूबर 1950"], ans: 1 },
  { q: "संविधान सभा के अध्यक्ष कौन थे?", opts: ["डॉ. राजेन्द्र प्रसाद","जवाहरलाल नेहरू","डॉ. अम्बेडकर","सरदार पटेल"], ans: 0 },
  { q: "संविधान के निर्माता किसे कहा जाता है?", opts: ["महात्मा गांधी","डॉ. बी. आर. अम्बेडकर","नेहरू","पटेल"], ans: 1 },
  { q: "भारतीय संविधान का सबसे बड़ा स्रोत क्या है?", opts: ["ब्रिटिश संविधान","अमेरिकी संविधान","भारत सरकार अधिनियम 1935","फ्रांसीसी संविधान"], ans: 2 },
  { q: "भारत का संविधान किस प्रकार का है?", opts: ["कठोर","लचीला","अर्ध-कठोर और अर्ध-लचीला","इनमें से कोई नहीं"], ans: 2 },
  { q: "प्रस्तावना में 'समाजवादी' शब्द कब जोड़ा गया?", opts: ["1950","1976 (42वाँ संशोधन)","1962","1980"], ans: 1 },
  { q: "भारतीय संविधान की प्रस्तावना किससे प्रेरित है?", opts: ["ब्रिटिश संविधान","अमेरिकी संविधान","फ्रांसीसी संविधान","कनाडा"], ans: 1 },
  { q: "संविधान का संरक्षक कौन है?", opts: ["राष्ट्रपति","प्रधानमंत्री","सर्वोच्च न्यायालय","संसद"], ans: 2 },
  { q: "भारत में कितने मूल अधिकार हैं?", opts: ["5","6","7","8"], ans: 1 },
  { q: "किस अनुच्छेद में समानता का अधिकार है?", opts: ["अनुच्छेद 14-18","19-22","23-24","25-28"], ans: 0 },
  { q: "शिक्षा का अधिकार किस अनुच्छेद में है?", opts: ["19","21A","25","32"], ans: 1 },
  { q: "संविधान में मौलिक कर्तव्य कब जोड़े गए?", opts: ["1950","1976 (42वाँ संशोधन)","1985","1991"], ans: 1 },
  { q: "मौलिक कर्तव्यों की संख्या कितनी है?", opts: ["10","11","12","9"], ans: 1 },
  { q: "राज्य नीति के निदेशक तत्व किस देश से लिए गए हैं?", opts: ["अमेरिका","आयरलैंड","ब्रिटेन","फ्रांस"], ans: 1 },
  { q: "राष्ट्रपति का चुनाव कौन करता है?", opts: ["जनता","संसद","निर्वाचक मंडल","प्रधानमंत्री"], ans: 2 },
  { q: "प्रधानमंत्री की नियुक्ति कौन करता है?", opts: ["राष्ट्रपति","संसद","जनता","न्यायालय"], ans: 0 },
  { q: "संसद के कितने सदन हैं?", opts: ["1","2","3","4"], ans: 1 },
  { q: "लोकसभा का कार्यकाल कितना होता है?", opts: ["4 वर्ष","5 वर्ष","6 वर्ष","7 वर्ष"], ans: 1 },
  { q: "सर्वोच्च न्यायालय के मुख्य न्यायाधीश की नियुक्ति कौन करता है?", opts: ["प्रधानमंत्री","राष्ट्रपति","संसद","राज्यपाल"], ans: 1 },
  { q: "राष्ट्रपति शासन किस अनुच्छेद में है?", opts: ["352","356","360","370"], ans: 1 },
];

const labels = ['A','B','C','D'];
let userAnswers = new Array(questions.length).fill(null);
let participantData = {};

function buildQuiz() {
  const container = document.getElementById('questionsContainer');
  container.innerHTML = '';
  questions.forEach((q, qi) => {
    const card = document.createElement('div');
    card.className = 'question-card';
    card.id = 'qcard_' + qi;
    let optsHTML = q.opts.map((opt, oi) => `
      <label class="option" id="opt_${qi}_${oi}" onclick="selectOption(${qi}, ${oi})">
        <input type="radio" name="q${qi}" value="${oi}">
        <div class="option-bubble">${labels[oi]}</div>
        <span class="option-text">${opt}</span>
      </label>
    `).join('');
    card.innerHTML = `
      <div class="q-number">प्रश्न ${qi+1} / 20</div>
      <div class="q-text">${q.q}</div>
      <div class="options">${optsHTML}</div>
    `;
    container.appendChild(card);
  });
}

function selectOption(qi, oi) {
  // Deselect all options for this question
  questions[qi].opts.forEach((_, idx) => {
    const el = document.getElementById(`opt_${qi}_${idx}`);
    if(el) el.classList.remove('selected');
  });
  // Select chosen
  const chosen = document.getElementById(`opt_${qi}_${oi}`);
  if(chosen) chosen.classList.add('selected');
  userAnswers[qi] = oi;
  // Mark card as answered
  const card = document.getElementById('qcard_' + qi);
  if(card) card.classList.add('answered');
  updateProgress();
}

function updateProgress() {
  const answered = userAnswers.filter(a => a !== null).length;
  const pct = Math.round((answered / 20) * 100);
  document.getElementById('progressText').textContent = `${answered} / 20 उत्तर दिए`;
  document.getElementById('progressPct').textContent = pct + '%';
  document.getElementById('progressFill').style.width = pct + '%';
}

function goToStep2() {
  const name = document.getElementById('pName').value.trim();
  const college = document.getElementById('pCollege').value.trim();
  const district = document.getElementById('pDistrict').value.trim();
  if (!name || !college || !district) {
    document.getElementById('step1Error').classList.remove('hidden');
    return;
  }
  participantData = { name, college, district };
  document.getElementById('step1Error').classList.add('hidden');
  document.getElementById('step1').classList.add('hidden');
  document.getElementById('step2').classList.remove('hidden');
  buildQuiz();
  // Update step indicator
  document.getElementById('dot1').className = 'step-dot done';
  document.getElementById('dot2').className = 'step-dot active';
  document.getElementById('line1').className = 'step-line done';
  window.scrollTo(0,0);
}

function submitQuiz() {
  const unanswered = userAnswers.filter(a => a === null).length;
  if (unanswered > 0) {
    document.getElementById('submitError').classList.remove('hidden');
    // Scroll to first unanswered
    const firstUnanswered = userAnswers.findIndex(a => a === null);
    document.getElementById('qcard_' + firstUnanswered).scrollIntoView({ behavior: 'smooth', block: 'center' });
    return;
  }
  document.getElementById('submitError').classList.add('hidden');
  showResults();
}

function showResults() {
  // Calculate score
  let score = 0;
  userAnswers.forEach((ans, i) => { if (ans === questions[i].ans) score++; });

  // Update step indicator
  document.getElementById('dot2').className = 'step-dot done';
  document.getElementById('dot3').className = 'step-dot done';
  document.getElementById('line2').className = 'step-line done';

  document.getElementById('step2').classList.add('hidden');
  document.getElementById('step3').classList.remove('hidden');
  window.scrollTo(0,0);

  // Score display
  document.getElementById('scoreDisplay').textContent = score;

  // Grade & message
  let emoji, msg, grade, gradeClass;
  const pct = (score / 20) * 100;
  if (pct >= 90) { emoji='🏆'; msg='अत्यंत उत्कृष्ट! शाबाश!'; grade='ग्रेड A+'; gradeClass='grade-a'; }
  else if (pct >= 75) { emoji='🥇'; msg='बहुत अच्छा प्रदर्शन!'; grade='ग्रेड A'; gradeClass='grade-a'; }
  else if (pct >= 60) { emoji='🥈'; msg='अच्छा प्रयास! और पढ़ें।'; grade='ग्रेड B'; gradeClass='grade-b'; }
  else if (pct >= 40) { emoji='🥉'; msg='ठीक है। और अभ्यास करें।'; grade='ग्रेड C'; gradeClass='grade-c'; }
  else { emoji='📚'; msg='और मेहनत करें। आप कर सकते हैं!'; grade='ग्रेड D'; gradeClass='grade-d'; }

  document.getElementById('resultEmoji').textContent = emoji;
  document.getElementById('resultMsg').textContent = msg;
  document.getElementById('resultGrade').textContent = grade;
  document.getElementById('resultGrade').className = 'result-grade ' + gradeClass;

  // Participant info
  document.getElementById('r_name').textContent = participantData.name;
  document.getElementById('r_college').textContent = participantData.college;
  document.getElementById('r_district').textContent = participantData.district;
  document.getElementById('r_date').textContent = new Date().toLocaleDateString('hi-IN', {day:'numeric',month:'long',year:'numeric'});

  // Answer key
  const keyContainer = document.getElementById('answerKey');
  keyContainer.innerHTML = '';
  questions.forEach((q, i) => {
    const ua = userAnswers[i];
    const correct = q.ans;
    const isCorrect = ua === correct;
    const card = document.createElement('div');
    card.className = `answer-card ${isCorrect ? 'correct-ans' : 'wrong-ans'}`;

    let yourAnsHTML = `<div class="ans-value your-ans ${isCorrect ? 'correct-choice' : ''}">
      ${isCorrect ? '✅' : '❌'} आपका उत्तर: ${labels[ua]}. ${q.opts[ua]}
    </div>`;

    let correctAnsHTML = isCorrect ? '' : `<div class="ans-value correct-ans-val">
      ✅ सही उत्तर: ${labels[correct]}. ${q.opts[correct]}
    </div>`;

    card.innerHTML = `
      <div class="ans-q">प्र. ${i+1}: ${q.q}</div>
      <div class="ans-row">${yourAnsHTML}${correctAnsHTML}</div>
    `;
    keyContainer.appendChild(card);
  });

  // Save to localStorage
  try {
    const record = {
      name: participantData.name,
      college: participantData.college,
      district: participantData.district,
      score,
      total: 20,
      date: new Date().toISOString(),
      answers: userAnswers
    };
    const existing = JSON.parse(localStorage.getItem('quizRecords') || '[]');
    existing.push(record);
    localStorage.setItem('quizRecords', JSON.stringify(existing));
  } catch(e) {}
}

function retake() {
  userAnswers = new Array(questions.length).fill(null);
  document.getElementById('step3').classList.add('hidden');
  document.getElementById('step1').classList.remove('hidden');
  document.getElementById('dot1').className = 'step-dot active';
  document.getElementById('dot2').className = 'step-dot';
  document.getElementById('dot3').className = 'step-dot';
  document.getElementById('line1').className = 'step-line';
  document.getElementById('line2').className = 'step-line';
  document.getElementById('pName').value = '';
  document.getElementById('pCollege').value = '';
  document.getElementById('pDistrict').value = '';
  window.scrollTo(0,0);
}
</script>
</body>
</html>
