function addRecommendation() {
  var nameInput = document.getElementById("name");
  var recommendationInput = document.getElementById("new_recommendation");

  var name = nameInput.value.trim();
  var recommendation = recommendationInput.value.trim();

  if (name !== "" && recommendation !== "") {
    // Create a new recommendation element
    var recommendationElement = document.createElement("div");
    recommendationElement.classList.add("recommendation");
    recommendationElement.innerHTML = `<span>&#8220;</span>${recommendation}<span>&#8221;</span> - ${name}`;

    // Add the new recommendation to the container
    var recommendationsContainer = document.getElementById(
      "all_recommendations"
    );
    recommendationsContainer.appendChild(recommendationElement);

    // Reset the input fields
    nameInput.value = "";
    recommendationInput.value = "";
    showPopup(true);
  }
}
function fadeIn(element) {
  var opacity = 0;
  var intervalId = setInterval(function () {
    if (opacity < 1) {
      opacity += 0.1;
      element.style.opacity = opacity;
    } else {
      clearInterval(intervalId);
    }
  }, 100);
}

// Function for a typewriter effect
function typeWriter(element, text, speed) {
  var i = 0;
  function type() {
    if (i < text.length) {
      element.innerHTML += text.charAt(i);
      i++;
      setTimeout(type, speed);
    }
  }
  type();
}

// Trigger animations when the page loads
window.addEventListener("load", function () {
  // Fade-in effect for the introduction section
  var introduction = document.querySelector(".introduction");
  fadeIn(introduction);

  // Typewriter effect for the about-me paragraph
  var aboutMeText = "Find Out more about me below...";
  var aboutMeParagraph = document.querySelector("#about-me p");
  typeWriter(aboutMeParagraph, aboutMeText, 50);
});
function scrollAnimations() {
  // Get elements that you want to animate
  var skillsSection = document.getElementById("skills");
  var projectsSection = document.getElementById("projects");
  var recommendationsSection = document.getElementById("recco");

  // Check if the elements are in the viewport
  function isInViewport(element) {
    var rect = element.getBoundingClientRect();
    return (
      rect.top >= 0 &&
      rect.left >= 0 &&
      rect.bottom <=
        (window.innerHeight || document.documentElement.clientHeight) &&
      rect.right <= (window.innerWidth || document.documentElement.clientWidth)
    );
  }

  // Trigger animations when elements come into the viewport
  window.addEventListener("scroll", function () {
    if (isInViewport(skillsSection)) {
      // Add your animation for the skills section here (e.g., scale, rotate)
      skillsSection.classList.add("animated-skills");
    }

    if (isInViewport(projectsSection)) {
      // Add your animation for the projects section here
      projectsSection.classList.add("animated-projects");
    }

    if (isInViewport(recommendationsSection)) {
      // Add your animation for the recommendations section here
      recommendationsSection.classList.add("animated-recommendations");
    }
  });
}

// Trigger the scrollAnimations function when the page loads
window.addEventListener("load", function () {
  scrollAnimations();
});

// Add hover effect for the skills
var skillCards = document.querySelectorAll(".skill");
skillCards.forEach(function (card) {
  card.addEventListener("mouseover", function () {
    card.classList.add("skill-hover");
  });
  card.addEventListener("mouseout", function () {
    card.classList.remove("skill-hover");
  });
});
