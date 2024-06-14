function calculateTripCost() {
  var vehicle_mpg = parseFloat(document.getElementById('vehicle_mpg').value);
  var gas_cost = parseFloat(document.getElementById('gas_cost').value);
  var trip_miles = parseFloat(document.getElementById('trip_miles').value);
  if (isNaN(vehicle_mpg) || isNaN(gas_cost) || isNaN(trip_miles)) {
    alert('Please enter valid numbers');
    return;
  }

  var total_gas_needed = trip_miles / vehicle_mpg;
  var total_cost = total_gas_needed * gas_cost;

  document.getElementById('result-total').textContent = total_cost.toFixed(2);

  document.getElementById('step1').textContent = trip_miles + " miles / " + vehicle_mpg + " MPG = " + total_gas_needed.toFixed(2) + " gallons";
  document.getElementById('step2').textContent = total_gas_needed.toFixed(2) + " gallons * $" + gas_cost + " = $" + total_cost.toFixed(2);
}

function clearFields() {
  document.getElementById('vehicle_mpg').value = '';
  document.getElementById('gas_cost').value = '';
  document.getElementById('trip_miles').value = '';
  document.getElementById('result-total').textContent = '';
  document.getElementById('step1').textContent = '';
  document.getElementById('step2').textContent = '';
}
