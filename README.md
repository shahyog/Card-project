<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Card project</title>

        <style>
        body{
            background-color: white;
            justify-content: center;
            align-items: center;
            height: 690px;
            margin-top: 200px;
            margin-left:30%;
        }
        .cardno{
            height: 300px;
            width: 50%;
            color: white;
            border: 2px solid black;
            border-radius: 20px;
            padding: 20px;
            line-height: 25px;
            font-size: 20px;
            background-color:indigo;

            
        }
        .card{
            /* background-color: red; */
            float: right;
            height: 50px;
            width:90px;
            margin-top: 20px;
        }
        .cardno input
        {
            font-size: xx-large;
        }

        img{
            height: inherit;
            width: inherit;
        }
        .card img
        {
            height: 120px;
            width: 100%;
        }
        .cardno input:nth-of-type("date")
        {
            background-color: brown;
        }

    </style>    
</head>
<body>

    <div class="cardno">
    card number <br>
    <input type="text" id="num" maxlength="4" onkeyup="reference()" required>
    <br>
    <br>
    Expiry date
    <br>
    <input type="date"><br>
    
    
    <div class="card">
        <img id="cardtype" src="image/White_full.jpeg" alt="" >
   
    </div>

    </div>
    <script>
        function reference(){
            a=document.getElementById('num').value
            if(a[0]=="0")
            {
                document.getElementById('cardtype').src="image/visa.png";
            }
            else if(a[0]=='4')
            {
                document.getElementById('cardtype').src="image/master card.jpeg";
            }
            else if(a[0]=='5')
            {
                document.getElementById('cardtype').src="image/RUPAY.JPEG";
            }
            else if(a[0]=='6')
            {
                document.getElementById('cardtype').src="image/american.jpeg";
            }
            else{
                document.getElementById('cardtype').src="image/not expext.jpeg";
            }
        }
    </script>
    <div style="font-size: xx-large; color: red; display: flex;">
        <h1>
                check card no 
        </h1>
        <input type="submit" name="" id="" style="height: 60px; margin-top: 50px; margin-left: 15%; width: 30%;color:white; font-size: xx-large; background-color: red; border-radius: 15px; border: none;">
    </div> 
</body>
</html>
