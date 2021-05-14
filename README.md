# react-component-signup-login-animated-slide


A Breautiful component to display Login and signup page with sliding cards

## Demo  <br/>
[See Demo](https://guhankesav.github.io/react-component-signup-login-animated-slide/)

## Code :


### app.js
```jsx
import './App.css';

function App() {
  function login(){
    var x = document.getElementById("login");
    var y = document.getElementById("register");
    var z = document.getElementById("btn");


    x.style.left = "50px" ;
    y.style.left = "450px" ;
    z.style.left = "0px" ;
    return 0;
  }
  function register(){ 
    var x = document.getElementById("login")
    var y = document.getElementById("register")
    var z = document.getElementById("btn")


    x.style.left = "-400px" 
    y.style.left = "50px" 
    z.style.left = "110px" 
  }


  return (
    <body>
      <link rel="stylesheet" type="text/css" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.css"/>
    <div className="App">
      <div class="hero">
      <div className="form-box">
      <div className="button-box">
            <div id="btn"></div>
            <button type="button" className="toggle-btn" onClick={() => login()}>Sign In</button>
            <button type="button" className="toggle-btn" onClick={() => register()}>  Sign Up</button>

          </div>
          <form id ="login" className="input-group">
            <div className="inputwithIcon">
              <input type="text" placeholder="Mail-Id"/>
              <i  type="icon" class="fa fa-user-circle-o fa-lg fa-fw" aria-hidden="true"></i>

            </div>
            <div class="inputwithIcon">
              <input type="text" placeholder="Password"/>
              <i type="icon" className="inputwithiconii" class="fa fa-lock fa-lg fa-fw" aria-hidden="true"></i>
            </div>
            <input type="checkbox" className="check-box1"></input><span1>Forgot Password</span1>
            <button type="submit" className="submit-btn">Login</button>

          </form>
          <form id="register" className="input-group">
            <div class="inputwithIcon">
              <input type="text" placeholder="Mail-Id"/>
              <i class="fa fa-user-circle-o fa-lg fa-fw" aria-hidden="true"></i>
            </div>
            <div class="inputwithIcon">
              <input type="text" placeholder="Password"/>
              <i type="icon" class="fa fa-lock fa-lg fa-fw" aria-hidden="true"></i>
          </div>
            <div class="inputwithIcon">
              <input type="text" placeholder="Re-Password"/>
              <i type="icon" class="fa fa-key fa-lg fa-fw" aria-hidden="true"></i>
            </div>
            <input type="checkbox" className="check-box"></input><span>I agree to terms and conditions*</span>
            <button type="submit" className="submit-btn">Register</button>
          </form>

      </div>
  </div>
    </div>

  
    </body>
  );
}

export default App;

```

### facecomponent.css
```css

*{
  margin:0;
  padding:0;
  font-family: sans-serif;
}

.hero{
  height: 100%;
  width: 100%;
  background-image: linear-gradient(rgba(0,0,0,0.4),rgba(0,0,0,0.4),url(amrita1.png));
  background-position: center;
  background-size: cover;
  position: absolute;
}

.form-box{
  width:380px;
  height:480px;
  position: relative;
  margin: 6% auto;
  /* background: rgb(244, 252, 135); */
  padding: 5px;
  overflow: hidden;
  
}
.button-box{
  width: 220px;
  margin: 35px auto;
  left:0px;
  position: relative;
  box-shadow: 0 0 10px 3px #494b51;
  border-radius: 30px;
}

.toggle-btn{
  padding: 10px 30px;
  cursor:pointer;
  background: transparent;
  border:0;
  outline: none;
  position: relative;
  font-weight: bold;
  color: #ffe957;

}

#btn{
  top:0;
  left:0;
  position: absolute;
  width:110px;
  height:100%;
  background-color: #494b51;
  border-radius: 30px;
  transition: .5s;
}
.social-icons {
  margin: 30px auto;
  text-align: center;
}
.social-icons img{
  height: 50px;
  width: 50px;
  margin: 30px auto;
  text-align: 0 12px;
  box-shadow: 0 0 20px 0 #7f7f7f3d;
  cursor: pointer;
  border-radius: 50%;
}
.input-group{
  top: 180px;
  position: absolute;
  width: 280px;
  transition: .5s;
}
.input-field{
  width: 100%;
  padding: 10px 0;
  margin: 5px 0;
  border-left: 2px solid rgb(82, 82, 82);
  border-top: 2px solid rgb(82, 82, 82);
  border-right:2px solid rgb(82, 82, 82);
  border-bottom: 2px solid rgb(82, 82, 82);
  border-color: dimgray;
  border-width: 3px;
  background: transparent;
  border-radius: 6px;
  
}
.submit-btn{
  width: 85%;
  padding: 10px 30px;
  cursor: pointer;
  display: block;
  margin: auto;
  top :5px;
  background-color: #ffe957;
  color:#494b51;
  font-weight: bold;

  border:0;
  outline: none;
  border-radius: 30px;
}
.check-box{
  margin: 30px 10px 30p 0;
  

}
.check-box1{
  margin: 30px 10px 30p 0;
  visibility: hidden;

}
span{
  color:#777;
  font-size: 12px;
  bottom:38px;
  left: 20px;
  position: absolute;
}
span1{
  text-emphasis-style: initial;
  text-decoration: underline;
  left: 180px;
  top:10;
  cursor: pointer;
  color:rgb(77, 76, 76);
  font-size: 11px;
  bottom:40px;
  /* bottom:68px; */
  position: absolute;
}

#login{
  left: 50px;
}
#register{
  left: 450px;
}

input[type="text"] {
  width: 100%;
  border: 2px solid rgb(104, 103, 103);
  border-radius: 4px;
  margin: 8px 0;
  outline: none;
  padding: 8px;
  box-sizing: border-box;
  transition: 0.3s;


}

input[type="text"]:focus {
  border-color: #f5a80eda;
  box-shadow: 0 0 8px 0 #f5a80eda;
}

.inputwithIcon input[type="text"] {
  padding-left: 40px;
}

.inputwithIcon {
  position: relative;
}

.inputwithIcon i{
  position: absolute;
  left: 0;
  top: 8px;
  padding: 9px 8px;
  color: rgb(104, 103, 103);
  transition: 0.3s;
}

.inputwithIcon input[type="text"]:focus + i {
  color: #f5a80eda;
}
```
## To install gh-pages<br/>
 npm install --save gh-pages<br/>
## To be added in package.json
  <li>"homepage":"http://guhankesav.github.io/react-face-component-test"<br/>
    <li>"scripts": {<br/>
    "predeploy":"npm run build",<br/>
    "deploy":"gh-pages -d build",<br/>
  },<br/>
   <li>"devDependencies": {<br/>
    "gh-pages": "^3.1.0"<br/>
  }<br/>
  
## Commands :<br/>
git init<br/>
git remote add origin https: <br/>
git status<br/>
git add .<br/>
git commit -m "ini commiy"<br/>
npm run deploy<br/>
git push -u origin master<br/>

## In case of origin prob :<br/>
git remote rm origin

