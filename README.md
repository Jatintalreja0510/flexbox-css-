description - in this project we build a flebox crash course page using html and css (flexbox) where we can hover on it 
screenshot - 
![image](https://github.com/Jatintalreja0510/flexbox-css-/assets/141000419/9dcc0edb-b394-4c13-aedb-3343254f6325)

live url - [http://127.0.0.1:5500/index.html](https://deft-pixie-f35080.netlify.app)
code - 
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      rel="stylesheet"
      href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css"
      integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p"
      crossorigin="anonymous"
    />

    <link rel="stylesheet" href="style.css" />
    <title>Flexbox Crash Course</title>
  </head>

  <body>
    <nav class="navbar">
      <div class="container">
        <div class="logo">Flexbox</div>
        <ul class="nav">
          <li>
            <a href="#">Home</a>
          </li>
          <li>
            <a href="#">About</a>
          </li>
          <li>
            <a href="#">Contact</a>
          </li>
        </ul>
      </div>
    </nav>

    <header class="header">
      <div class="container">
        <div>
          <h1>Flexbox Crash Course</h1>
          <p>
            This crash course was created to help learn the basics of flexbox.
            Flexbox is a very important and useful tool in CSS.
          </p>
        </div>
        <img src="https://traversymedia.com/images/grid.svg" alt="" />
      </div>
    </header>

    <section class="boxes">
      <div class="container">
        <div class="box">
          <h2><i class="fas fa-arrows-alt-v"></i> Alignment & Space</h2>
          <p>
            A more efficient way to lay out, align and distribute space among
            items in a container
          </p>
        </div>

        <div class="box">
          <h2><i class="fas fa-arrows-alt"></i>Tricky Positioning</h2>
          <p>
            Flexbox usually solves tricky problems including how to position or
            dynamically resize elements on a page
          </p>
        </div>

        <div class="box">
          <h2><i class="fas fa-mobile"></i>Responsive Design</h2>
          <p>
            Flexbox makes building a website layout (and making it responsive!)
            much, much easier
          </p>
        </div>
      </div>
    </section>
  </body>
</html>
css code-

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: "Poppins", sans-serif;
      font-size: 16px;
      line-height: 1.5;
      color: #333;
      background: #a1c3ff;
    }

    img {
      max-width: 100%;
    }

    h1,
    h2 {
      margin-bottom: 15px;
    }

    ul {
      list-style-type: none;
    }

    .container {
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 30px;
    }

    .navbar {
      background: #3474e6;
      color: #fff;
      height: 60px;
    }

    .navbar .logo {
      font-size: x-large;
      font-weight: bold;
    }

    .navbar a {
      color: #fff;
      text-decoration: none;
      font-size: 18px;
      font-weight: bold;
    }

    .navbar a:hover {
      color: lightblue;
    }

    .navbar .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      height: 100%;
    }

    .navbar ul {
      display: flex;
    }

    .navbar ul li {
      margin-left: 20px;
    }

    .header {
      background-color: #0151cc;
      color: #fff;
      min-height: 400px;
    }

    .header h1 {
      font-size: 3rem;
      font-weight: bold;
      line-height: 1.2;
    }

    .header img {
      max-width: 400px;
    }

    .header .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .boxes .container {
      display: flex;
      justify-content: space-between;
    }

    .box {
      flex: 1;
      background: #0a51cc;
      color: #fff;
      border-radius: 10px;
      margin: 20px 10px;
      box-shadow: 0 3px 5px rgba(0, 0, 0, 0.6);
      padding: 15px 20px;
    }

    .box i {
      margin-right: 10px;
    }

    @media (max-width: 768px) {
      .header .container {
        flex-direction: column;
        padding-top: 20px;
        text-align: center;
      }

      .boxes .container {
        display: block;
        text-align: center;
      }
    }
  
