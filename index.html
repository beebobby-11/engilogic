<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thai Alphabet Drill - Streak Edition</title>
    <style>
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; display: flex; justify-content: center; align-items: center; height: 100vh; margin: 0; background-color: #f7f9fc; }
        .card { background: white; padding: 30px; border-radius: 16px; box-shadow: 0 8px 24px rgba(0,0,0,0.1); text-align: center; width: 350px; border: 2px solid #e5e7eb; }
        #welcome-screen input { width: 100%; padding: 12px; margin: 15px 0; border: 2px solid #e5e7eb; border-radius: 8px; box-sizing: border-box; font-size: 16px; }
        .btn-start { background-color: #58cc02; color: white; border: none; padding: 14px; border-radius: 12px; cursor: pointer; font-size: 16px; font-weight: bold; width: 100%; text-transform: uppercase; border-bottom: 4px solid #46a302; }
        .btn-start:active { border-bottom: 0; margin-top: 4px; }
        .hidden { display: none; }
        .streak-badge { display: inline-block; background: #ff9600; color: white; padding: 4px 12px; border-radius: 20px; font-weight: bold; font-size: 14px; margin-bottom: 10px; }
        .hearts { color: #ff4b4b; font-size: 24px; margin: 10px 0; }
        .consonant-display { font-size: 90px; margin: 20px 0; color: #3c3c3c; }
        .option-btn { display: block; width: 100%; padding: 12px; margin: 8px 0; background: white; border: 2px solid #e5e7eb; border-radius: 12px; cursor: pointer; font-size: 16px; transition: all 0.2s; border-bottom: 4px solid #e5e7eb; }
        .option-btn:hover { background: #f1f4f6; }
        .option-btn:active { border-bottom: 0; transform: translateY(2px); }
    </style>
</head>
<body>

    <div id="welcome-screen" class="card">
        <div id="streak-display" class="streak-badge">Streak: 0 🔥</div>
        <h2 style="margin-top:10px;">CSII Team X</h2>
        <p>Thai Alphabet Mastery</p>
        <input type="text" id="nickname-input" placeholder="Enter Nickname">
        <button class="btn-start" onclick="startQuiz()">Start Quiz</button>
    </div>

    <div id="quiz-screen" class="card hidden">
        <div id="user-header" style="font-weight: bold; color: #4b4b4b;"></div>
        <div class="hearts">❤️❤️❤️</div>
        <div id="remaining-count" style="font-size: 13px; color: #afafaf;">Remaining: 44</div>
        <h3 style="margin: 15px 0 5px 0;">Thai Consonant Drill</h3>
        <div id="char-display" class="consonant-display">ก</div>
        <div id="options-container">
            </div>
    </div>

    <script>
        const thaiConsonants = [
            {char: 'ก', name: 'kor kai', class: 'Middle'}, {char: 'ข', name: 'khor khai', class: 'High'},
            {char: 'ค', name: 'khor khwai', class: 'Low'}, {char: 'ง', name: 'ngor ngu', class: 'Low'},
            {char: 'จ', name: 'jor jan', class: 'Middle'}, {char: 'ฉ', name: 'chor ching', class: 'High'},
            {char: 'ช', name: 'chor chang', class: 'Low'}, {char: 'ซ', name: 'sor so', class: 'Low'},
            {char: 'ย', name: 'yor yak', class: 'Low'}, {char: 'ร', name: 'ror ruea', class: 'Low'}
            // ... (Add all 44 here)
        ];

        let quizSequence = [];

        // Load Streak on page load
        window.onload = () => {
            const streak = localStorage.getItem('userStreak') || 0;
            document.getElementById('streak-display').innerText = `Streak: ${streak} 🔥`;
        };

        function shuffle(array) {
            for (let i = array.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [array[i], array[j]] = [array[j], array[i]];
            }
            return array;
        }

        function startQuiz() {
            const nickname = document.getElementById('nickname-input').value;
            if (!nickname.trim()) return alert("Enter a name!");

            // 1. Increment Streak
            let currentStreak = parseInt(localStorage.getItem('userStreak') || 0);
            currentStreak++;
            localStorage.setItem('userStreak', currentStreak);

            // 2. Prepare Data
            quizSequence = shuffle([...thaiConsonants]);
            
            // 3. UI Transition
            document.getElementById('user-header').innerText = nickname;
            document.getElementById('welcome-screen').classList.add('hidden');
            document.getElementById('quiz-screen').classList.remove('hidden');
            
            loadQuestion();
        }

        function loadQuestion() {
            if (quizSequence.length === 0) {
                alert("Course Complete!");
                location.reload();
                return;
            }

            const current = quizSequence[0];
            document.getElementById('char-display').innerText = current.char;
            document.getElementById('remaining-count').innerText = `Remaining: ${quizSequence.length}`;

            // Generate 3 random options including the correct one
            const container = document.getElementById('options-container');
            container.innerHTML = '';
            
            let choices = [current];
            while(choices.length < 3) {
                let randomChar = thaiConsonants[Math.floor(Math.random() * thaiConsonants.length)];
                if(!choices.includes(randomChar)) choices.push(randomChar);
            }
            
            shuffle(choices).forEach(choice => {
                const btn = document.createElement('button');
                btn.className = 'option-btn';
                btn.innerText = `${choice.name} — ${choice.class}`;
                btn.onclick = () => handleAnswer(choice === current);
                container.appendChild(btn);
            });
        }

        function handleAnswer(isCorrect) {
            if (isCorrect) {
                quizSequence.shift();
                loadQuestion();
            } else {
                alert("Try again!");
            }
        }
    </script>
</body>
</html>
