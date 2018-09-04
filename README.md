# calculator63  css/style.css
@@ -1,72 +1,83 @@
 body {
    background-image: url("../img/09pXgsGypas.jpg");    
    background-image: url("../img/09pXgsGypas.jpg");
}
.container{
 .container {
    display: flex;
    margin-top: 80px;
}
.calc-wrapper{
 .calc-wrapper {
    background-color: #f1efef;
    width: 340px;
    height: 410px;
    border-radius: 10px;
    box-shadow: 1px 35px 91px -23px #050505;
    padding-left: 20px;
}
#display{
background-color: #050505;
   padding: 0px 10px;
 #display {
    background-color: #050505;
    padding: 0px 10px;
    width: 300px;
    font-size: 39px;
   border-radius: 8px;
    margin:38px 0px;
    color: aliceblue;  
    font-family: 'Press Start 2P', cursive;   
    border-radius: 8px;
    margin: 38px 0px;
    color: aliceblue;
    font-family: 'Press Start 2P', cursive;
    text-align: right;
}
 ::-webkit-input-placeholder {
    color: rgba(193, 193, 193, 0.29);
}
.title{
 .title {
    color: white;
    font-size: 50px;
    margin: 80px 100px;
}
.about{
background-color: white;
 .about {
    background-color: white;
    width: 220px;
    padding: 8px 20px;
    font-size: 20px;
    border-radius: 23px;
    margin-left: 100px;
    margin-top: -50px;
}
.btn{
 .btn {
    width: 68px;
    height: 42px;
    background-color: #f4f4f4;
    border: 2px solid #e3e3e3;
    border-radius:6px; 
    border-radius: 6px;
    font-size: 20px;
    text-transform: uppercase;
    padding: 0px;
    color: #5b5c5d;
    cursor: pointer;
    margin: 3px;      
    margin: 3px;
}
.btn:hover{
    background-color:#b5b5b5;
 .btn:hover {
    background-color: #b5b5b5;
}
.btn_hover_red:hover{
 .btn_hover_red:hover {
    background-color: rgba(235, 53, 53, 0.92);
}
.btn_hover_blue:hover{
    background-color:#2957e0;
 .btn_hover_blue:hover {
    background-color: #2957e0;
}
#n0{
 #n0 {
    width: 145px;
}
#equal{
 #equal {
    height: 92px;
} 
}
  
46  index.html
@@ -10,6 +10,7 @@
    <link href="/css/style.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=VT323" rel="stylesheet">
    <script src="js/script.js"></script> 
    
</head>
<body>
    <div class="wrapper">
@@ -21,72 +22,72 @@
                            <div class="calc-wrapper">
                                <div class="calc">
                                    <div class="page_display">
                                        <input type="text" id="display" name="" class="calc_display-input" placeholder="00000000000000">
                                        <input disabled type="text" value="0" id="display" class="calc_display-input" placeholder="00000000000000">
                                    </div>
                                    <div class="calc_buttons">
                                        <table class="calc_table">
                                            <tr class="calc_buttons-row">
                                                <td>
                                                    <button type="button" class="btn btn_default btn_hover_red">ce</button>
                                                    <button type="button" id="ce" class="clearBtn btn btn_default btn_hover_red">ce</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default btn_hover_red">c</button>
                                                    <button type="button" id="c" class="clearBtn btn btn_default btn_hover_red">c</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default btn_hover_blue">/</button>
                                                    <button type="button" value="Деление" class="operation btn btn_default btn_hover_blue">/</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default btn_hover_blue">*</button>
                                                    <button type="button" value="Умножение" class="operation btn btn_default btn_hover_blue">*</button>
                                                </td>
                                            </tr>
                                            <tr class="calc_buttons-row">
                                                <td>
                                                    <button type="button" class="btn btn_default ">7</button>
                                                    <button type="button" class="number btn btn_default ">7</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default ">8</button>
                                                    <button type="button" class="number btn btn_default ">8</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default ">9</button>
                                                    <button type="button" class="number btn btn_default ">9</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default btn_hover_blue">-</button>
                                                    <button type="button" value="Вычитание" class="operation btn btn_default btn_hover_blue">-</button>
                                                </td>
                                            </tr>
                                            <tr class="calc_buttons-row">
                                                <td>
                                                    <button type="button" class="btn btn_default ">4</button>
                                                    <button type="button" class="number btn btn_default ">4</button>
                                                </td>
                                                <td>
                                                    <button type="button"class="btn btn_default ">5</button>
                                                    <button type="button"class="number btn btn_default ">5</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default ">6</button>
                                                    <button type="button" class="number btn btn_default ">6</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default btn_hover_blue">+</button>
                                                    <button type="button" value="Сложение" class="operation btn btn_default btn_hover_blue">+</button>
                                                </td>
                                            </tr>
                                            <tr class="calc_buttons-row">
                                                <td>
                                                    <button type="button" class="btn btn_default ">1</button>
                                                    <button type="button" class="number btn btn_default ">1</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default ">2</button>
                                                    <button type="button" class="number btn btn_default ">2</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default ">3</button>
                                                    <button type="button" class="number btn btn_default ">3</button>
                                                </td>
                                                <td rowspan="2">
                                                    <button type="button" id="equal" class="btn btn_default btn_hover_blue">=</button>
                                                    <button type="button" value="Результат" id="equal" class="operation btn btn_default btn_hover_blue">=</button>
                                                </td>
                                            </tr>
                                            <tr class="calc_buttons-row">
                                                <td colspan="2">
                                                    <button type="button" id="n0" class="btn btn_default btn_long">0</button>
                                                    <button type="button" id="n0" class="number btn btn_default btn_long">0</button>
                                                </td>
                                                <td>
                                                    <button type="button" class="btn btn_default ">.</button>
                                                    <button type="button" class="btn btn_default " id="decimal">.</button>
                                                </td>
                                            </tr>
                                        </table>
@@ -100,16 +101,21 @@ <h1 class="title">
                            </h1>
                            <div class="about">
                                <div class="about_btn">
                                    <a href="#" class="about_btn-link">
                                    <a href="#" id="howWorkBtn" class="about_btn-link">
                                    Как это работает?
                                </a>
                                </div>
                                <div>
                                    <ul id="operationsList">
                                    </ul>
                                </div>
                            </div>
                        </div>
                    </div>
                </main>
            </div>
        </div>
    </div>
    <script src="js/script.js"></script>
</body>
</html>
  
109  js/script.js
@@ -1 +1,110 @@
var Numbers = document.querySelectorAll('.number'),
    Operations = document.querySelectorAll('.operation'),
    DecimalBtn = document.getElementById('decimal'),
    ClearBtns = document.querySelectorAll('.clearBtn'),
    HowWorkBtn = document.getElementById('howWorkBtn'),
    Display = document.getElementById('display'),
    MemoryCurrentNumber = 0,
    MemoryNewNumber = false,
    MemoryPendingOperation = '',
    operationsList = document.getElementById('operationsList');
 for (var i = 0; i < Numbers.length; i++) {
    var number = Numbers[i];
    number.addEventListener('click', function (e) {
        numberPress(e.target.textContent);
    });
}
 for (var i = 0; i < Operations.length; i++) {
    var operationBtn = Operations[i];
    operationBtn.addEventListener('click', function (e) {
        operation(e.target.textContent);
    });
}
 for (var i = 0; i < ClearBtns.length; i++) {
    var clearBtn = ClearBtns[i];
    clearBtn.addEventListener('click', function (e) {
        clear(e.srcElement.id);
    });
};
 DecimalBtn.addEventListener('click', decimal);
 HowWorkBtn.addEventListener('click', howWork);
 function numberPress(number) {
    if (MemoryNewNumber) {
        display.value = number;
        MemoryNewNumber = false;
    } else {
        if (display.value === '0') {
            display.value = number;
        } else {
            display.value += number;
        };
    };
};
 function operation(op) {
    var localOperationMemory = display.value;
    if (MemoryNewNumber && MemoryPendingOperation !== '=') {
        display.value = MemoryCurrentNumber;
    } else {
        MemoryNewNumber = true;
        if (MemoryPendingOperation === '+') {
            MemoryCurrentNumber += parseFloat(localOperationMemory);
        } else if (MemoryPendingOperation === '-') {
            MemoryCurrentNumber -= parseFloat(localOperationMemory);
        } else if (MemoryPendingOperation === '*') {
            MemoryCurrentNumber *= parseFloat(localOperationMemory);
        } else if (MemoryPendingOperation === '/') {
            MemoryCurrentNumber /= parseFloat(localOperationMemory);
        } else {
            MemoryCurrentNumber = parseFloat(localOperationMemory);
        };
        display.value = MemoryCurrentNumber;
        MemoryPendingOperation = op;
    };
};
 function clear(id) {
    if (id === 'ce') {
        display.value = '0';
        MemoryNewNumber = true;
    } else if (id === 'c') {
        display.value = '0';
        MemoryNewNumber = true;
        MemoryCurrentNumber = 0;
        MemoryPendingOperation = '';
    };
};
 function decimal() {
    var localDecimalMemory = display.value;
     if (MemoryNewNumber) {
        localDecimalMemory = '0.';
        MemoryNewNumber = false;
    } else {
        if (localDecimalMemory.indexOf('.') === -1) {
            localDecimalMemory += '.';
        }
    };
    display.value = localDecimalMemory;
};
 function howWork(argument) {
    for (var i = 0; i < Operations.length; i++) {
        var newLi = document.createElement('li');
        var operationText = Operations[i].value;
        newLi.innerText = operationText;
        operationsList.appendChild(newLi);
    };
};
