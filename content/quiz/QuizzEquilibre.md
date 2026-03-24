---
title: "QCM: Equilibre général et autres concepts"
layout: "raw"
date: "2026-01-13"
---
<p>3 questions – une ou plusieurs bonnes réponses</p>
<form id="quizForm">

<!-- Q1 -->
<p><b>1.</b> <em>(Examen 2025)</em> Quelle(s) affirmation(s) correspond(ent) au « consommateur rationnel » de ce modèle ?</p>
<input type="checkbox" name="q1" value="A"> A. Il égalise l'utilité marginale de sa consommation en période 1 à celle de la période 2.<br>
<input type="checkbox" name="q1" value="B"> B. Il égalise propension marginale et moyenne.<br>
<input type="checkbox" name="q1" value="C"> C. Il lisse sa consommation entre périodes.<br>
<input type="checkbox" name="q1" value="D"> D. Il ignore le taux d'intérêt.<br>
<input type="checkbox" name="q1" value="E"> E. En moyenne, il anticipe correctement son revenu futur.<br><br>

<!-- Q2 -->
<p><b>2.</b> <em>(Examen 2025)</em> Le premier théorème du bien-être affirme que :</p>
<input type="checkbox" name="q2" value="A"> A. Le bien-être est maximisé sous contraintes budgétaire et technologique.<br>
<input type="checkbox" name="q2" value="B"> B. À l'équilibre, l'offre égale toujours la demande.<br>
<input type="checkbox" name="q2" value="C"> C. Tout équilibre de concurrence parfaite est Pareto-efficient.<br>
<input type="checkbox" name="q2" value="D"> D. Les préférences sont concaves.<br>
<input type="checkbox" name="q2" value="E"> E. En concurrence parfaite, toute intervention ne peut que diminuer le bien-être des agents économiques.<br><br>

<!-- Q3 -->
<p><b>3.</b> <em>(Examen 2025)</em> Quelle(s) affirmation(s) est(sont) vraie(s) à propos de l'équivalence ricardienne  ?</p>
<input type="checkbox" name="q3" value="A"> A. Elle implique que le calendrier des dépenses publiques n'a pas d'importance du point de vue des ménages.<br>
<input type="checkbox" name="q3" value="B"> B. Elle implique que le calendrier des impôts n'a pas d'importance du point de vue des ménages.<br>
<input type="checkbox" name="q3" value="C"> C. Pour qu'elle s'applique, les ménages ne peuvent être soumis à une contrainte d'emprunt.<br>
<input type="checkbox" name="q3" value="D"> D. Pour qu'elle s'applique, les impôts doivent être forfaitaires ou avoir des effets de distorsion.<br>
<input type="checkbox" name="q3" value="E"> E. Pour qu'elle s'applique, les ménages doivent avoir des anticipations rationnelles.<br><br>

<button type="button" onclick="gradeQuiz()">Valider</button>
</form>

<h2 id="result"></h2>

<div id="correction" style="display:none;">
<h3>Correction</h3>
<ol>
  <li>C et E</li>
  <li>C et E</li>
  <li>B, C et E</li>
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
const multiAnswers = {
  q1: ["C", "E"],
  q2: ["C", "E"],
  q3: ["B", "C", "E"]
};

function gradeQuiz() {
  let score = 0;
  const total = Object.keys(multiAnswers).length;

  for (let q in multiAnswers) {
    const correct = multiAnswers[q];
    const checked = Array.from(document.querySelectorAll('input[name="' + q + '"]:checked')).map(el => el.value);
    const isCorrect =
      correct.length === checked.length &&
      correct.every(v => checked.includes(v));
    if (isCorrect) score++;
  }

  document.getElementById("result").innerHTML =
    "Score : <strong>" + score + "/" + total + "</strong>";
  document.getElementById("correction").style.display = "block";
}
</script>