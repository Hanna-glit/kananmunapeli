# kananmunapeli
<!doctype html>

<head>
    <title>Morjesta</title>
    <style>
        #kananmuna {
            max-width: 100vw;
            max-height: 100vh;
        }
    </style>
</head>

<body>
    <h1 id="tulostaulu">0</h1>
    <img id="kananmuna" onclick="kananmunanKlikkaus()" src="kananmuna-ehja.jpg" />
    <script>

        let laskurinLukema = 0;

        let kananmunaElem = document.getElementById("https://cdn.pixabay.com/photo/2014/11/22/15/31/eggs-541763__340.jpg")
        let tulostauluElem = document.getElementById("https://cdn.pixabay.com/photo/2018/02/12/20/11/sorbian-easter-eggs-3149016__340.jpg")

        function kananmunanKlikkaus() {
            laskurinLukema = laskurinLukema + 1
            console.log(laskurinLukema)

            // päivitetään klikkausten määrä käyttöliittymään
            tulostauluElem.innerHTML = laskurinLukema

            if(laskurinLukema > 5) {
                kananmunaElem.src="https://cdn.pixabay.com/photo/2018/02/12/20/11/sorbian-easter-eggs-3149016__340.jpg" 
                laskurinLukema = 0
                alert("Voitit pelin")
            } 
            else {
                kananmunaElem.src="https://cdn.pixabay.com/photo/2014/11/22/15/31/eggs-541763__340.jpg"
            }
        }

    </script>
</body>
