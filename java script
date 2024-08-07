document.addEventListener('DOMContentLoaded', () => {
    const ensaButton = document.getElementById('ensa-btn');
    const options = document.getElementById('options');
    const quizContainer = document.getElementById('quiz-container');
    const submitButton = document.getElementById('submit-btn');
    const scoreContainer = document.getElementById('score');
    const timerElement = document.getElementById('timer-count');
    
    let timer;
    let currentQuiz;

    ensaButton.addEventListener('click', () => {
        options.classList.remove('hidden');
    });

    document.querySelectorAll('.option-btn').forEach(button => {
        button.addEventListener('click', () => {
            const type = button.getAttribute('data-type');
            currentQuiz = type;
            loadQuiz(type);
        });
    });

    function loadQuiz(type) {
        quizContainer.classList.remove('hidden');
        document.getElementById('options').classList.add('hidden');
        if (type === 'maths') {
            loadImages([
                'https://scontent.fcmn2-1.fna.fbcdn.net/v/t39.30808-6/453005822_503996065487809_7270909177636529631_n.jpg',
                'https://scontent.fcmn3-1.fna.fbcdn.net/v/t39.30808-6/453059806_503996108821138_7779194545139845968_n.jpg',
                'https://scontent.fcmn3-1.fna.fbcdn.net/v/t39.30808-6/453168015_503996195487796_7953178559514120609_n.jpg',
                'https://scontent.fcmn3-2.fna.fbcdn.net/v/t39.30808-6/453038163_503996235487792_3980965127081529082_n.jpg'
            ]);
            loadQuestions([
                { question: 'Question 1', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 2', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 3', answers: ['A', 'B', 'C', 'D'], correct: 'D' },
                { question: 'Question 4', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 5', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 6', answers: ['A', 'B', 'C', 'D'], correct: 'D' },
                { question: 'Question 7', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 8', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 9', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 10', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 11', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 12', answers: ['A', 'B', 'C', 'D'], correct: 'D' },
                { question: 'Question 13', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 14', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 15', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 16', answers: ['A', 'B', 'C', 'D'], correct: 'D' },
                { question: 'Question 17', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 18', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 19', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 20', answers: ['A', 'B', 'C', 'D'], correct: 'B' }
            ]);
        } else if (type === 'pc') {
            loadImages([
                'https://scontent.fcmn2-1.fna.fbcdn.net/v/t39.30808-6/453072992_503996292154453_4979698021201570870_n.jpg',
                'https://scontent.fcmn3-1.fna.fbcdn.net/v/t39.30808-6/453092583_503996355487780_1736659329333461992_n.jpg',
                'https://scontent.fcmn3-2.fna.fbcdn.net/v/t39.30808-6/453148112_503996392154443_6420239165576951411_n.jpg',
                'https://scontent.fcmn2-2.fna.fbcdn.net/v/t39.30808-6/453060917_503996418821107_451627619982632372_n.jpg'
            ]);
            loadQuestions([
                { question: 'Question 1', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 2', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 3', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 4', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 5', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 6', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 7', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 8', answers: ['A', 'B', 'C', 'D'], correct: 'D' },
                { question: 'Question 9', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 10', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 11', answers: ['A', 'B', 'C', 'D'], correct: 'D' },
                { question: 'Question 12', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 13', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 14', answers: ['A', 'B', 'C', 'D'], correct: 'D' },
                { question: 'Question 15', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 16', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 17', answers: ['A', 'B', 'C', 'D'], correct: 'B' },
                { question: 'Question 18', answers: ['A', 'B', 'C', 'D'], correct: 'C' },
                { question: 'Question 19', answers: ['A', 'B', 'C', 'D'], correct: 'A' },
                { question: 'Question 20', answers: ['A', 'B', 'C', 'D'], correct: 'A' }
            ]);
        }
        startTimer();
    }

    function loadImages(urls) {
        const container = document.getElementById('image-container');
        container.innerHTML = '';
        urls.forEach(url => {
            const img = document.createElement('img');
            img.src = url;
            container.appendChild(img);
        });
    }

    function loadQuestions(questions) {
        const form = document.getElementById('quiz-form');
        form.innerHTML = '';
        questions.forEach((question, index) => {
            const questionElem = document.createElement('div');
            questionElem.classList.add('question');
            questionElem.innerHTML = `
                <p>${question.question}</p>
                <label><input type="radio" name="q${index}" value="A"> A</label>
                <label><input type="radio" name="q${index}" value="B"> B</label>
                <label><input type="radio" name="q${index}" value="C"> C</label>
                <label><input type="radio" name="q${index}" value="D"> D</label>
            `;
            form.appendChild(questionElem);
        });
    }

    function startTimer() {
        let time = 90 * 60; // 90 minutes
        timer = setInterval(() => {
            const minutes = Math.floor(time / 60);
            const seconds = time % 60;
            timerElement.textContent = `${String(minutes).padStart(2, '0')}:${String(seconds).padStart(2, '0')}`;
            time--;
            if (time < 0) {
                clearInterval(timer);
                submitQuiz();
            }
        }, 1000);
    }

    document.getElementById('quiz-form').addEventListener('submit', (event) => {
        event.preventDefault();
        submitQuiz();
    });

    function submitQuiz() {
        clearInterval(timer);

        // Calculate score
        let score = 0;
        const formData = new FormData(document.getElementById('quiz-form'));
        const answers = Array.from(formData.entries()).map(entry => entry[1]);
        const correctAnswers = currentQuiz === 'maths'
            ? ['A', 'A', 'D', 'B', 'C', 'D', 'A', 'C', 'A', 'C', 'B', 'D', 'C', 'A', 'B', 'D', 'C', 'A', 'A', 'B']
            : ['A', 'B', 'B', 'B', 'B', 'C', 'B', 'D', 'A', 'A', 'D', 'C', 'C', 'D', 'A', 'A', 'B', 'C', 'A', 'A'];

        answers.forEach((answer, index) => {
            if (answer === correctAnswers[index]) {
                score += 2;
            } else if (answer) {
                score -= 1;
            }
        });

        // Display score
        scoreContainer.classList.remove('hidden');
        scoreContainer.textContent = `You got ${score}/40 points!`;
    }
});
