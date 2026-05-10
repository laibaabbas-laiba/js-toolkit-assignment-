# js-toolkit-assignment-
index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>JS Toolkit Assignment</title>
    <link href="[https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css](https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css)" rel="stylesheet">
</head>
<body class="bg-gray-100 flex flex-col items-center justify-center min-h-screen">
    <h1 class="text-3xl font-bold text-blue-600 mb-4">Modern JS Toolkit</h1>
    <div id="output" class="p-6 bg-white rounded shadow-lg text-lg text-gray-800">
        Check the console and screen for output!
    </div>
    <script src="script.js"></script>
</body>
</html>


script.js

// Function 1: Modern Arrow Function for Greeting
const showGreeting = () => {
    const msg = "Welcome to the JS Toolkit Assignment!";
    document.getElementById('output').innerHTML = `<p class='font-bold'>${msg}</p>`;
};

// Function 2: Array Mapping (Modern JS Concept)
const displayTools = () => {
    const tools = ['Git', 'GitHub', 'JavaScript', 'Tailwind CSS'];
    const list = tools.map(tool => `<li class='text-blue-500'>${tool}</li>`).join('');
    document.getElementById('output').innerHTML += `<ul class="mt-4 list-disc pl-5">${list}</ul>`;
};

showGreeting();
displayTools();
