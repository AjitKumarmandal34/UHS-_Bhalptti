<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>मेरे स्कूल की वेबसाइट</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
            color: #333;
        }

        header {
            background-color: #007bff;
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav {
            background: #0056b3;
            color: white;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-size: 16px;
        }

        nav a:hover {
            text-decoration: underline;
        }

        section {
            padding: 20px;
            margin: 10px auto;
            max-width: 800px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        h2 {
            color: #007bff;
            text-align: center;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
        }

        table, th, td {
            border: 1px solid #ddd;
        }

        th, td {
            padding: 10px;
            text-align: center;
        }

        th {
            background: #f0f0f0;
        }

        footer {
            text-align: center;
            padding: 15px;
            background-color: #333;
            color: white;
            margin-top: 20px;
        }

        /* Login and Registration Section */
        #login-section, #register-section {
            display: block;
            text-align: center;
            padding: 50px;
            background-color: #f9f9f9;
        }

        #main-content {
            display: none;
        }

        input {
            padding: 10px;
            margin: 10px;
            width: 200px;
            border-radius: 5px;
        }

        button {
            padding: 10px 15px;
            background-color: #007bff;
            color: white;
            border: none;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

<!-- Register Section -->
<div id="register-section">
    <h2>रजिस्टर करें</h2>
    <input type="text" id="username" placeholder="यूजरनेम दर्ज करें" />
    <input type="password" id="new-password" placeholder="नया पासवर्ड बनाएं" />
    <button onclick="register()">रजिस्टर करें</button>
    <p>अगर आपका अकाउंट पहले से है, तो <a href="#" onclick="showLogin()">यहां लॉगिन करें</a>.</p>
</div>

<!-- Login Section -->
<div id="login-section" style="display: none;">
    <h2>लॉगिन करें</h2>
    <input type="text" id="login-username" placeholder="यूजरनेम" />
    <input type="password" id="login-password" placeholder="पासवर्ड" />
    <button onclick="login()">लॉगिन करें</button>
    <p>अगर आपने रजिस्टर नहीं किया है, तो <a href="#" onclick="showRegister()">रजिस्टर करें</a>.</p>
</div>

<!-- Main Content -->
<div id="main-content">
    <header>
        <h1>मेरे स्कूल की वेबसाइट</h1>
        <p>यहां आपको हमारे स्कूल के बारे में पूरी जानकारी मिलेगी।</p>
    </header>

    <nav>
        <a href="#about-school">स्कूल के बारे में</a>
        <a href="#time-table">टाइम टेबल</a>
        <a href="#library">लाइब्रेरी</a>
        <a href="#teachers">टीचर्स की जानकारी</a>
    </nav>

    <section id="about-school">
        <h2>स्कूल के बारे में</h2>
        <p>हमारे स्कूल का निर्माण वर्ष 1995 में हुआ। यह विद्यालय शिक्षा के क्षेत्र में बेहतरीन सेवाएं प्रदान करता है। हमारा उद्देश्य छात्रों को एक उज्ज्वल भविष्य प्रदान करना है।</p>
    </section>

    <section id="time-table">
        <h2>स्कूल टाइम टेबल</h2>
        <table>
            <thead>
                <tr>
                    <th>पीरियड</th>
                    <th>समय</th>
                    <th>विषय</th>
                    <th>अध्यापक</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>1</td>
                    <td>12:00 - 12:40</td>
                    <td>जियोग्राफी</td>
                    <td>संतोष सर</td>
                </tr>
                <tr>
                    <td>2</td>
                    <td>12:40 - 1:20</td>
                    <td>होम साइंस / साइकोलॉजी</td>
                    <td>सोनू सर</td>
                </tr>
                <tr>
                    <td>3</td>
                    <td>1:20 - 2:00</td>
                    <td>इतिहास</td>
                    <td>रंजीत सर</td>
                </tr>
                <tr>
                    <td>4</td>
                    <td>2:00 - 2:40</td>
                    <td>राजनीति विज्ञान</td>
                    <td>प्रिया मैम</td>
                </tr>
                <tr>
                    <td>लंच</td>
                    <td>3:00 - 3:30</td>
                    <td colspan="2">आराम</td>
                </tr>
                <tr>
                    <td>5</td>
                    <td>3:30 - 4:10</td>
                    <td>अंग्रेजी</td>
                    <td>राखी मैम</td>
                </tr>
                <tr>
                    <td>6</td>
                    <td>4:10 - 5:00</td>
                    <td>हिंदी</td>
                    <td>आशा मैम</td>
                </tr>
            </tbody>
        </table>
    </section>

    <section id="library">
        <h2>स्कूल लाइब्रेरी</h2>
        <p>हमारी लाइब्रेरी में 5000 से अधिक किताबें हैं। यहां छात्रों के लिए विभिन्न विषयों पर पुस्तकें उपलब्ध हैं। लाइब्रेरी का समय सुबह 9:00 बजे से शाम 5:00 बजे तक है।</p>
    </section>

    <section id="teachers">
        <h2>टीचर्स की जानकारी</h2>
        <ul>
            <li><strong>प्रिया मैम:</strong> राजनीति विज्ञान पढ़ाती हैं।</li>
            <li><strong>सोनू सर:</strong> होम साइंस और साइकोलॉजी पढ़ाते हैं।</li>
            <li><strong>रंजीत सर:</strong> इतिहास पढ़ाते हैं।</li>
            <li><strong>संतोष सर:</strong> जियोग्राफी पढ़ाते हैं।</li>
            <li><strong>राखी मैम:</strong> अंग्रेजी पढ़ाती हैं।</li>
            <li><strong>आशा मैम:</strong> हिंदी पढ़ाती हैं।</li>
        </ul>
    </section>

    <footer>
        <p>© 2025 मेरे स्कूल का वेबसाइट | सभी अधिकार सुरक्षित</p>
    </footer>
</div>

<script>
    // Registration and Login functionality
    let users = [];

    function register() {
        var username = document.getElementById('username').value;
        var password = document.getElementById('new-password').value;

        if (username && password) {
            users.push({ username: username, password: password });
            alert("रजिस्टर सफलतापूर्वक हो गया!");
            showLogin();
        } else {
            alert("कृपया सभी फ़ील्ड भरें।");
        }
    }

    function login() {
        var username = document.getElementById('login-username').value;
        var password = document.getElementById('login-password').value;

        var user = users.find(u => u.username === username && u.password === password);

        if (user) {
            document.getElementById('login-section').style.display = 'none';
            document.getElementById('main-content').style.display = 'block';
        } else {
            alert("गलत यूजरनेम या पासवर्ड!");
        }
    }

    function showRegister() {
        document.getElementById('login-section').style.display = 'none';
        document.getElementById('register-section').style.display = 'block';
    }

    function showLogin() {
        document.getElementById('register-section').style.display = 'none';
        document.getElementById('login-section').style.display = 'block';
    }
</script>

</body>
</html>
