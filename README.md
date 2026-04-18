<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Terminal Velocity</title>

<!-- MathJax（讓公式漂亮） -->
<script src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

<style>
body {
    font-family: Arial, sans-serif;
    line-height: 1.8;
    margin: 40px;
    max-width: 800px;
}

h1, h2, h3 {
    color: #333;
}

.section {
    margin-bottom: 25px;
}

.box {
    background: #f4f4f4;
    padding: 10px;
    border-radius: 8px;
    margin: 10px 0;
}
</style>
</head>

<body>

<h1>Engineering Mathematics: Terminal Velocity of a Falling Object</h1>

<div class="section">
<h2>Problem</h2>
<p>How does the velocity of an object change as it falls through air?</p>
</div>

<div class="section">
<h2>Modeling (Newton’s Second Law)</h2>
<ul>
<li>Gravity: \( mg \)</li>
<li>Air resistance: \( cv \)</li>
</ul>

<div class="box">
\( m \frac{dv}{dt} = mg - cv \)
</div>
</div>

<div class="section">
<h2>Solving the Differential Equation</h2>

<h3>1. Rewrite</h3>
<div class="box">
\( \frac{dv}{dt} = g - \frac{c}{m}v \)
</div>

<h3>2. Separate Variables</h3>
<div class="box">
\( \frac{dv}{g - \frac{c}{m}v} = dt \)
</div>

<h3>3. Integrate</h3>
<div class="box">
\( -\frac{m}{c} \ln\left(g - \frac{c}{m}v\right) = t + C \)
</div>

<h3>4. Rearrange</h3>
<div class="box">
\( g - \frac{c}{m}v = Ae^{-\frac{c}{m}t} \)
</div>

<h3>5. Solve for \( v(t) \)</h3>
<div class="box">
\( v(t) = \frac{mg}{c}\left(1 - Ae^{-\frac{c}{m}t}\right) \)
</div>

<h3>6. Initial Condition</h3>
<div class="box">
\( v(0)=0 \Rightarrow A=1 \)
</div>

</div>

<div class="section">
<h2>Final Answer</h2>
<div class="box">
\( v(t) = \frac{mg}{c}\left(1 - e^{-\frac{c}{m}t}\right) \)
</div>
</div>

<div class="section">
<h2>Physical Interpretation</h2>
<ul>
<li>As \( t \to \infty \), velocity approaches terminal velocity: \( \frac{mg}{c} \)</li>
<li>Initially accelerates</li>
<li>Acceleration decreases over time</li>
<li>Eventually reaches constant speed</li>
</ul>
</div>

</body>
</html>
</body>
</html>
