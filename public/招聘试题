<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>招聘试题</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            background: linear-gradient(180deg, #7B2FFD 0%, #3B0899 100%);
            min-height: 100vh;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            font-family: Arial, sans-serif;
        }
        p{
            padding: 20px;
            color: #fff;
        }
        .btn-container {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
            width: 80%;
            max-width: 400px;
        }
        .list-btn, .add-btn {
            width: 100%;
            height: 120px;
            padding: 20px;
            border: 2px solid #fff;
            border-radius: 8px;
            background: transparent;
            color: #fff;
            font-size: 18px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        .list-btn.active {
            background-color: #4CAF50;
            border-color: #4CAF50;
        }
        .add-btn::after {
            content: "+";
            font-size: 24px;
            margin-top: 5px;
        }
        .add-btn:hover {
            background-color: rgba(255, 255, 255, 0.1);
        }
    </style>
</head>
<body>
    <p>Button list</p>
    <div class="btn-container" id="btnContainer">
        <button class="add-btn" id="addButton">Add Button</button>
    </div>

    <script>
        const btnContainer = document.getElementById('btnContainer');
        const addButton = document.getElementById('addButton');
        let btnIndex = 1;

        addButton.addEventListener('click', () => {
            const newBtn = document.createElement('button');
            newBtn.className = 'list-btn';
            newBtn.textContent = `Button ${btnIndex}`;
            btnIndex++;

            newBtn.addEventListener('click', () => {
                newBtn.classList.toggle('active');
            });

            btnContainer.insertBefore(newBtn, addButton);
        });
    </script>
</body>
</html>
