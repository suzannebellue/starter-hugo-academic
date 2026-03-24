---
title: "QCM: PIB & Mesure du niveau de vie"
layout: "raw"
date: "2026-01-18"
---
<p>4 questions – une ou plusieurs bonnes réponses</p>
<form id="quizForm">

<!-- Q1 -->
<p><b>1.</b> Le PIB nominal se distingue du PIB réel parce que :</p>
<input type="checkbox" name="q1" value="A"> A. Le PIB nominal est évalué aux prix courants de l'année considérée.<br>
<input type="checkbox" name="q1" value="B"> B. Le PIB réel est corrigé de l'inflation.<br>
<input type="checkbox" name="q1" value="C"> C. Le PIB nominal exclut les biens durables.<br>
<input type="checkbox" name="q1" value="D"> D. Le PIB réel utilise un indice chaîné.<br>
<input type="checkbox" name="q1" value="E"> E. Le PIB nominal tient compte des variations de parité de pouvoir d'achat.<br><br>

<!-- Q2 -->
<p><b>2.</b> <em>(Examen 2025)</em> Le PIB peut être mesuré par trois approches équivalentes. Lesquelles ? </p>
<input type="checkbox" name="q2" value="A"> A. Approche production.<br>
<input type="checkbox" name="q2" value="B"> B. Approche investissement.<br>
<input type="checkbox" name="q2" value="C"> C. Approche dépense.<br>
<input type="checkbox" name="q2" value="D"> D. Approche monétaire.<br>
<input type="checkbox" name="q2" value="E"> E. Approche revenus.<br><br>

<!-- Q3 -->
<p><b>3.</b> <em>(Examen 2025)</em> Quelle limite du PIB la mesure structurelle du niveau de vie (Jones &amp; Klenow) cherche-t-elle avant tout à corriger ? </p>
<input type="checkbox" name="q3" value="A"> A. L'exclusion des services publics.<br>
<input type="checkbox" name="q3" value="B"> B. L'absence de prise en compte des inégalités.<br>
<input type="checkbox" name="q3" value="C"> C. L'omission de la qualité de l'environnement.<br>
<input type="checkbox" name="q3" value="D"> D. La non-prise en compte des loisirs.<br>
<input type="checkbox" name="q3" value="E"> E. La difficulté à mesurer l'économie informelle.<br><br>

<!-- Q4 -->
<p><b>4.</b> <em>(Examen 2025)</em> Laquelle ou lesquelles des observations suivantes seraient utiles pour déterminer la pondération de l'espérance de vie dans le bien-être ?</p>
<input type="checkbox" name="q4" value="A"> A. Observer les variations d'espérance de vie entre les personnes ayant différents niveaux de revenus au sein d'un même pays.<br>
<input type="checkbox" name="q4" value="B"> B. Observer les variations d'espérance de vie entre les pays.<br>
<input type="checkbox" name="q4" value="C"> C. Observer le montant que les gens sont prêts à payer pour les obsèques.<br>
<input type="checkbox" name="q4" value="D"> D. Observer les différences de prix de l'immobilier entre les quartiers présentant des taux de criminalité différents.<br><br>

<button type="button" onclick="gradeQuiz()">Valider</button>
</form>

<h2 id="result"></h2>

<div id="correction" style="display:none;">
<h3>Correction</h3>
<ol>
  <li>A et B</li>
  <li>A, C et E</li>
  <li>B et D</li>
  <li>D</li>
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
// Définition des bonnes réponses (toutes multi-choix)
const correctAnswers = {
  q1: ["A", "B"],
  q2: ["A", "C", "E"],
  q3: ["B", "D"],
  q4: ["D"]
};

function gradeQuiz() {
  let score = 0;
  const total = Object.keys(correctAnswers).length;

  for (let q in correctAnswers) {
    const correct = correctAnswers[q];
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
