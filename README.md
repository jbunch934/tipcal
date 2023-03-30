function calculateTip() {
    // Get the values of the inputs
    var totalBill = parseFloat(document.getElementById("total-bill").value);
    var numGuests = parseInt(document.getElementById("num-guests").value);
    var qualityOfService = parseFloat(document.getElementById("quality-of-service").value);
    
    // Calculate the tip
    var tip = totalBill * qualityOfService;
    var tipPerGuest = tip / numGuests;
    
    // tip amount
    document.getElementById("tip-amount").innerHTML = "Tip Amount: $" + tip.toFixed(2) + "<br>Tip Per Guest: $" + tipPerGuest.toFixed(2);
  }

  <!DOCTYPE html>
<html>
  <head>
    <title>Tip Calculator</title>
  </head>
  <body>
    <h1>Tip Calculator</h1>
    <p>Calculate the Bill:</p>
    <form>
      <label for="total-bill">Total Bill:</label>
      <input type="number" id="total-bill" name="total-bill"><br><br>
      
      <label for="num-guests">Number of Guests:</label>
      <input type="number" id="num-guests" name="num-guests"><br><br>
      
      <label for="quality-of-service">Quality of Service:</label>
      <select id="quality-of-service" name="quality-of-service">
        <option value="0.2"> (20%)</option>
        <option value="0.15">(18%)</option>
        <option value="0.1">(15%)</option>
        <option value="0.05">(10%)</option>
      </select><br><br>
      
      <input type="button" value="Calculate Tip" onclick="calculateTip()">
    </form>
    
    <p id="tip-amount"></p>
  </body>
  
  <script src="tip.js">
    
  </script>
</html>
# tipcal
# tipcal
# tipcal
# tipcal
