<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>example of div</title>
</head>
<body>
    <div>
        <h2>Contact form</h2>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" placeholder="Enter your name">
    </div>
    <br>
    <div>
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" placeholder="Enter your email">
    </div>
    <div>
        <label for="phone">Phone Number:</label>
        <input type="tel" id="Phone" name="Phone" 
        placeholder="Enter your 10 digit phone number" pattern="[0-9]{10}" 
        inputmode="numeric" required aria-required="true"
        aria-describedby="phone-error"
        onkeypress="restrictAlphabets(event)">
        <span id="phone-error" role="alert" 
        style="display: none;">numbers only.</span>"></span>
    </div>
    <script>
        function restrictAlphabets(event){
            const key=event.key;
            if(!/[0-9]/.test(key) && key !=="Backspace" && key !=="Arrowlight"){
                event.preventDefault();
            }
        }
    </script>
</body>
</html># div
html
