<!DOCTYPE html>
<!--=== Coding by CodingLab | www.codinglabweb.com === -->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!----======== CSS ======== -->
    <link rel="stylesheet" href="specificdetails.css">
     
    <!----===== Iconscout CSS ===== -->
    <link rel="stylesheet" href="https://unicons.iconscout.com/release/v4.0.0/css/line.css">

    <!--<title>Responsive Regisration Form </title>--> 
</head>
<body>
    <div class="container">
        <header>SPECIFIC DETAILS</header>

        <form action="#">
            <div class="form first">
                <div class="details personal">
                    <span class="title"></span>

                    <div class="fields">
                        <div class="input-field">
                            <label>Differently Abled</label>
                            <select required>
                                <option disabled selected>Select differently abled</option>
                                <option>Yes</option>
                                <option>No</option>
                            </select>
                           
                        </div>
                        
                 
                            <div class="input-field">
                            <label>special category</label>
                            <select required>
                                <option disabled selected>Special category</option>
                                <option>Orphan</option>
                                <option>Semi-Orphan</option>
                            </select>

                        </div>

                        <div class="input-field">
                            <label>Ex-Serviceman</label>
                            <select required>
                                <option disabled selected>Special category</option>
                                <option>Yes</option>
                                <option>No</option>
                            </select>
                        </div>

                        <div class="input-field">
                            <label>First Generation Learner</label>
                            <select required>
                                <option disabled selected>First Generation Learner</option>
                                <option>Yes</option>
                                <option>No</option>
                            </select>
                        </div>

                        <div class="input-field">
                            <label>Sports Quota</label>
                            <select required>
                                <option disabled selected>Sports Quota</option>
                                <option>Yes</option>
                                <option>No</option>
                            </select>
                        </div>

                        <button class="BackBtn">
                            <span class="btnText">Back</span>
                            <i class="uil uil-navigator"></i>
                        </button>

                <button class="SaveBtn">
                    <span class="btnText">SAVE</span>
                    <i class="uil uil-navigator"></i>
                </button>
            
                <button class="nextBtn">
                    <span class="btnText">Next</span>
                    <i class="uil uil-navigator"></i>
                </button>
            </div> 
        </div>
                                    
<!--<script src="script.js"></script>-->
</body>
</html>








SPECIFIC DETAILS CSS




/* ===== Google Font Import - Poppins ===== */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
body{
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(to top, rgba(77, 51, 77, 0.5)100%,rgba(13, 15, 14, 0.5)50%), url('./unom bg.jpg');
    background-size: cover;
}
.container{
    position: relative;
    max-width: 900px;
    width: 100%;
    border-radius: 6px;
    padding: 30px;
    margin: 0 15px;
    background-color: #fff;
    box-shadow: 0 5px 10px rgba(0,0,0,0.1);
}
.container header{
    position: relative;
    font-size: 20px;
    font-weight: 600;
    color: #333;
}
.container header::before{
    content: "";
    position: absolute;
    left: 0;
    bottom: -2px;
    height: 3px;
    width: 27px;
    border-radius: 8px;
    background-color: unom bg jpg ;
}
.container form{
    position: relative;
    margin-top: 16px;
    min-height: 490px;
    background-color: #fff;
    overflow: hidden;
}
.container form .form{
    position: absolute;
    background-color: #fff;
    transition: 0.3s ease;
}
.container form .form.second{
    opacity: 0;
    pointer-events: none;
    transform: translateX(100%);
}
form.secActive .form.second{
    opacity: 1;
    pointer-events: auto;
    transform: translateX(0);
}
form.secActive .form.first{
    opacity: 0;
    pointer-events: none;
    transform: translateX(-100%);
}
.container form .title{
    display: block;
    margin-bottom: 8px;
    font-size: 16px;
    font-weight: 500;
    margin: 6px 0;
    color: #333;
}
.container form .fields{
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}
form .fields .input-field{
    display: flex;
    width: calc(100% / 3 - 15px);
    flex-direction: column;
    margin: 4px 0;
}
.input-field label{
    font-size: 12px;
    font-weight: 500;
    color: #2e2e2e;
}
.input-field input, select{
    outline: none;
    font-size: 14px;
    font-weight: 400;
    color: #333;
    border-radius: 5px;
    border: 1px solid #aaa;
    padding: 0 15px;
    height: 42px;
    margin: 8px 0;
}
.input-field input :focus,
.input-field select:focus{
    box-shadow: 0 3px 6px rgba(0,0,0,0.13);
}
.input-field select,
.input-field input[type="date"]{
    color: #707070;
}
.input-field input[type="date"]:valid{
    color: #333;
}
.container form button, .backBtn{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 45px;
    max-width: 200px;
    width: 100%;
    border: none;
    outline: none;
    color: rgb(14, 14, 14);
    border-radius: 5px;
    margin: 25px 0;
    background-color:rgb(108, 105, 105)(223, 220, 255);
    transition: all 0.3s linear;
    cursor: pointer;
}
.container form .btnText{
    font-size: 14px;
    font-weight: 400;
}
form button:hover{
    background-color:rgb(209, 171, 119);
}
form button i,
form .backBtn i{
    margin: 0.7px;
}
form .backBtn i{
    transform: rotate(180deg);
}
form .buttons{
    display: flex;
    align-items: absolute;
}
form .buttons button , .backBtn{
    margin-right: 50px;
}

@media (max-width: 750px) {
    .container form{
        overflow-y: scroll;
    }
    .container form::-webkit-scrollbar{
       display: none;
    }
    form .fields .input-field{
        width: calc(100% / 2 - 15px);
    }
}

@media (max-width: 550px) {
    form .fields .input-field{
        width: 100%;
    }
}

