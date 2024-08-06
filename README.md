<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Order Form</title>
<style>
body {
    font-family: Arial, sans-serif;
    background-color: #f7f7f7;
    margin: 0;
    padding: 20px;
}
h2 {
    color: #333;
}
form {
    background: #fff;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    max-width: 800px;
    margin: auto;
}
.form-row {
    display: flex;
    justify-content: space-between;
    margin-bottom: 15px;
}
.form-row label {
    flex-basis: 25%;
}
.form-row input, .form-row select, .form-row textarea {
    flex-basis: 70%;
    padding: 10px;
    margin-left: 5%;
    border: 1px solid #ccc;
    border-radius: 4px;
}
#productFields {
    display: flex;
    flex-wrap: wrap;
}
#productFields .product {
    display: flex;
    width: 100%;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 15px;
}
#productFields .product select, #productFields .product input {
    width: 15%;
    padding: 10px;
    margin-right: 2%;
}
#productFields .product button {
    width: auto;
    background: #d9534f;
    color: #fff;
    border: none;
    padding: 10px;
    cursor: pointer;
}
#productFields .product button:hover {
    background: #c9302c;
}
button.add-product {
    background: #5cb85c;
    color: #fff;
    border: none;
    padding: 10px;
    cursor: pointer;
}
button.add-product:hover {
    background: #4cae4c;
}
#orderList {
    max-width: 800px;
    margin: 20px auto;
    background: #fff;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}
#orderList table {
    width: 100%;
    border-collapse: collapse;
}
#orderList table, #orderList th, #orderList td {
    border: 1px solid #ccc;
}
#orderList th, #orderList td {
    padding: 10px;
    text-align: left;
}
</style>
</head>
<body>
<h2>Order Form</h2>
<form id="orderForm" method="post">
<div class="form-row">
    <label for="firmName">Firm Name:</label>
    <input type="text" id="firmName" name="Firm Name" required>
</div>
<div class="form-row">
    <label for="contactNumber">Contact Number:</label>
    <input type="text" id="contactNumber" name="Contact Number" required>
    <label for="remarks">Remarks/Comments:</label>
    <input type="text" id="remarks" name="Remarks/Comments">
</div>
<div class="form-row">
    <label for="city">City:</label>
    <input type="text" id="city" name="City" required>
    <label for="transporterName">Transporter Name:</label>
    <input type="text" id="transporterName" name="Transporter Name">
</div>
<div class="form-row">
    <label for="deliveryDate">Delivery Date:</label>
    <input type="date" id="deliveryDate" name="Delivery Date" required>
    <label for="transporterAddress">Transporter Address:</label>
    <input type="text" id="transporterAddress" name="Transporter Address">
</div>
<div class="form-row">
    <label for="creditDays">Credit in days:</label>
    <input type="number" id="creditDays" name="Credit in days" required>
    <label for="discountStatus">Discount Status:</label>
    <select id="discountStatus" name="Discount Status" required>
        <option value=""></option>
        <option value="✅">✅</option>
        <option value="❌">❌</option>
    </select>
</div>
<div class="form-row">
    <label for="estimateBy">Estimate by which person:</label>
    <select id="estimateBy" name="Estimate by which person" required>
        <option value="Sanjeev sir">Sanjeev sir</option>
        <option value="Kashish sir">Kashish sir</option>
        <option value="Kajal mam">Kajal mam</option>
        <option value="Natwar">Natwar</option>
        <option value="Deepak">Deepak</option>
        <option value="Pradeep">Pradeep</option>
        <option value="CRM">CRM</option>
        <option value="Akshay kumar">Akshay kumar</option>
        <option value="EA">EA</option>
        <option value="MIS">MIS</option>
    </select>
    <label for="visitingCard">Visiting Card:</label>
    <input type="file" id="visitingCard" name="Visiting Card">
</div>
<div id="productFields">
    <div class="product">
        <select name="Product Name0" required>
            <option value="" disabled selected>Product Name</option>
            <option value="2.1 kg">2.1 kg</option>
            <option value="2.2 kg">2.2 kg</option>
            <option value="2.3 kg">2.3 kg</option>
            <option value="2.4 kg">2.4 kg</option>
            <option value="2.5 kg">2.5 kg</option>
            <option value="2.6 kg">2.6 kg</option>
            <option value="2.7 kg">2.7 kg</option>
            <option value="2.8 kg">2.8 kg</option>
            <option value="3 kg">3 kg</option>
            <option value="Floor">Floor</option>
            <option value="Jumbo (24 inch)">Jumbo (24 inch)</option>
            <option value="Super Jumbo (36 inch)">Super Jumbo (36 inch)</option>
            <option value="Z1">Z1</option>
            <option value="Z2">Z2</option>
            <option value="Z3">Z3</option>
            <option value="Z4">Z4</option>
            <option value="SS 8">SS 8</option>
            <option value="SS 13">SS 13</option>
            <option value="SS 16">SS 16</option>
            <option value="SS 19">SS 19</option>
            <option value="SS 24">SS 24</option>
            <option value="MS 13">MS 13</option>
            <option value="MS 16">MS 16</option>
            <option value="MS 19">MS 19</option>
            <option value="MS 24">MS 24</option>
        </select>
       <input type="text" name="Quantity0" placeholder="Quantity" required>	
<input type="number" name="Price" placeholder="Price" required>	
<select name="Trolley colour">	
<option value="" disabled selected>Trolley colour</option>	
<option value="Grey">Grey</option>	
<option value="Black">Black</option>	
<option value="White">White</option>	
</select>	
<select name="Trolley packing">	
<option value="" disabled selected>Trolley packing</option>	
<option value="LG">LG</option>	
<option value="Laminated">Laminated</option>	
<option value="Zabric">Zabric</option>	
</select>	
<select name="AC Stand packing Types">	
<option value="" disabled selected>AC Stand packing Types</option>	
<option value="Bag(16pcs)">Bag(16pcs)</option>	
<option value="Bag(20pcs)">Bag(20pcs)</option>	
<option value="Box(12pcs)">Box(12pcs)</option>	
</select>	
<select name="AC Fastener">	
<option value="" disabled selected>AC Fastener</option>	
<option value="Rawal">Rawal</option>	
<option value="Pin Type/Bullet/Zebra">Pin Type/Bullet/Zebra</option>	
<option value="Killa">Killa</option>	
<option value="Special Type Anchor">Special Type Anchor</option>	
<option value="None">None</option>	
<option value="Other">Other</option>	
	
</select>	
<select name="AC Stand Powder Types">	
<option value="" disabled selected>AC Stand Powder Types</option>	
<option value="Regular">Regular</option>	
<option value="Premium">Premium</option>	
</select>	
        <button type="button" class="remove-product" onclick="removeProduct(this)">Remove</button>
    </div>
</div>
<button type="button" class="add-product" onclick="addProduct()">Add Product</button>
<br><br>
<button type="submit">Submit</button>
</form>

<h2>Submitted Orders</h2>
<div id="orderList">
    <table>
        <thead id="orderHeaders"></thead>
        <tbody id="orderBody"></tbody>
    </table>
</div>

<script>
function addProduct() {
    const productFields = document.getElementById('productFields');
    const productTemplate = productFields.querySelector('.product');
    const newProduct = productTemplate.cloneNode(true);
    const inputs = newProduct.querySelectorAll('input, select');
    const index = productFields.children.length;
    inputs.forEach(input => {
        const name = input.name;
        input.name = name.replace(/\d+$/, '') + index;
        input.value = '';
    });
    productFields.appendChild(newProduct);
}

function removeProduct(button) {
    const productFields = document.getElementById('productFields');
    if (productFields.children.length > 1) {
        productFields.removeChild(button.parentNode);
    } else {
        alert("Cannot remove the last product field.");
    }
}

document.getElementById('orderForm').addEventListener('submit', function(event) {
    event.preventDefault();
    const formData = new FormData(this);
    const data = {};

    formData.forEach((value, key) => {
        const match = key.match(/(.*?)(\d*)$/);
        if (match) {
            const field = match[1];
            const index = match[2] || '0';
            if (!data[field]) {
                data[field] = [];
            }
            data[field][index] = value;
        }
    });

    google.script.run.withSuccessHandler(response => {
        if (response.status === 'Success') {
            alert('Order submitted successfully!');
            this.reset();
            loadOrders(); // Load orders after successful submission
        } else {
            alert('Error submitting order: ' + response.message);
        }
    }).withFailureHandler(error => {
        console.error('Error:', error);
        alert('Error submitting order: ' + error.message);
    }).doPost({ postData: { contents: JSON.stringify(data) } });
});

function loadOrders() {
    google.script.run.withSuccessHandler(displayOrders).getOrders();
}

function displayOrders(data) {
    const headers = data[0];
    const orders = data.slice(1);
    const orderHeaders = document.getElementById('orderHeaders');
    const orderBody = document.getElementById('orderBody');
    orderHeaders.innerHTML = '';
    orderBody.innerHTML = '';
    const headerRow = document.createElement('tr');
    headers.forEach(header => {
        const th = document.createElement('th');
        th.textContent = header;
        headerRow.appendChild(th);
    });
    orderHeaders.appendChild(headerRow);
    orders.forEach(order => {
        const row = document.createElement('tr');
        order.forEach(cell => {
            const td = document.createElement('td');
            td.textContent = cell;
            row.appendChild(td);
        });
        orderBody.appendChild(row);
    });
}

document.addEventListener('DOMContentLoaded', loadOrders);
</script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/google-apps-script/1.0.0/google-apps-script.js"></script>
</body>
</html>
