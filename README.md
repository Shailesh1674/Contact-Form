# Contact-Form
This project features a responsive contact form built with HTML and CSS. It collects user name, email, and message, styled with a light blue background and rounded corners for a user-friendly interface. The form submits data via POST to Formspree, ideal for personal or small business websites needing a simple contact solution.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        form{
            text-align: center;
            margin: 3%;
            padding: 3%;
            width: auto;
            height: auto;
            background-color: aliceblue;
            border-radius: 10px;
            border: 2px solid;
            border-color: black;
        }
        #name, #email, #message{
            font-family:Arial, Helvetica, sans-serif;
            font-size: large;
            padding: 2px;
            margin: 5px;
            width: 100%;
            border-radius: 5px;
        }
        textarea{
            border-radius: 10px;
            width: 100%;
            border: 2px solid black;
        }
        .submit{
            text-align: center;
            background-color: rgb(0, 174, 255);
            font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
            font-size: larger;
            border-radius: 5px;
        }
    </style>
<body>
    <form action="https://formspree.io/f/mkgwryno" method="post">
        <label for="name" style="padding: 10px;">Your Name*</label>
        <br><input type="text" name="name" id="name" required placeholder="[FIrst Name] [Middle Name] [Last Name]">
        <br>
        <label for="email" style="padding: 10px;">Email*</label>
        <br>
        <input type="email" name="email" id="email" required placeholder="xyz@gmail.com">
        <br><br>
        <label for="message" style="padding: 10px;">Message*</label>
        <br>
        <textarea name="message" id="message" rows="5" cols="10" required placeholder="Your Query !"></textarea>
        <br><br>
        <input type="submit" value="Submit" class="submit">
    </form>
</body>
</html>
