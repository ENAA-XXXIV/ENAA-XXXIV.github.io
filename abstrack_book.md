<!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Password Protected Page</title>
       <script>
       function checkPassword() {
           var password = document.getElementById("passwordBox").value;
           var passwordHash = "enaa2024@gui"; // SHA-256 hash of "password"
           
           if (password === passwordHash) {
               document.getElementById("content").style.display = "block";
               document.getElementById("passwordPrompt").style.display = "none";
           } else {
                alert("Wrong password! You will be redirected.");
                window.location.href = "https://enaa-xxxiv.github.io/index"; // Redirect if incorrect
           }
       }
       </script>
   </head>
   <body>
       <div id="passwordPrompt">
           <label for="passwordBox">Enter Password:</label>
           <input type="password" id="passwordBox">
           <button onclick="checkPassword()">Submit</button>
       </div>
       <div id="content" style="display:none;">
           <h1>Secret Content</h1>
           <p>This is the protected content of your page.</p>
       </div>
   </body>
   </html>