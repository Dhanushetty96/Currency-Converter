# 💱 Currency Converter
A responsive and user-friendly currency converter web application built using HTML, CSS, and JavaScript. This project allows users to convert an amount from one currency to another using real-time exchange rates fetched from the free Latest Currency API.

It also dynamically displays the country flags for selected currencies, making the interface more intuitive and engaging.


🚀 Features
🔁 Real-time currency conversion

🌍 Dynamic dropdown menus for currency selection

🏳️ Auto-updating country flags based on selected currencies

💵 Input validation to handle empty or invalid amounts

🧠 Default settings: USD → INR conversion

⚡ Fast and lightweight — built with vanilla JavaScript

📱 Mobile-responsive design

📸 Screenshots
(Insert screenshots here if available)

🛠️ Tech Stack
HTML5 — Semantic layout structure

CSS3 — Styling and responsive design

JavaScript (ES6+) — Core logic and API interaction

Latest Currency API — Exchange rate data source

Flags API — Country flag images

📂 File Structure
graphql
Copy
Edit
Currency-Converter/
│
├── index.html        # Main HTML structure
├── style.css         # CSS styling
├── script.js         # JavaScript logic and API calls
└── codes.js          #country's currency and code
📚 How It Works
On load, dropdowns are populated with currency codes.

USD is selected as the default "From" currency, and INR as "To".

Selecting a currency automatically updates the corresponding flag using the Flags API.

Entering an amount and clicking "Convert" fetches the latest exchange rate and displays the converted value.

Handles empty or invalid input by defaulting to "1".

🔄 Example API Usage
js
Copy
Edit
const BASE_URL = "https://latest.currency-api.pages.dev/v1/currencies";
const response = await fetch(`${BASE_URL}/usd.json`);
const data = await response.json();
const rate = data["usd"]["inr"];
✅ To Do / Improvements
 Add dark mode toggle

 Show historical exchange rates

 Add loading spinner during API fetch

 Support currency name display (e.g., USD → United States Dollar)

🙌 Acknowledgements
💹 Latest Currency API for free exchange rates

🏳️ FlagsAPI.com for country flags

👩‍💻 Author
Dhanu Shetty
A passionate web developer focused on building practical and user-friendly web applications.
Feel free to connect with me on LinkedIn (add your profile link) or check out more of my projects!

📃 License
This project is open-source and available under the MIT License.

