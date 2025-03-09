<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <title>Anh có yêu em không?</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; padding: 20px; }
        #message { font-size: 18px; color: red; margin-top: 20px; }
    </style>
    <script>
        function checkAnswer() {
            var answer = document.getElementById("answer").value;
            var message = document.getElementById("message");
            
            if (answer !== "Có") {
                message.innerText = "Sai rồi! Chọn lại đi nhé!";
                return false;
            }
            message.innerText = "Đúng rồi! Nếu yêu em thì chiều nay 4h tới nhà Phanh đón em về nhé!";
            return true;
        }
    </script>
</head>
<body>
    <h2>Anh có yêu em không?</h2>
    <select id="answer">
        <option value="Không">Không</option>
        <option value="Có">Có</option>
    </select>
    <button onclick="checkAnswer()">Xác nhận</button>
    <p id="message"></p>
</body>
</html>
