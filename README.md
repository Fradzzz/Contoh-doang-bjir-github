<html>
<meta charset='UTF-8' />
<meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport' />
<meta content='IE=edge' http-equiv='X-UA-Compatible' />
<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script>
<script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script>
<link href="https://feeldreams.github.io/kaloada/style.css" rel="stylesheet" type="text/css" />

<head>
    <title>Script HTML Feeldream Repl Co</title>
</head>

<body>

    <audio src="https://kaloada.feeldream.repl.co/kaloada.mp3" id="linkmp3" class="sembunyi"></audio>

    <div id="bgbelakang">
        <img src="" id="wallpaper" />
    </div>

    <div class="overlay">
        <div class="loading-message">Harap tunggu...</div>
    </div>

    <div id='Content'>

        <p id="ket">Klik di bawah ya <3</p> <div>
                <div id="loveIn" class="awalan">
                    <svg class='line' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24'>
                        <g transform='translate(2.000000, 2.000000)'>
                            <path
                                d='M9.27542857,0.714285714 C14.0030476,0.714285714 17.836381,4.54666667 17.836381,9.2752381 C17.836381,14.0038095 14.0030476,17.8361905 9.27542857,17.8361905 C4.54685714,17.8361905 0.71447619,14.0038095 0.71447619,9.2752381 C0.71447619,4.54666667 4.54685714,0.714285714 9.27542857,0.714285714 Z'>
                            </path>
                            <path
                                d='M17.8989524,16.487619 C18.678,16.487619 19.3094286,17.12 19.3094286,17.8980952 C19.3094286,18.6780952 18.678,19.3095238 17.8989524,19.3095238 C17.1199048,19.3095238 16.4875238,18.6780952 16.4875238,17.8980952 C16.4875238,17.12 17.1199048,16.487619 17.8989524,16.487619 Z'>
                            </path>
                        </g>
                    </svg>
                    <label>S.id/kaloada</label>
                </div>
    </div>

    <div><img id="fotosatu" src="" /><img id="fotodua" src="" /><img id="fototiga" src="" /><img id="fotoempat"
            src="" /><img id="fotolima" src="" /><img id="fotoenam" src="" /><img id="fototujuh" src="" /></div>

    <div>
        <blockquote id='bq'>
            <p id="kalimat"></p>
            <p id="kalimatc"></p>
        </blockquote>
    </div>

    <div id="contTom"><a id="By" class='button' onClick="sjawab()">Klik Ini</a></div>

    </div>

    <script src="https://feeldreams.github.io/kaloada/script.js"></script>

    <script type="text/javascript">
        Content.style = "display:none";
        async function menuju() {
            await swals.fire('Kirim pesan ke WhatsApp aku, ya!');
            window.location = "https://api.whatsapp.com/send?phone=&text=" + pesanwhatsapp;
        }

        async function jawab() {
            var {
                value: jawaban
            } = await swals.fire({
                title: 'Ketik Pesan Kamu &#128073;&#128072;',
                input: 'text',
                allowOutsideClick: false,
                showCancelButton: false,
            });
            if (jawaban && jawaban.length < 21) {
                window.jawaban = jawaban;
                pesanwhatsapp = jawaban;
                finalakhir();
            } else {
                await swals.fire('Ups!', 'Jawaban tidak boleh kosong atau lebih dari 20 karakter, ya!');
                jawab();
            }
        }

        function pergantian() {
            setTimeout(gantikata, 0900); //1
            setTimeout(gantikata, 3300); //2
            setTimeout(gantikata, 4800); //3
            setTimeout(gantikata, 7500); //4
            setTimeout(gantikata, 8400); //5
        }

        async function pertama() {
            kata1 = "Kalo ada yang<br>deketin kamu ðŸ« ";
            kata2 = "Bilang ajaa..";
            kata3 = "Kamu punya<br>aku sekarang ðŸ‘‰ðŸ‘ˆ";
            kata4 = "Titik. ðŸ˜¡";
            katangetik = "Gapake koma ðŸ˜‹ðŸ’—";

            fotosatu.style = "display:inline-flex";
            audio.play();
            showDiv()
        }
    </script>
</body>

</html>
