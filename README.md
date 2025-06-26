<!DOCTYPE html>
<!DOCTYPE html>
<html lang="as">
<head>
  <meta charset="UTF-8">
  <title>A Letter to Niharika</title>
  <style>
    body {
      margin: 0;
      font-family: 'Georgia', serif;
      background: linear-gradient(to bottom right, #fff0f5, #ffe0ec);
      color: #5c1a47;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 20px;
      text-align: center;
    }

    .slide {
      display: none;
      max-width: 900px;
      background: rgba(255, 255, 255, 0.95);
      padding: 34px;
      border-radius: 20px;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.15);
    }

    .slide.active {
      display: block;
      animation: fadein 1s;
    }

    @keyframes fadein {
      from { opacity: 0; transform: scale(0.97); }
      to { opacity: 1; transform: scale(1); }
    }

    button {
      margin-top: 30px;
      padding: 12px 28px;
      font-size: 1em;
      background-color: #f06292;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    button:hover {
      background-color: #e91e63;
    }

    footer {
      margin-top: 20px;
      font-size: 0.9em;
      color: #8e3a63;
    }
  </style>
</head>
<body>

<div id="slides">

  <div class="slide active">
    <h1>Why one should love Niharika Gogoi<br>and how I am slowly falling in it</h1>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Tai khana dhuniya bonai,<br>
      so moi jodi tair logot bohi ghanta kotha patibo paru<br>
      aru taik sohai koribo paru—<br>
      then khua aru tair hator dhuniya khana.
    </p>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Life-t ketia-u tumak bore hubo nidie,<br>
      jetia mon beya — tair logot duta kotha pata,<br>
      misikiya hahi tu mukhot loi — hai xubo dibo tai.
    </p>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Jetia professor-r gaali aru chemistry equation buji nupua hubo,<br>
      tetia room-r pa ulai tai hahi tu mari tumar loi rokhi thakibo —<br>
      taat ke bhal feeling ki hubo?
    </p>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Tair height-t mutke xoru,  
      so jetia hug koribo—sob tension pahori taik fully hug koribo parim.  
      Ru jetia ekeloge khuj karhim, hath tu dhori,  
      pakka June dekhe kobo: "cute lagise duyu 💓"
    </p>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Tai xunkale theh lage,  
      so taik monaute monaute juntu bhl lagibo—seitu bhl.  
      Ru kot paba hei?
    </p>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Tair dukh-t hath tu dhori just bohi tair kotha xuni,  
      jodi tumi taik alp holeu xanti disa—  
      ru ki lage oo tumak?
    </p>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Tair soku kita bahut dhuniya oo, tai koi kiba kibi—  
      but jetia moi dekhilu college-t, sei soku kita nije eta natun kahani  
      aru moi sai bahut bhal pau.  
      (Moi tu taik sei cute chosma jurat-u bor bhal pau)
    </p>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Tai hahi tu oo, ketiaba jodi mur karone sei hahi tu jabo gei lage  
      moi ketia-u nijok xoma koribo nuarim—  
      because mur karone sei hahi tu mut-ke-u important.  
      Xosaye xoday sei hahi tu logot thaka therapy-t ke kom nohoi.
    </p>
    <button onclick="nextSlide()">Next</button>
  </div>

  <div class="slide">
    <p>
      Thank you mur life-t exist kora karone.  
      Idk xopun-ru dithok kiman usarat tumar logot,  
      but I hope one day.  
      Ru jodi nohoi-u, jar logot hubo xi xosaye, tar life is just best.  
      Moi etia pa-ye jealous and I just hope seitu future me-ye hou.  
      Tumi best—everything from the minute details.  
      You’re the missing piece of my puzzle of life.
    </p>
    <footer>— With all the warmth I never found words for, but finally did.</footer>
  </div>

</div>

<script>
  const slides = document.querySelectorAll('.slide');
  let index = 0;

  function nextSlide() {
    if (index < slides.length - 1) {
      slides[index].classList.remove('active');
      index++;
      slides[index].classList.add('active');
    }
  }
</script>

</body>
</html>
