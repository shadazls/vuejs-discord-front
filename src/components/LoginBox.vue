<template>
    <div class="container d-flex align-items-center justify-content-center">

        <div id="mainBox" class="row text-center justify-content-center">

            <h1 id="primaryText">Ha, te revoilà !</h1>
            <h2 id="secondaryText">Nous sommes si heureux de te revoir</h2>

            <form class="row justify-content-center needs-validation" novalidate>

                <div class="row">

                    <label id= "emailLabel" for="validationEmail" class="tertiarytext">E-mail
                        <p class="requiredInput">*</p>
                    </label>
                    <input id="emailInput" type="text" class="form-control inputtext" name="validationEmail" required>

                </div>

                <div class="row">

                    <label id="passwordLabel" for="validationPassword" class="tertiarytext">Mot de passe
                        <p class="requiredInput">*</p></label>
                    <input id="passwordInput" type="password" class="form-control inputtext" name="validationPassword" required>
                
                </div>

            <div>
                <button id="connectionButton" type="submit" class="btn btn-primary connectionbutton">Connexion</button>
            </div>
            
        </form>
        <label id="fourthText">Besoin d'un compte ?
            <a id="linkSignup" href="./signup.html" >S'inscrire</a>
        </label>
        </div>
    </div>
</template>

<script>    
    export default {
        name: 'LoginBox',
        props: {
            msg: String
        }
    }   
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.row > * {
    padding: 0;
}

.container{
    height: 100%;
}

#mainBox {
    border-radius: 5px;
    background-color: rgb(54, 57, 63);
    box-sizing: border-box;
    box-shadow: 0 2px 10px 0;
    width: 500px;
    height: 408px;
    padding: 32px;
}

#primaryText{
    font-family: 'Noto Sans', Helvetica, Arial, sans-serif;
    font-weight: 600; 
    font-size: 24px;
    line-height: 30px;
    color: white
}

#secondaryText{
    font-family: 'Noto Sans', Helvetica, Arial, sans-serif;
    font-weight: 400;
    font-size: 16px;
    line-height: 20px;
    margin-bottom: 8px;
    color: rgb(185, 187, 189)
}

.tertiarytext{
    font-family: 'Noto Sans', Helvetica, Arial, sans-serif;
    font-weight: 700;
    font-size: 12px;
    line-height: 16px;
    text-align: left;
    text-transform: uppercase;
    letter-spacing: .02em;
    margin-bottom: 8px;
    color: rgb(185, 187, 190)
}

.formError1{
    color: rgb(243, 134, 136);
}

.formError2{
    text-transform: none;
    font-style: italic;
    font-weight: 300;
    display: inline;
}

.requiredInput{
    display : inline;
    color: red;
}

#fourthText{
    font-family: 'Noto Sans', Helvetica, Arial, sans-serif;
    font-weight: 300;
    font-size: 14px;
    line-height: 16px;
    text-align: left;
    color: rgb(185, 187, 190)
}

.inputtext{
    background-color: rgb(32, 34, 37);
    width: 100%;
    border: none;
    padding: 10px;
    height: 40px;
    box-sizing: border-box;
    border-radius: 3px;
    font-weight: 400;
    font-size: 16px;
    margin-bottom: 20px;
    color: white;
}

.inputtext:focus{
    background-color: rgb(32, 34, 37);
    color: white;
}

.connectionbutton{
    font-size: 16px;
    line-height: 24px;
    min-width: 130px;
    min-height: 44px;
    border: none;
    border-radius: 3px;
    text-rendering: optimizeLegibility;
    font-weight: 600;
    padding: 2px 16px;
    width: 100%;
    margin-bottom: 8px;
}

#linkSignup{
    color: rgb(6, 167, 231);
    text-align: left;
    text-decoration: none;
    font-weight: 500;
    font-size: 14px;
}
</style>