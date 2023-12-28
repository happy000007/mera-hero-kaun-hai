<!DOCTYPE html>
<html lang="en">
<head>
<marquee direction="left"><Font size="7">aapka future aapke hath mai hai "Jai Baba ki" </font></marquee>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form</title>
</head>
<body>
    <form onsubmit="showHeroMessage()">
        <p>Enter Your Name<br>
            <input type="text" placeholder="Enter" name="name"></p>

        <p>Enter Your favourite Hero Name<br>
            <input type="text" placeholder="Enter" name="hero"></p>

        <p>Enter Your Date of birth<br>
            <input type="date" placeholder="Enter Your Dob" name="dob"></p>

        <p>Enter Your Mobile Number<br>
            <input type="tel" placeholder="Enter" name="mobile"></p>

        <p>Enter Your Password<br>
            <input type="password" placeholder="Enter Your Password" name="password"></p>

        <p align="center">
            <input type="submit" value="Login">
        </p>
    </form>

    <!-- Message to be displayed after submission -->
    <p id="heroMessage" style="font-size: 20px; color: red; text-align: center;"></p>

    <script>
        function showHeroMessage() {
            // Prevent the form from submitting (for demonstration purposes)
            event.preventDefault();

            // Get the hero name entered by the user
            var hero = document.getElementsByName('hero')[0].value;

            // Construct the message
            var message = hero + " ka gu kha le<br> bhul gya bhagat singh or jinhone desh ke liye apni jan de di , abe apne per dada ka hi name likh detA.";

            // Display the message with increased font size, red color, and centered
            var heroMessageElement = document.getElementById('heroMessage');
            heroMessageElement.innerHTML = message;
            heroMessageElement.style.display = 'block';
        }
    </script>
</body>
</html>
