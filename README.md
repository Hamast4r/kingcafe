<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>King Cafe</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
        }
        nav button {
            background-color: #444;
            color: white;
            border: none;
            padding: 15px 20px;
            cursor: pointer;
            font-size: 16px;
        }
        nav button:hover {
            background-color: #666;
        }
        .section {
            display: none;
            padding: 20px;
        }
        .active {
            display: block;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        ul li {
            margin: 10px 0;
            font-size: 18px;
        }
    </style>
</head>
<body>
    <header>
        <h1>King Cafe</h1>
    </header>
    <nav>
        <button onclick="showSection(0)">نێرگەلەکان</button>
        <button onclick="showSection(1)">Section 2</button>
        <button onclick="showSection(2)">Section 3</button>
        <button onclick="showSection(3)">Section 4</button>
        <button onclick="showSection(4)">Section 5</button>
        <button onclick="showSection(5)">Section 6</button>
        <button onclick="showSection(6)">Section 7</button>
    </nav>
    <div id="sections">
        <div class="section active">
            <h2>تامەکان</h2>
            <ul>
                <li>King 1</li>
                <li>King 2</li>
                <li>King 3</li>
                <li>King 4</li>
                <li>King 5</li>
                <li>King 6</li>
                <li>King 7</li>
                <li>King 8</li>
                <li>King 9</li>
                <li>King 10</li>
                <li>King 11</li>
                <li>Dw Sew</li>
                <li>بنیشت</li>
                <li>Baghdadi</li>
                <li>کاسترۆ</li>
                <li>لیمۆ</li>
            </ul>
        </div>
        <div class="section">
            <h2>Section 2</h2>
            <p>Content for section 2</p>
        </div>
        <div class="section">
            <h2>Section 3</h2>
            <p>Content for section 3</p>
        </div>
        <div class="section">
            <h2>Section 4</h2>
            <p>Content for section 4</p>
        </div>
        <div class="section">
            <h2>Section 5</h2>
            <p>Content for section 5</p>
        </div>
        <div class="section">
            <h2>Section 6</h2>
            <p>Content for section 6</p>
        </div>
        <div class="section">
            <h2>Section 7</h2>
            <p>Content for section 7</p>
        </div>
    </div>

    <script>
        function showSection(index) {
            const sections = document.querySelectorAll('.section');
            sections.forEach((section, i) => {
                section.classList.toggle('active', i === index);
            });
        }
    </script>
</body>
</html>
