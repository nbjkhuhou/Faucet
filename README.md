<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Faucet Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        .container {
            margin-top: 50px;
        }
        .balance {
            font-size: 24px;
            margin-bottom: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Faucet Website</h1>
        <div class="balance">Your balance: <span id="balance">0</span> Gá</div>
        <button onclick="claim()">Claim Gá</button>
    </div>

    <script>
        let balance = 0;

        function claim() {
            balance += 1; // Increase balance by 1 on each claim
            document.getElementById("balance").textContent = balance;
            alert("You claimed 1 Gá!");
        }
    </script>
</body>
</html>
