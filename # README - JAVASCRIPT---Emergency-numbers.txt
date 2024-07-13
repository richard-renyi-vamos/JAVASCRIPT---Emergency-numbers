CHATGPT CONVERSATION

----------

create a JAVASCRIPT code that shows the emergency numbers for a selected country
ChatGPT
Sure! Below is a simple JavaScript code snippet that displays emergency numbers for a selected country. This example uses a basic HTML structure with a dropdown menu to select the country and a div to display the emergency numbers.

html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emergency Numbers by Country</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        select, #emergency-numbers {
            font-size: 18px;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Emergency Numbers by Country</h1>
    <select id="country-select" onchange="showEmergencyNumbers()">
        <option value="">Select a country</option>
        <option value="USA">United States</option>
        <option value="UK">United Kingdom</option>
        <option value="Germany">Germany</option>
        <option value="France">France</option>
        <option value="Hungary">Hungary</option>
    </select>
    <div id="emergency-numbers"></div>

    <script>
        const emergencyNumbers = {
            "USA": "911",
            "UK": "999",
            "Germany": "112",
            "France": "112",
            "Hungary": "112"
        };

        function showEmergencyNumbers() {
            const countrySelect = document.getElementById('country-select');
            const selectedCountry = countrySelect.value;
            const emergencyNumbersDiv = document.getElementById('emergency-numbers');

            if (selectedCountry) {
                emergencyNumbersDiv.innerHTML = `<h2>Emergency Number for ${selectedCountry}</h2><p>${emergencyNumbers[selectedCountry]}</p>`;
            } else {
                emergencyNumbersDiv.innerHTML = '';
            }
        }
    </script>
</body>
</html>
This code consists of:

An HTML select element to choose a country.
A div to display the emergency numbers.
A JavaScript function showEmergencyNumbers that updates the div based on the selected country.
When a user selects a country from the dropdown menu, the corresponding emergency number is displayed. Feel free to expand the emergencyNumbers object with more countries and their emergency numbers as needed. 🚒🚓🚑🌍👩‍⚕️👮‍♂️👨‍🚒🆘📞💻






