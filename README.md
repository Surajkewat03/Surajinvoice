<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Invoice Generator</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      background: #f4f4f4;
      color: #333;
    }
    .container {
      background: #fff;
      padding: 20px;
      max-width: 900px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    h1 {
      text-align: center;
    }
    .row {
      display: flex;
      justify-content: space-between;
      margin: 10px 0;
    }
    .input-group {
      flex: 1;
      margin: 5px;
    }
    input, select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 20px;
    }
    th, td {
      padding: 12px;
      border: 1px solid #ccc;
      text-align: left;
    }
    .btn {
      display: block;
      width: 100%;
      padding: 12px;
      margin-top: 20px;
      background: #6c5ce7;
      color: white;
      border: none;
      font-size: 16px;
      cursor: pointer;
    }
    .btn:hover {
      background: #5a4dcf;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Invoice</h1>
    <div class="row">
      <div class="input-group">
        <label>Invoice No</label>
        <input type="text" placeholder="A0001">
      </div>
      <div class="input-group">
        <label>Invoice Date</label>
        <input type="date" value="2025-07-27">
      </div>
    </div>
    <div class="row">
      <div class="input-group">
        <label>Billed By (Your Details)</label>
        <input type="text" placeholder="Your Business Name">
      </div>
      <div class="input-group">
        <label>Billed To (Client's Details)</label>
        <input type="text" placeholder="Client's Business Name">
      </div>
    </div>
    <div class="row">
      <div class="input-group">
        <label>Email</label>
        <input type="email" placeholder="your@email.com">
      </div>
      <div class="input-group">
        <label>Phone</label>
        <input type="tel" placeholder="+44 123456789">
      </div>
    </div>
    <table>
      <thead>
        <tr>
          <th>Item Name</th>
          <th>Qty</th>
          <th>Rate</th>
          <th>Amount</th>
        </tr>
