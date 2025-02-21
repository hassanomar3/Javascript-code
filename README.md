// script.js

document.getElementById("contactForm").addEventListener("submit", function(event) {
    event.preventDefault(); // Prevents the form from submitting the traditional way

    // Simple feedback message
    const name = document.getElementById("name").value;
    document.getElementById("responseMessage").innerText = Thank you, ${name}! We will get back to you soon.;

    // Clear form fields after submission
    document.getElementById("contactForm").reset();
});
