written in bootstrap and js
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Fire-with-code</title>
        <link rel="stylesheet" href="style.css" />
        <script src="script.js"></script>
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="<KEY>" crossorigin="anonymous">
    </head>
    <body>
        <div id="login-area" class="mt-5">
            <h1 class="text-center">Welcome to Fire-with-code Bank</h1>
            <div id="login-box" class="container rounded p-5 shadow mt-5">
                <h3>Login</h3>
              <input type="text" class="form-control" placeholder="email">
              <br>
              <input type="password" class="form-control" placeholder="password">
              <br
             <button id="submit-btn" class="btn btn-success">Submit</button>
            </div>
        </div>
        <div id="dashboard" class="d-none mt-5 container">
            <div class="d-flex justify-content-center">
                <div class="col-md-3 bg-info ms-5 p-4 rounded">
                    <h2>Deposit</h2>
                    <p class="fs-3">
                        $ <span id="deposit">0</span>
                    </p>
                </div>
                <div class="col-md-3 bg-success ms-5 p-4 rounded"></div>
                <h2>Withdraw</h2>
                <p class="fs-3">
                    $ <span id="withdraw">0</span>
                </p>
            </div>
            <div class="col-md-3 bg-primary ms-5 p-4 rounded">
                <h2>Balance</h2>
                <p class="fs-3">
                    $ <span id="balance">1200</span>
                </p>
            </div>
        </div>
        <div id="input-section" class="mt-5 d-flex justify-content-center">
            <div class="col-md-5 container rounded shadow p-4">
                <h3>Deposit</h3>
                <input type="number" class="form-control" id="deposit-input" placeholder="Deposit"/>
                <br>
                <button class="btn btn-success" id="deposit-btn">Deposit</button> 
            </div>
            <div class="col-md-5 container rounded shadow p-4">
                <h3>Withdraw</h3>
                <input type="number" class="form-control" id="withdraw-input" placeholder="Withdraw"/>
                <br>
                <button class="btn btn-danger" id="withdraw-btn">Withdraw</button>
            </div>
        </div>
        <script>
            const loginArea =document.getElementById("login-area");
            const depositInput = document.getElementById("deposit-input");
            const depositBtn = document.getElementById("deposit-btn");
            const withdrawInput = document.getElementById("withdraw-input");
            const submitBtn =document.getElementById("submit-btn");
            const dashboard = document.getElementById("dashboard");
            const balance = document.getElementById("balance");
            const deposit = document.getElementById("deposit");
            const withdraw = document.getElementById("withdraw");
            const withdrawBtn =document.getElementById("withdraw-btn");

            submitBtn.addEventListener("click",() => {
                loginArea.style.display ='none';
                dashboard.classList.remove("d-none");
            })
        </script>
    </body>
</html>
