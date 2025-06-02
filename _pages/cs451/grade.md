---
permalink: "/cs451/grade.html"
layout: cs451_page
title: What's My Grade?
exclude: true
---

<div class="aside">
    <div class="container-fluid">
      <span><b>Programming Assignments</b></span>
      <table class="table">
        <thead>
          <tr class="row">
            <th scope="col" class="text-center col-1">1</th>
            <th scope="col" class="text-center col-1">2</th>
            <th scope="col" class="text-center col-1">3</th>
            <th scope="col" class="text-center col-1">4</th>
            <th scope="col" class="text-center col-1">5</th>
            <th scope="col" class="text-center col-1">6</th>
          </tr>
        </thead>
        <tr class="row">
          <td class="col-1">
            <input id="pa1" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="pa2" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="pa3" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="pa4" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="pa5" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="pa6" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
        </tr>
      </table>
      <p/>
      <span><b>Exams</b></span>
      <table class="table">
        <thead>
          <tr class="row">
            <th scope="col" class="text-center col-1">1</th>
            <th scope="col" class="text-center col-1">2</th>
          </tr>
        </thead>
        <tr class="row">
          <td class="col-1">
            <input id="exam1" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="exam2" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
        </tr>
      </table>
      <p/>
    <p/>
    <span><b>Participation</b> (based on in-class quizzes)</span>
    <table>
    <tr>
    <td>
    <input id="participation" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
    </td>
    </tr>
    </table>
    <p/>
    <p/>
    <span><b>Course Evaluation</b></span>
    <table>
    <tr>
    <td>
    <input id="eval" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
    </td>
    </tr>
    </table>
    <p/>
    <p/>
    <input class="btn btn-info" type="button" value="Calculate My Grade" onclick="grade()"/>
    <p/>
      <div class="scores"></div>
      <p/>
      <h2><div class="grade"></div></h2>
      <div class="disclaimer"></div>
    </div>
    <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"
            integrity="sha384-KJ3o2DKtIkvYIK3UENzmM7KCkRr/rE9/Qpg6aAZGJwFDMVNA/GpGFF93hXpG5KkN"
            crossorigin="anonymous">
    </script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js"
            integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q"
            crossorigin="anonymous">
    </script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"
            integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl"
            crossorigin="anonymous">
    </script>
      <script type="text/javascript">
// Return an object containing the assessment types and counts.
function assessments() {
    var assessments = new Object();
    assessments.assignment = 6;
    assessments.exam = 2;
    assessments.participation = 1;
    assessments.evals = 1;
    return assessments;
}

// Return an object containing weights for calculating student grade.
function weights() {
    var weights = new Object();
    weights.assignment = 6;
    weights.exam = 30;
    weights.participation = 10;
    weights.evals = 1; 
    return weights;
}

// Return letter grade corresponding to the specified percentage score
function score2grade(score) {
    if (score < 60) {
        return "F";
    }
    else if (score < 63) {
        return "D-";
    }
    else if (score < 67) {
        return "D";
    }
    else if (score < 70) {
        return "D+";
    }
    else if (score < 73) {
        return "C-";
    }
    else if (score < 77) {
        return "C";
    }
    else if (score < 80) {
        return "C+";
    }
    else if (score < 83) {
        return "B-";
    }
    else if (score < 87) {
        return "B";
    }
    else if (score < 90) {
        return "B+";
    }
    else if (score < 93) {
        return "A-";
    }
    else if (score < 100) {
        return "A";
    }
    else {
        return "A+";
    }
}

// Return true if score is within half-a-point of a grade boundary, and false otherwise.
function borderline(score) {
    return score >= 92.5 && score < 93 || 
        score >= 89.5 && score < 90 ||
        score >= 86.5 && score < 87 ||
        score >= 82.5 && score < 83 ||
        score >= 79.5 && score < 80 ||
        score >= 76.5 && score < 77 ||
        score >= 72.5 && score < 73 ||
        score >= 69.5 && score < 70 ||
        score >= 66.5 && score < 67 ||
        score >= 62.5 && score < 63 ||
        score >= 59.5 && score < 60;
}

// Return the non-NaN elements of the list a as a list of floats.
function graded(a) {
    return a.filter(Boolean).map(function(item) {return parseFloat(item)});
}

// Return the sum of the values in the list a.
function sum(a) {
    return a.reduce(function(x, y) {return x + y});
}

function grade() {
    var scores = new Object();
    scores.assignment = [];
    scores.assignment.push($("#pa1").val());
    scores.assignment.push($("#pa2").val());
    scores.assignment.push($("#pa3").val());
    scores.assignment.push($("#pa4").val());
    scores.assignment.push($("#pa5").val());
    scores.assignment.push($("#pa6").val());
    scores.exam = [];
    scores.exam.push($("#exam1").val());
    scores.exam.push($("#exam2").val());
    scores.participation = [];
    scores.participation.push($("#participation").val());
    scores.evals = [];
    scores.evals.push($("#evals").val());

    var a = assessments();
    var w = weights();
    var score = 0.0;
    var total = 0.0;

    // Assignments.
    var assignments = graded(scores.assignment);
    if (assignments.length > 0) {
        if (assignments.length == a.assignment) {
            // 1, 2, 3, 5, and best of 4 and 6.
            assignments = [assignments[0], assignments[1], assignments[2], assignments[4], Math.max(assignments[3], assignments[5])];
        }
        score += w.assignment / 100.0 * sum(assignments);
        total += w.assignment * assignments.length;
    }

    // Exams.
    var exams = graded(scores.exam);
    if (exams.length > 0) {
        if (exams.length == a.exam && exams[0] >= 87 && exams[1] >= 87) {
            // If each exam score is at least 87 (B+), the higher score is the exam average.
            exams[0] = exams[1] = Math.max(...exams);
        }
        score += w.exam / 100.0 * sum(exams);
        total += w.exam * exams.length;
    }

    // Participation.
    var participation = graded(scores.participation);
    if (participation.length == a.participation) {
        score += w.participation / 100.0 * participation[0]; 
        total += w.participation * participation.length;
    }
    
    // Course evaluation.
    var evals = graded(scores.evals);
    if (evals.length == a.evals) {
        score += w.evals / 100.0 * scores.evals[0];
    }

    score = total > 0.0 ? score / total * 100.0 : score;
    if (borderline(score)) {
        score = Math.ceil(score);
    }
    
    var grade = "";
    if (score >= 70) {
        grade = '<span><font color="green">' +
            score.toFixed(2) + ' (' + score2grade(score) + ')</font></span>';
    }
    else if (score >= 60) {
        grade = '<span><font color="orange">' +
            score.toFixed(2) + ' (' + score2grade(score) + ')</font></span>';
    }
    else {
        grade = '<span><font color="red">' +
            score.toFixed(2) + ' (' + score2grade(score) + ')</font></span>';
    }
    var disclaimer = "The above grade accurately reflects the grading scheme for the course only when all the scores have been entered."
    $(".grade").html(grade);
    $(".disclaimer").html(disclaimer);
}
    </script>
  </div>
