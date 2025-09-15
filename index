<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Percentage Calculator - Simple & Fast</title>
    <meta name="description" content="Free online percentage calculator. Calculate percentages instantly with our simple, clean interface.">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px 0;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            text-align: center;
            margin-bottom: 40px;
            color: white;
        }
        
        h1 {
            font-size: 3rem;
            font-weight: 300;
            margin-bottom: 10px;
            text-shadow: 0 2px 4px rgba(0,0,0,0.3);
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            font-weight: 300;
        }
        
        /* Main Calculator Card */
        .calculator-card {
            background: white;
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.1);
            margin-bottom: 40px;
            position: relative;
            overflow: hidden;
        }
        
        .calculator-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #667eea, #764ba2);
        }
        
        .calc-grid {
            display: grid;
            gap: 30px;
        }
        
        .calc-item {
            background: #f8f9fc;
            padding: 25px;
            border-radius: 12px;
            border: 1px solid #e3e8f0;
            transition: all 0.3s ease;
        }
        
        .calc-item:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }
        
        .calc-question {
            font-size: 1.1rem;
            color: #2d3748;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 8px;
        }
        
        input {
            background: white;
            border: 2px solid #e2e8f0;
            border-radius: 8px;
            padding: 8px 12px;
            font-size: 16px;
            width: 80px;
            text-align: center;
            transition: border-color 0.3s ease;
        }
        
        input:focus {
            outline: none;
            border-color: #667eea;
            box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
        }
        
        .calc-button {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 14px;
            font-weight: 500;
            transition: all 0.3s ease;
            margin-top: 10px;
        }
        
        .calc-button:hover {
            transform: translateY(-1px);
            box-shadow: 0 4px 12px rgba(102, 126, 234, 0.4);
        }
        
        .result {
            margin-top: 10px;
            padding: 10px 15px;
            background: #f0fff4;
            border: 1px solid #9ae6b4;
            border-radius: 8px;
            color: #22543d;
            font-weight: 600;
            font-size: 1.1rem;
            display: none;
        }
        
        .result.show {
            display: block;
        }
        
        /* Content Sections */
        .content-section {
            background: white;
            border-radius: 16px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.05);
        }
        
        .content-section h2 {
            color: #2d3748;
            margin-bottom: 20px;
            font-size: 1.5rem;
            font-weight: 600;
        }
        
        .content-section p {
            color: #4a5568;
            margin-bottom: 15px;
        }
        
        .tips-box {
            background: linear-gradient(135deg, #e3f2fd, #f3e5f5);
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 30px;
            border-left: 4px solid #667eea;
        }
        
        .tips-title {
            font-weight: 600;
            color: #2d3748;
            margin-bottom: 10px;
        }
        
        .tip-item {
            color: #4a5568;
            margin-bottom: 5px;
        }
        
        /* Ad Spaces */
        .ad-space {
            background: #f7fafc;
            border: 2px dashed #cbd5e0;
            border-radius: 12px;
            padding: 40px 20px;
            text-align: center;
            color: #718096;
            margin: 30px 0;
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.2rem;
            }
            
            .calculator-card {
                padding: 25px;
            }
            
            .calc-question {
                flex-direction: column;
                align-items: flex-start;
                gap: 10px;
            }
            
            input {
                width: 100%;
                max-width: 200px;
            }
        }
        
        /* Simple animations */
        .calculator-card {
            animation: slideUp 0.6s ease-out;
        }
        
        @keyframes slideUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Percentage Calculator</h1>
            <p class="subtitle">Simple, fast, and accurate percentage calculations</p>
        </header>
        
        <div class="tips-box">
            <div class="tips-title">Quick Tips:</div>
            <div class="tip-item">• Use Tab to move between fields</div>
            <div class="tip-item">• Press Enter to calculate</div>
            <div class="tip-item">• All calculations are instant</div>
        </div>
        
        <div class="calculator-card">
            <div class="calc-grid">
                <!-- Calculator 1: What is X% of Y? -->
                <div class="calc-item">
                    <div class="calc-question">
                        What is <input type="number" id="percent1" placeholder="15"> % of <input type="number" id="number1" placeholder="200"> ?
                    </div>
                    <button class="calc-button" onclick="calculate1()">Calculate</button>
                    <div class="result" id="result1"></div>
                </div>
                
                <!-- Calculator 2: X is what percent of Y? -->
                <div class="calc-item">
                    <div class="calc-question">
                        <input type="number" id="number2" placeholder="30"> is what percent of <input type="number" id="total2" placeholder="200"> ?
                    </div>
                    <button class="calc-button" onclick="calculate2()">Calculate</button>
                    <div class="result" id="result2"></div>
                </div>
                
                <!-- Calculator 3: Percentage Change -->
                <div class="calc-item">
                    <div class="calc-question">
                        Percentage change from <input type="number" id="old" placeholder="100"> to <input type="number" id="new" placeholder="125">
                    </div>
                    <button class="calc-button" onclick="calculateChange()">Calculate</button>
                    <div class="result" id="resultChange"></div>
                </div>
                
                <!-- Calculator 4: X is Y% of what? -->
                <div class="calc-item">
                    <div class="calc-question">
                        <input type="number" id="number3" placeholder="50"> is <input type="number" id="percent3" placeholder="25"> % of what?
                    </div>
                    <button class="calc-button" onclick="calculate3()">Calculate</button>
                    <div class="result" id="result3"></div>
                </div>
            </div>
        </div>
        
        <!-- Ad Space -->
        <div class="ad-space">
            <div>Advertisement</div>
            <small>728x90 or responsive ad unit</small>
        </div>
        
        <div class="content-section">
            <h2>How to Use This Calculator</h2>
            <p><strong>What is X% of Y?</strong> - Find a percentage of a number (e.g., 15% of 200 = 30)</p>
            <p><strong>X is what percent of Y?</strong> - Find what percentage one number is of another (e.g., 30 is 15% of 200)</p>
            <p><strong>Percentage change</strong> - Calculate the percentage increase or decrease between two numbers</p>
            <p><strong>X is Y% of what?</strong> - Find the total when you know the part and percentage (e.g., 50 is 25% of 200)</p>
        </div>
        
        <div class="content-section">
            <h2>Common Uses</h2>
            <p><strong>Shopping:</strong> Calculate discounts, sales tax, and tips</p>
            <p><strong>Finance:</strong> Interest rates, investment returns, and budget planning</p>
            <p><strong>Business:</strong> Growth rates, profit margins, and performance metrics</p>
            <p><strong>Education:</strong> Grade calculations and statistical analysis</p>
        </div>
        
        <!-- Ad Space -->
        <div class="ad-space">
            <div>Advertisement</div>
            <small>300x250 ad unit</small>
        </div>
    </div>
    
    <script>
        // Enhanced enter key functionality
        document.addEventListener('keypress', function(e) {
            if (e.key === 'Enter') {
                const activeElement = document.activeElement;
                const parent = activeElement.closest('.calc-item');
                if (parent) {
                    const button = parent.querySelector('.calc-button');
                    if (button) button.click();
                }
            }
        });
        
        function showResult(elementId, text) {
            const resultElement = document.getElementById(elementId);
            resultElement.textContent = text;
            resultElement.classList.add('show');
        }
        
        function calculate1() {
            const percent = parseFloat(document.getElementById('percent1').value);
            const number = parseFloat(document.getElementById('number1').value);
            if (!isNaN(percent) && !isNaN(number)) {
                const result = (percent / 100) * number;
                showResult('result1', `${result.toLocaleString()}`);
            }
        }
        
        function calculate2() {
            const number = parseFloat(document.getElementById('number2').value);
            const total = parseFloat(document.getElementById('total2').value);
            if (!isNaN(number) && !isNaN(total) && total !== 0) {
                const result = (number / total) * 100;
                showResult('result2', `${result.toFixed(2)}%`);
            }
        }
        
        function calculate3() {
            const number = parseFloat(document.getElementById('number3').value);
            const percent = parseFloat(document.getElementById('percent3').value);
            if (!isNaN(number) && !isNaN(percent) && percent !== 0) {
                const result = (number * 100) / percent;
                showResult('result3', `${result.toLocaleString()}`);
            }
        }
        
        function calculateChange() {
            const oldValue = parseFloat(document.getElementById('old').value);
            const newValue = parseFloat(document.getElementById('new').value);
            if (!isNaN(oldValue) && !isNaN(newValue) && oldValue !== 0) {
                const change = ((newValue - oldValue) / oldValue) * 100;
                const direction = change >= 0 ? 'increase' : 'decrease';
                const color = change >= 0 ? '#22543d' : '#c53030';
                const resultElement = document.getElementById('resultChange');
                resultElement.style.color = color;
                showResult('resultChange', `${Math.abs(change).toFixed(2)}% ${direction}`);
            }
        }
        
        // Auto-clear results when inputs change
        document.querySelectorAll('input').forEach(input => {
            input.addEventListener('input', function() {
                const parent = this.closest('.calc-item');
                const result = parent.querySelector('.result');
                result.classList.remove('show');
            });
        });
    </script>
</body>
</html>
