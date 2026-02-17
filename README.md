<!DOCTYPE html>
<html>
<head>
    <title>India Quiz</title>
    <style>
        body { font-family: Arial; max-width: 600px; margin: 50px auto; padding: 20px; background: #fff3cd; }
        h1 { color: #dc3545; text-align: center; }
        h2 { color: #856404; }
        label { display: block; margin: 10px 0; padding: 10px; background: white; border-radius: 8px; }
        button { background: #dc3545; color: white; padding: 12px 24px; border: none; border-radius: 6px; font-size: 16px; }
        .result { font-size: 20px; font-weight: bold; margin-top: 20px; }
    </style>
</head>
<body>
    <h1>🇮🇳 India Quiz</h1>
    
    <h2>What is the national animal of India?</h2>
    <form>
        <label><input type="radio" name="q1" value="1"> 1. Tiger</label>
        <label><input type="radio" name="q1" value="2"> 2. Lion</label>
        <label><input type="radio" name="q1" value="3"> 3. Elephant</label>
        <label><input type="radio" name="q1" value="4"> 4. Peacock</label>
        <label><input type="radio" name="q1" value="5"> 5. Bear</label>
        <button type="submit">Submit</button>
        <div class="result" id="result"></div>
    </form>

    <p style="margin-top: 30px; font-size: 14px;">
        More questions: National bird = Peacock, National flower = Lotus
    </p>

    <script>
    document.querySelector('form').addEventListener('submit', function(e) {
        e.preventDefault();
        if(document.querySelector('input[value="1"]').checked) {
            document.getElementById('result').innerHTML = '✅ Correct! Tiger is the national animal!';
            document.getElementById('result').style.color = 'green';
        } else {
            document.getElementById('result').innerHTML = '❌ Wrong! It\'s Tiger!';
            document.getElementById('result').style.color = 'red';
        }
    });
    </script>
</body>
</html>
