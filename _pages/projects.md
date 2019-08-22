---
permalink: /projects/
title: "Projects"
---
<h2 id="projects">Projects</h2>
<div>
  <a href="#" onclick="filterProjects(event, 'all')" class="btn btn--primary">All</a>
  <a href="#" onclick="filterProjects(event, 'hifi')" class="btn btn--primary">High Fidelity</a>
  <a href="#" onclick="filterProjects(event, 'lab')" class="btn btn--primary">Lab</a>
  <a href="#" onclick="filterProjects(event, 'personal')" class="btn btn--primary">Personal</a>
  <a href="#" onclick="filterProjects(event, 'odu')" class="btn btn--primary">Grad School</a>
</div>

[Mythbusters](https://youtu.be/2KmXllrBNHw?t=80)
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/2KmXllrBNHw?start=80" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

[Last Avatar Standing Trivia](https://youtu.be/ACxZT6zaieQ)

[Last Avatar Standing Trivia](https://github.com/MarkBrosche/hifi-content/tree/master/events/lastAvatarStandingTrivia)

[Money tree](https://github.com/MarkBrosche/hifi-content/tree/master/placeSpecificContent/theSpot/moneyTree)

[Google Calendar](https://github.com/MarkBrosche/hifi-content/tree/master/usefulUtilities/hiFiCalendar)

[Vizard MR Training Proof of Concept](https://drive.google.com/open?id=0B1LmsSL44FGCbkNEREpQR0I5elU)

[VR/AR Trombone App](https://drive.google.com/open?id=1G-VsoYhNXNamcCYy2tWiOncjCo5i22Hz)

[Dynamic Depth of Field HMD](https://drive.google.com/open?id=1C4EfZhXr0-ocq4Z7vP7fQWkmf4nkuEBd)

[OpenGL 3.0 Quaternion Orbit Project](https://drive.google.com/open?id=1ivDRDrZ-T3X9veExEKZM0RVKpzjLBfdE)

[OpenGL 3.0 Shooting Gallery](https://drive.google.com/file/d/1VLpVX2h9FrAKQwVVd02E1tp8MRURmpm_/view)


<script>

const projectsElement = document.getElementsByClassName("feature__wrapper")[0];
const hiddenElement = document.getElementById("hidden");

function filterProjects(e, str) {
  e.preventDefault();

  if (str === "all") {
    while (hiddenElement.firstChild) {
      projectsElement.appendChild(hiddenElement.firstChild); // might be out of order
    }
    return;
  }

  var visibleProjects = projectsElement.getElementsByClassName("filter-item");
  var hiddenProjects = hiddenElement.getElementsByClassName("filter-item");

  var addToHidden = [...visibleProjects].filter(elem => elem.className.indexOf(str) === -1);
  var addToVisible = [...hiddenProjects].filter(elem => elem.className.indexOf(str) !== -1);

  while (addToHidden.length) {
    hiddenElement.appendChild(addToHidden[0]);
    addToHidden.shift();
  }
  while (addToVisible.length) {
    projectsElement.appendChild(addToVisible[0]);
    addToVisible.shift();
  }

}

</script>
