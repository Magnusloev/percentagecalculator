<!DOCTYPE html>
<html>
<head>
    <title>Percentage Calculator</title>
    <style>
        body { 
            font-family: Arial, sans-serif; 
            max-width: 800px; 
            margin: 0 auto; 
            padding: 20px;
            background: #f0f0f0;
        }
        .calculator { 
            background: white; 
            padding: 30px; 
            border-radius: 10px; 
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        h1 { color: #333; text-align: center; }
        input { padding: 10px; margin: 5px; border: 1px solid #ddd; }
        button { padding: 10px 20px; background: #007bff; color: white; border: none; cursor: pointer; }
        .result { font-weight: bold; color: green; margin: 10px 0; }
    </style>
</head>
<body>
    <h1>Percentage Calculator</h1>
    <div class="calculator">
        <p>What is <input type="number" id="percent1" placeholder="15"> % of <input type="number" id="number1" placeholder="100"> ?</p>
        <button onclick="calculate1()">Calculate</button>
        <div class="result" id="result1"></div>
    </div>
    
    <script>
        function calculate1() {
            const percent = parseFloat(document.getElementById('percent1').value);
            const number = parseFloat(document.getElementById('number1').value);
            if (!isNaN(percent) && !isNaN(number)) {
                const result = (percent / 100) * number;
                document.getElementById('result1').textContent = `= ${result}`;
            }
        }
    </script>
</body>
</html>
