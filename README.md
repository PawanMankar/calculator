# calculator
Simple Calcultor HTML Code
Created to perform basic arthmatic oprations like (additon,sub,mul,div)
<!DOCTYPE html>
<html>

<head>
    <title>My-Calculator</title>

    
</head>

<body >
    <h2>PM-Calculator</h2>
    <form name="calculator">
        <hr>
        <input type="text" width: 120px; name="display" id="display" readonly>
        <br>
        
        <input type="button" value="1" onclick="addToDisplay('1')">&nbsp;
        <input type="button" value="2" onclick="addToDisplay('2')">&nbsp;
        <input type="button" value="3" onclick="addToDisplay('3')">&nbsp;
        <input type="button" value="+" onclick="addToDisplay('+')">
        <br>
        <input type="button" value="4" onclick="addToDisplay('4')">&nbsp;
        <input type="button" value="5" onclick="addToDisplay('5')">&nbsp;
        <input type="button" value="6" onclick="addToDisplay('6')">&nbsp;
        <input type="button" value="-" onclick="addToDisplay('-')">
        <br>
        <input type="button" value="7" onclick="addToDisplay('7')">&nbsp;
        <input type="button" value="8" onclick="addToDisplay('8')">&nbsp;
        <input type="button" value="9" onclick="addToDisplay('9')">&nbsp;
        <input type="button" value="*" onclick="addToDisplay('*')">
        <br>
        <input type="button" value="C" onclick="clearDisplay()"> 
        <input type="button" value="0" onclick="addToDisplay('0')">&nbsp;
        <input type="button" value="=" onclick="calculate()"> &nbsp;
        <input type="button" value="/" onclick="addToDisplay('/')"> 
        <hr>
    </form>
    <br>
    <br>
    <br>

    <p>Created By Pawan Mankar<p>
        <p> Connect Me On Github :
        
           <a href="https://github.com/PawanMankar"><button>GITHUB</button></a>
        </p>


    <script>
        function addToDisplay(value) {
            document.calculator.display.value += value;
        }

        function clearDisplay() {
            document.calculator.display.value = "";
        }

        function calculate() {
            try {
                document.calculator.display.value = eval(document.calculator.display.value);
            } catch (error) {
                document.calculator.display.value = "Error";
            }
        }
    </script>
</body>

</html>
