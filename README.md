<!DOCTYPE html>
     
<html>
<body>
<head>
  <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chatbot AI</title>

    
    <h1>Chatbot AI</h1>
    <div id="chatbox">
        <div id="messages"></div>
    </div>
    <input type="text" id="userInput" placeholder="Digite sua mensagem...">
    <button onclick="sendMessage()">Enviar</button>
  
    <script>
        function sendMessage() {
            const userInput = document.getElementById('userInput').value;
            const messages = document.getElementById('messages');
            messages.innerHTML += `<div>Você: ${userInput}`;
            document.getElementById('userInput').value = '';
            // Aqui você chamaria sua lógica de AI
            const aiResponse = "olá"; // Substitua por sua lógica
             const aiResponde = "tudo bem";
          messages.innerHTML += `
          
AI: ${aiResponse}
AI: ${aiResponde}</div>`;} 
        
    </script>
     <style>
        body {
            font-family: Arial, sans-serif;
        }
        {
            border: 1px solid #ccc;
            padding: 10px;
            width: 300px;
            height: 400px;
            overflow-y: scroll;
        }
        #userInput {
            width: 240px;
        }
    </style>
</body>
</html>

