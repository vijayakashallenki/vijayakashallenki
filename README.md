## Hi there👋

@import url("https://fonts.googleapis.com/css2?family=Baloo+Paaji+2:wght@400;500&display=swap");

.container {
  display: grid;
  grid-template-columns: 300px 300px;
  grid-gap: 50px;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-image:url("https://images.pexels.com/photos/998641/pexels-photo-998641.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500");
  background-size: cover;
  font-family: 'Baloo Paaji 2', cursive;
}

.card {
  background-color: #222831;
  height: 37rem;
  border-radius: 5px;
  display: flex;
  flex-direction: column;
  align-items: center;
  box-shadow: rgba(0, 0, 0, 0.7);
  color: white;
}


.card__name {
  margin-top: 10px;
  font-size: 1.5em;
}

.card__image2{
    height: 160px;
    width: 160px;
    border-radius: 50%;
    border: 5px solid #570508;
    margin-top: 20px;
    box-shadow: 0 10px 50px #950b09;
  }

.btn {
  background: none;
  border: none;
  cursor: pointer;
  line-height: 1.5;
  font: 700 1.2rem 'Roboto Slab', sans-serif;
  padding: 0.75em 2em;
  letter-spacing: 0.05rem;
  margin: 1em;
  width: 13rem;
}

.btn:focus {
  outline: 2px dotted #55d7dc;
}

.draw-border2 {
    box-shadow: inset 0 0 0 4px #fc575e;
    color: #fc575e;
    -webkit-transition: color 0.25s 0.0833333333s;
    transition: color 0.25s 0.0833333333s;
    position: relative;
  }

  .draw-border2::before,
  .draw-border2::after {
    border: 0 solid transparent;
    box-sizing: border-box;
    content: '';
    pointer-events: none;
    position: absolute;
    width: 0rem;
    height: 0;
    bottom: 0;
    right: 0;
  }

  .draw-border2::before {
    border-bottom-width: 4px;
    border-left-width: 4px;
  }

  .draw-border2::after {
    border-top-width: 4px;
    border-right-width: 4px;
  }

  .draw-border2:hover {
    color: #f9484a;
  }

  .draw-border2:hover::before,
  .draw-border2:hover::after {
    border-color: #f7b42c ;
    -webkit-transition: border-color 0s, width 0.25s, height 0.25s;
    transition: border-color 0s, width 0.25s, height 0.25s;
    width: 100%;
    height: 100%;
  }

  .draw-border2:hover::before {
    -webkit-transition-delay: 0s, 0s, 0.25s;
    transition-delay: 0s, 0s, 0.25s;
  }

  .draw-border2:hover::after {
    -webkit-transition-delay: 0s, 0.25s, 0s;
    transition-delay: 0s, 0.25s, 0s;
  }
  .social-icons2 {
    padding: 0;
    list-style: none;
    margin: 1em;
  }

  .social-icons2 li {
    display: inline-block;
    margin: 0.15em;
    position: relative;
    font-size: 1em;
  }

  .social-icons2 i {
    color: #fff;
    position: absolute;
    top: 0.95em;
    left: 0.96em;
    transition: all 265ms ease-out;
  }

  .social-icons2 a {
    display: inline-block;
  }

  .social-icons2 a:before {
    transform: scale(1);
    -ms-transform: scale(1);
    -webkit-transform: scale(1);
    content: " ";
    width: 45px;
    height: 45px;
    border-radius: 100%;
    display: block;
    background: linear-gradient(145deg,#a71d31 0%, #3f0d12 74%);
    transition: all 265ms ease-out;
  }

  .social-icons2 a:hover:before {
    transform: scale(0);
    transition: all 265ms ease-in;
  }

  .social-icons2 a:hover i {
    transform: scale(2.2);
    -ms-transform: scale(2.2);
    -webkit-transform: scale(2.2);
    color: #f7b42c;
    background: -webkit-linear-gradient(315deg, #f7b42c 0%, #fc575e 74%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    transition: all 265ms ease-in;
  }

.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 20px;
  font-size: 1.2em;
}
 37  card/index.html 
@@ -0,0 +1,37 @@
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile Cards</title>
    <link rel="stylesheet" href="cssstyles\code.css">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" integrity="sha384-wvfXpqpZZVQGK6TAh5PVlGOfQNHSoD2xbE+QkPxCAFlNEevoEH3Sl0sibVcOQVnN" crossorigin="anonymous">
</head>
<body>
    <div class="container">
        <div class="card">
          <img src="circle-cropped.png" alt="Person" class="card__image2">
          <p class="card__name"><strong>Vijayakash Allenki</strong></p>
          <div class="grid-container">

            <div class="grid-child-posts">
              Posts Not yet😂
            </div>

            <div class="grid-child-followers">
              450 Followers
            </div>

          </div>
          <ul class="social-icons2">
            <li><a href="https://www.instagram.com/mrvijayakash/"><i class="fa fa-instagram"></i></a></li>
            <li><a href="https://t.me/vijayakashallenki/"><i class="fa fa-telegram"></i></a></li>
            <li><a href="https://github.com/vijayakashallenki"><i class="fa fa-github"></i></a></li>
          </ul>
          <button class="btn draw-border2">Follow</button>
          <button class="btn draw-border2">Message</button>
        </div>
    </div>
</body>
</html>
* 🌱 I’m currently learning webdevelopment 
* 🤔 I’m looking for help with Networking stuff
* 💬 Ask me about Anything
> 📫 I am intrested to collabrate with different people you can reach me: 
>> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Instagram : [@mrvijayakash](https://www.instagram.com/mrvijayakash/) 
>>
>> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;LinkedIn: [Vijayakash](https://www.linkedin.com/in/Vijayakash/) 
> 
> ⚡ Fun fact: **I am half filled.**

