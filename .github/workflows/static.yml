<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Math Calculator 🎀</title>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0px 5px 20px rgba(0, 0, 0, 0.2);
            width: 90%;
            max-width: 400px;
            text-align: center;
        }
        h2 {
            color: #d63384;
        }
        select, input {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 2px solid #f8a5c2;
            border-radius: 8px;
            font-size: 16px;
        }
        button {
            width: 100%;
            padding: 12px;
            background: #ff6b81;
            border: none;
            color: white;
            font-size: 18px;
            font-weight: bold;
            border-radius: 8px;
            cursor: pointer;
        }
        button:hover {
            background: #d63384;
        }
        .result {
            margin-top: 20px;
            font-size: 18px;
            font-weight: bold;
            color: #444;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>🎀 Math Calculator 🎀</h2>
        <label for="chapter">Select Chapter:</label>
        <select id="chapter" onchange="showOptions()">
            <option value="">-- Choose Chapter --</option>
            <option value="11">Perimeter & Area</option>
            <option value="13">Multiplication</option>
            <option value="14">Volume</option>
            <option value="15">Equations</option>
        </select>
        <div id="options" style="display: none;"></div>
        <button onclick="calculate()">Calculate</button>
        <div id="output" class="result"></div>
    </div>
    <script>
        function showOptions() {
            let chapter = document.getElementById("chapter").value;
            let options = document.getElementById("options");
            options.style.display = "block";
            options.innerHTML = "";
            
            if (chapter === "11") {
                options.innerHTML = `<label>Choose Shape:</label>
                                    <select id='shape'>
                                        <option value='rectangle'>Rectangle</option>
                                        <option value='square'>Square</option>
                                    </select>`;
            } else if (chapter === "13") {
                options.innerHTML = `<input type='number' id='num1' placeholder='Enter First Number'>
                                     <input type='number' id='num2' placeholder='Enter Second Number'>`;
            } else if (chapter === "14") {
                options.innerHTML = `<label>Choose Solid:</label>
                                    <select id='solid'>
                                        <option value='rectangular_prism'>Rectangular Prism</option>
                                        <option value='cube'>Cube</option>
                                    </select>`;
            } else if (chapter === "15") {
                options.innerHTML = `<input type='text' id='equation' placeholder='Enter equation (e.g., x+5)'>
                                     <input type='number' id='x_value' placeholder='Enter value of x'>`;
            }
        }
        
        function calculate() {
            let chapter = document.getElementById("chapter").value;
            let output = document.getElementById("output");
            output.innerHTML = "";
            
            if (chapter === "11") {
                let shape = document.getElementById("shape").value;
                if (shape === "rectangle") {
                    let l = prompt("Enter Length:");
                    let b = prompt("Enter Breadth:");
                    output.innerHTML = `📏 Perimeter: <b>${2 * (parseInt(l) + parseInt(b))}</b><br>
                                        📐 Area: <b>${l * b}</b>`;
                } else {
                    let a = prompt("Enter Side Length:");
                    output.innerHTML = `🟦 Perimeter: <b>${4 * a}</b><br>
                                        🔲 Area: <b>${a * a}</b>`;
                }
            } else if (chapter === "13") {
                let num1 = document.getElementById("num1").value;
                let num2 = document.getElementById("num2").value;
                output.innerHTML = 🔢 Product: <b>${num1 * num2}</b>;
            } else if (chapter === "14") {
                let solid = document.getElementById("solid").value;
                if (solid === "rectangular_prism") {
                    let l = prompt("Enter Length:");
                    let b = prompt("Enter Breadth:");
                    let h = prompt("Enter Height:");
                    output.innerHTML = 📦 Volume: <b>${l * b * h}</b>;
                } else {
                    let s = prompt("Enter Side Length:");
                    output.innerHTML = 🎲 Volume: <b>${s ** 3}</b>;
                }
            } else if (chapter === "15") {
    let equation = document.getElementById("equation").value;
    let x = document.getElementById("x_value").value;

    try {
        // Ensure multiplication is explicitly stated
        let formattedEquation = equation.replace(/(\d)(x)/g, "$1*$2").replace(/x/g, (${x}));
        let y = eval(formattedEquation);
        output.innerHTML = 📊 Result: <b>y = ${y}</b>;
    } catch (e) {
        output.innerHTML = ⚠ Invalid Equation;
    }
} else {
    output.innerHTML = ⚡ Chapter <b>${chapter}</b> is coming soon...;
}
        }
    </script>
</body>
</html>
