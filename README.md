<html>
<head><title>calculator</title>
<style>
input {
    font-size: 52px;
    border-block: 2px black;

}
p{
    font-size: 25px;
}
body{
text-align:center;
background-image: linear-gradient(45deg, rgb(0, 255, 213), grey);;}
button {
    font-size: 45px;
    background-color: gray;
}
select {
    font-size:45px;
    
}
</style></head>
<script>
            
            function calc()
            {
                var n1 = parseFloat(document.getElementById('n1').value);
                var n2 = parseFloat(document.getElementById('n2').value);
                
                var oper = document.getElementById('operators').value;
                
                if(oper === '+')
                {
                    document.getElementById('result').value = n1+n2;
                }
                
                if(oper === '-')
                {
                    document.getElementById('result').value = n1-n2;
                }
                
                if(oper === '/')
                {
                    document.getElementById('result').value = n1/n2;
                }
                
                if(oper === 'X')
                {
                    document.getElementById('result').value = n1*n2;
                }
            }
            
        </script>
        
    </head>
    <body>
	<h1>Basic calculator</h1>
        
    <p>Enter A Number </p>  <input type="text" id="n1" required><br/><br/>
     <p> Enter B Number </p><input type="text" id="n2" required/><br/><br/>
        
        <select id="operators">
            <option value="+">+</option>
            <option value="-">-</option>
            <option value="/">/</option>
            <option value="X">X</option>
        </select>
        
        <button onclick="calc();">result</button>
       <p>Result</p> <input type="text" id="result"/>
        
    </body>
</html>
