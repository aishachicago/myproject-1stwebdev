myproject-1stwebdev
===================

My first web development project.
DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Non Profit Organizations</title>

        <!-- Bootstrap -->
        <link href="css/bootstrap.min.css" rel="stylesheet">

    </head>
    <body>

        <style>
            h1 {
                text-align: center;
            }

            #buttonAndText {
                margin-top:30px;
            }

        </style>
        <div class="container">
            <h1>Non Profit Organizations</h1>
            <p style="color:green;">Enter a Chicago non profit organization to find out the predominant economic organization</p>


            <div class="input-group" id="buttonAndText">
                <input type="text" class="form-control" id="textBox">
                <span class="input-group-btn">
                    <button class="btn btn-warning" type="button" id="myButton">Submit</button>
                </span>
            </div><!-- /input-group -->

        </div>
        <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
        <!-- Include all compiled plugins (below), or include individual files as needed -->
        <script src="js/bootstrap.min.js"></script>
        <script src="js/languagesChicago.js"></script>

        <script>
            $('#myButton').on('click', function () {
                var neighborhood = $('#textBox').val();
                mostSpokenNonEnglish(neighborhood);
            })
