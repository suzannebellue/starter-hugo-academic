---
title: "QCM: Investissement"
layout: "raw"
date: "2026-01-14"
---

<p>3 questions – une ou plusieure bonnes réponses</p>

<form id="quizForm">

<!-- Q1 -->
<p><b>1.</b> Projet rentable si :</p>
<input type="radio" name="q1" value="A"> A. VAN&lt;0<br>
<input type="radio" name="q1" value="B"> B. VAN=0<br>
<input type="radio" name="q1" value="C"> C. VAN&gt;0<br>
<input type="radio" name="q1" value="D"> D. r=0<br><br>

<!-- Q2 -->
<p><b>2.</b>Quelle est la condition d'équilibre sur le marché de l'investissement ?</p>
<input type="radio" name="q2" value="A"> A. F<sub>K</sub>=r<br>
<input type="radio" name="q2" value="B"> B. F<sub>K</sub>−δ=r<br>
<input type="radio" name="q2" value="C"> C. F<sub>K</sub>=δ<br>
<input type="radio" name="q2" value="D"> D. r=s<br><br>


<!-- Q3 — plusieurs bonnes réponses : checkboxes -->
<p><b>3.</b> <em>(Examen 2025)</em> La valeur actuelle nette d’un projet est positive si :</p>
<input type="checkbox" name="q3" value="A"> A. Le taux d'intérêt est nul<br>
<input type="checkbox" name="q3" value="B"> B. Les flux sont constants<br>
<input type="checkbox" name="q3" value="C"> C. Les flux futurs sont positifs<br>
<input type="checkbox" name="q3" value="D"> D. L'investissement est autofinancé<br>
<input type="checkbox" name="q3" value="E"> E. La somme actualisée des flux dépasse le coût initial<br><br>
  
<button type="button" onclick="gradeQuiz()">Valider</button>

</form>

<h2 id="result"></h2>

<div id="correction" style="display:none;">
<h3>Correction</h3>
<ol>
<li>C</li>
<li>B</li>
<li>E</li>
</ol>
</div>

<p>
  <a href="/quiz/" style="
    display:inline-block;
    padding:10px 18px;
    background-color:#2c3e50;
    color:white;
    text-decoration:none;
    border-radius:6px;
    font-weight:bold;
  ">
    Retour
  </a>
</p>

<script>
function gradeQuiz() {
  const singleAnswers = {
  q1:"C", q2:"B"
  };

  let score = 0;

  for (let q in singleAnswers) {
    const selected = document.querySelector('input[name="' + q + '"]:checked');
    if (selected && selected.value === singleAnswers[q]) {
      score++;
    }
  }

  // Correction de la Q3 (checkboxes, plusieurs bonnes réponses)
  const correctQ3 = ["E"];
  const checkedQ3 = Array.from(document.querySelectorAll('input[name="q3"]:checked')).map(el => el.value);
  const isCorrectQ3 =
    correctQ3.length === checkedQ3.length &&
    correctQ3.every(v => checkedQ3.includes(v));
  if (isCorrectQ3) score++;


  document.getElementById("result").innerHTML =
    "Score : <strong>" + score + "/3</strong>";

  document.getElementById("correction").style.display = "block";
}

</script>

