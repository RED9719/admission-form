# admission-form
Design an admission form for any course in your college with text, password fields, drop-down 
list, check-boxes, and radio buttons, submit and reset button etc. with proper CSS formatting. 
CODE
           <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>College Admission Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            margin: 0;
            padding: 0;
        }
        .container {
            max-width: 600px;
            margin: 50px auto;
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h2 {
            text-align: center;
            margin-bottom: 20px;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
        }
        input[type="text"],
        input[type="password"],
        select,
        textarea {
            width: 100%;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }
        input[type="checkbox"],
        input[type="radio"] {
            margin-right: 10px;
        }
        
        button {
            padding: 10px 15px;
            background-color: #007bff;
            border: none;
            border-radius: 5px;
            color: #fff;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>College Admission Form</h2>
        <form action="#" method="post">
            <div class="form-group">
                <label for="full-name">Full Name:</label>
                <input type="text" id="full-name" name="full-name" required>
            </div>
            <div class="form-group">
                <label for="email">Email:</label>
                <input type="text" id="email" name="email" required>
            </div>
            <div class="form-group">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" required>
            </div>
            <div class="form-group">
                <label for="course">Course:</label>
                <select id="course" name="course">
                    <option value="bsc">B.Sc</option>
                    <option value="bcom">B.Com</option>
                    <option value="ba">B.A</option>
                    <option value="mca">MCA</option>
                    <option value="mba">MBA</option>
                </select>
            </div>
            <div class="form-group">
                <label>Gender:</label>
                <input type="radio" id="male" name="gender" value="male">
                <label for="male">Male</label>
                <input type="radio" id="female" name="gender" value="female">
                <label for="female">Female</label>
                <input type="radio" id="other" name="gender" value="other">
                <label for="other">Other</label>
            </div>
            <div class="form-group">
                <label>Interests:</label>
                <input type="checkbox" id="sports" name="interests" value="sports">
                <label for="sports">Sports</label>
                <input type="checkbox" id="music" name="interests" value="music">
                <label for="music">Music</label>
                <input type="checkbox" id="reading" name="interests" value="reading">
                <label for="reading">Reading</label>
            </div>
            <div class="form-buttons">
                <button type="submit">Submit</button>
                <button type="reset" class="reset">Reset</button>
            </div>
        </form>
    </div>
</body>
</html>
