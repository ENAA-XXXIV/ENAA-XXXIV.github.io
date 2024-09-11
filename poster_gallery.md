
<html lang="en">
<head>
    <script>
    function checkPassword() {
        var password = document.getElementById("passwordBox").value;
        var passwordHash = "posters@enaa2024"; // SHA-256 hash of "password"
        
        if (password === passwordHash) {
            document.getElementById("content").style.display = "block";
            document.getElementById("passwordPrompt").style.display = "none";
        } else {
            alert("Wrong password! You will be redirected.");
            window.location.href = "https://enaa-xxxiv.github.io/index"; // Redirect if incorrect
        }
    }
    </script>
    <style>
        div.gallery {
            margin-bottom: 50px;
            margin-top: 50px;
            margin-left: 10px;
            margin-right: 10px;
            border: 1px solid #ccc;
            float: left;
            width: 180px;
            height: 200px
        }

        div.gallery:hover {
            border: 1px solid #777;
        }

        div.gallery img {
            width: 100%;
            height: 100%;
            display: block;
        }

        div.desc {
            padding: 5px;
            text-align: center;
            font-size: 12px
        }

        div.name {
            padding: 5px;
            text-align: center;
            font-size: 12px;
            font-weight: bold;
        }
    </style>
</head>

<body>
    <div id="passwordPrompt">
        <label for="passwordBox">Enter Password:</label>
        <input type="password" id="passwordBox">
        <button onclick="checkPassword()">Submit</button>
    </div>
<div>
<h1 id="poster-gallery">Poster Gallery</h1>

<div>
You can find a gallery of the posters for this conference below. Click on the image to open the poster. Click on the poster title to see the corresponding abstract.
</div>


    <div class="gallery">
    <a target="_blank" href="assets/posters/poster-id-2.pdf">
        <img src="assets/posters/poster-id-2.png" alt="Poster <i>Product Design for Scientific Literacy: development of a multifunctional orrery for cognitive stimulation</i> by F. Alves">
    </a>
    <div class="name">F. Alves</div>
    <div class="desc">
     <a href=https://enaa-xxxiv.github.io/abstract_book#abs-2> 
        Product Design for Scientific Literacy: development of a multifunctional orrery for cognitive stimulation
     </a>
    </div>
    </div>

    <div class="gallery">
    <a target="_blank" href="assets/posters/poster-id-12.pdf">
        <img src="assets/posters/poster-id-12.png" alt="Poster <i>OLHANDO O FIRMAMENTO: A OBSERVAÇÃO ASTRONÓMICA NO ATUAL TERRITÓRIO PORTUGUÊS DURANTE O NEOLÍTICO</i> by T. Canhota">
    </a>
    <div class="name">T. Canhota</div>
    <div class="desc">
     <a href=https://enaa-xxxiv.github.io/abstract_book#abs-12> 
        OLHANDO O FIRMAMENTO: A OBSERVAÇÃO ASTRONÓMICA NO ATUAL TERRITÓRIO PORTUGUÊS DURANTE O NEOLÍTICO
     </a>
    </div>
    </div>

    <div class="gallery">
    <a target="_blank" href="assets/posters/poster-id-45.pdf">
        <img src="assets/posters/poster-id-45.png" alt="Poster <i>The stellar activity in stars with exoplanets</i> by T. Monteiro">
    </a>
    <div class="name">T. Monteiro</div>
    <div class="desc">
     <a href=https://enaa-xxxiv.github.io/abstract_book#abs-45> 
        The stellar activity in stars with exoplanets
     </a>
    </div>
    </div>

    <div class="gallery">
    <a target="_blank" href="assets/posters/poster-id-66.pdf">
        <img src="assets/posters/poster-id-66.png" alt="Poster <i>"A JWST IFU deep study of gas, dust, and PAHs in a prototypical externally illuminated protoplanetary disk"</i> by S. Vicente">
    </a>
    <div class="name">S. Vicente</div>
    <div class="desc">
     <a href=https://enaa-xxxiv.github.io/abstract_book#abs-66> 
        "A JWST IFU deep study of gas, dust, and PAHs in a prototypical externally illuminated protoplanetary disk"
     </a>
    </div>
    </div>

    
</div>
    
</body>

</html>

