---
permalink: "/cs210/grade.html"
layout: cs210_page
title: What's My Grade?
exclude: true
---

<div class="aside">
    <div class="container-fluid">
      <span><b>Exercises</b></span>
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
            <input id="exer1" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="exer2" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="exer3" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="exer4" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="exer5" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="exer6" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
        </tr>
      </table>
      <p/>
      <span><b>Projects</b></span>
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
            <input id="proj1" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="proj2" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="proj3" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="proj4" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="proj5" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
          </td>
          <td class="col-1">
            <input id="proj6" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/>
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
    <span><b>Attendance</b></span>
    <table>
      <tr>
        <td><input id="attendance" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/></td>
    </tr>
    </table>
    <p/>
    <p/>
    <span><b>Supplemental Instruction (SI)</b></span>
    <table>
      <tr>
        <td><input id="si" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/></td>
      </tr>
    </table>
    <p/>
    <p/>
    <span><b>Course Evaluation</b></span>
    <table>
      <tr>
        <td><input id="eval" type="number" min="0" max="100" size="10" class="form-control" placeholder="%"/></td>
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
    assessments.exercise = 6;
    assessments.project = 6;
    assessments.exam = 2;
    assessments.attendance = 1;
    assessments.si = 1;
    assessments.evals = 1;
    return assessments;
}

// Return an object containing weights for calculating student grade.
function weights() {
    var weights = new Object();
    weights.exercise = 1;
    weights.project = 4;
    weights.exam = 35;
    weights.attendance = 5;
    weights.si = 3;
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
    scores.exercise = [];
    scores.exercise.push($("#exer1").val());
    scores.exercise.push($("#exer2").val());
    scores.exercise.push($("#exer3").val());
    scores.exercise.push($("#exer4").val());
    scores.exercise.push($("#exer5").val());
    scores.exercise.push($("#exer6").val());
    scores.project = [];
    scores.project.push($("#proj1").val());
    scores.project.push($("#proj2").val());
    scores.project.push($("#proj3").val());
    scores.project.push($("#proj4").val());
    scores.project.push($("#proj5").val());
    scores.project.push($("#proj6").val());
    scores.exam = [];
    scores.exam.push($("#exam1").val());
    scores.exam.push($("#exam2").val());
    scores.attendance = [];
    scores.attendance.push($("#attendance").val());
    scores.si = [];
    scores.si.push($("#si").val());
    scores.evals = [];
    scores.evals.push($("#eval").val());
    
    var a = assessments();
    var w = weights();
    var score = 0.0;
    var total = 0.0;

    // Exercises
    var exercises = graded(scores.exercise);
    if (exercises.length == a.exercise) {
        // Drop the lowest exercise score.
        exercises.sort(function(x, y) {return x - y});
        exercises.reverse();
        exercises = exercises.slice(0, -1);
    }
    if (exercises.length > 0) {
        score += w.exercise / 100.0 * sum(exercises);
        total += w.exercise * exercises.length;
    }

    // Projects
    var projects = graded(scores.project);
    if (projects.length == a.project) {
        // Drop the lowest project score.
        projects.sort(function(x, y) {return x - y});
        projects.reverse();
        projects = projects.slice(0, -1);
    }
    if (projects.length > 0) {
        score += w.project / 100.0 * sum(projects);
        total += w.project * projects.length;
    }
    
    // Exams
    var exams = graded(scores.exam);
    if (exams.length == a.exam) {
        // If both exam scores >= 80%, max exam score is the exam average.
        if (exams[0] >= 80 && exams[1] >= 80) {
            exams[0] = exams[1] = Math.max(exams[0], exams[1]);
        }
    }
    if (exams.length > 0) {
        score += w.exam / 100.0 * sum(exams);
        total += w.exam * exams.length;
    }

    // Attendance.
    var attendance = graded(scores.attendance);
    if (attendance.length == a.attendance) {
        score += w.attendance / 100.0 * attendance[0]; 
        total += w.attendance * attendance.length;
    }
        
    // Supplemental instruction
    si = graded(scores.si);
    if (si.length == a.si) {
        score += w.si / 100.0 * scores.si[0];
    }
    
    // Course evaluation
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
