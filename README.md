<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>工程數學：終端速度推導</title>
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    <style>
        body { font-family: sans-serif; line-height: 1.6; padding: 20px; max-width: 800px; margin: auto; }
        .highlight { background-color: #f4f4f4; padding: 15px; border-left: 5px solid #333; }
    </style>
</head>
<body>

    <h2>Engineering Mathematics: Terminal Velocity of a Falling Object</h2>
    
    <h3>1. Modeling (Newton's Second Law)</h3>
    <p>根據牛頓第二運動定律，考慮重力與空氣阻力：</p>
    <div class="highlight">
        \[ m \frac{dv}{dt} = mg - cv \]
    </div>

    <h3>2. Solving the Differential Equation</h3>
    <p>使用分離變數法 (Separation of Variables)：</p>
    \[ \frac{m}{mg - cv} dv = dt \]
    
    <p>兩邊同時積分：</p>
    \[ \int \frac{m}{mg - cv} dv = \int dt \]
    
    <p>解得積分結果（考慮初始條件 \( v(0)=0 \)）：</p>
    \[ -\frac{m}{c} \ln(mg - cv) = t + C \]

    <h3>3. Final Velocity Formula</h3>
    <p>最終求得物體隨時間變化的速度公式：</p>
    <div class="highlight" style="color: #d9534f; font-weight: bold;">
        \[ v(t) = \frac{mg}{c} \left( 1 - e^{-\frac{c}{m}t} \right) \]
    </div>

    <p>當 \( t \to \infty \) 時，物體達到終端速度：</p>
    \[ v_{terminal} = \frac{mg}{c} \]

</body>
</html>
