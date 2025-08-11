<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GK Master - 1000+ General Knowledge Questions</title>
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #2ecc71;
            --dark-color: #2c3e50;
            --light-color: #ecf0f1;
            --danger-color: #e74c3c;
            --warning-color: #f39c12;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 1rem 0;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            display: flex;
            align-items: center;
        }
        
        .logo i {
            margin-right: 10px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 20px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 5px 10px;
            border-radius: 4px;
        }
        
        nav ul li a:hover {
            background-color: rgba(255, 255, 255, 0.2);
        }
        
        .hero {
            background: url('https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80') no-repeat center center/cover;
            height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            position: relative;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.6);
        }
        
        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 800px;
            padding: 0 20px;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            text-decoration: none;
            font-size: 1rem;
            transition: all 0.3s ease;
        }
        
        .btn:hover {
            background-color: #2980b9;
            transform: translateY(-2px);
        }
        
        .btn-secondary {
            background-color: var(--secondary-color);
        }
        
        .btn-secondary:hover {
            background-color: #27ae60;
        }
        
        .main-content {
            padding: 40px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: var(--dark-color);
        }
        
        .section-title h2 {
            font-size: 2rem;
            position: relative;
            display: inline-block;
            padding-bottom: 10px;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
        }
        
        .search-container {
            display: flex;
            margin-bottom: 30px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            border-radius: 4px;
            overflow: hidden;
        }
        
        .search-container input {
            flex: 1;
            padding: 12px 20px;
            border: none;
            font-size: 1rem;
        }
        
        .search-container button {
            padding: 0 20px;
            background-color: var(--primary-color);
            color: white;
            border: none;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .search-container button:hover {
            background-color: #2980b9;
        }
        
        .category-filter {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            margin-bottom: 30px;
            gap: 10px;
        }
        
        .category-btn {
            padding: 8px 16px;
            background-color: white;
            border: 1px solid #ddd;
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .category-btn:hover, .category-btn.active {
            background-color: var(--primary-color);
            color: white;
            border-color: var(--primary-color);
        }
        
        .questions-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 20px;
        }
        
        .question-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }
        
        .question-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
        }
        
        .question-header {
            background-color: var(--dark-color);
            color: white;
            padding: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .question-category {
            background-color: var(--secondary-color);
            color: white;
            padding: 3px 10px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: bold;
        }
        
        .question-body {
            padding: 20px;
        }
        
        .question-text {
            font-size: 1.1rem;
            margin-bottom: 15px;
        }
        
        .show-answer-btn {
            background-color: transparent;
            color: var(--primary-color);
            border: 1px solid var(--primary-color);
            padding: 5px 10px;
            border-radius: 4px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .show-answer-btn:hover {
            background-color: var(--primary-color);
            color: white;
        }
        
        .answer-text {
            margin-top: 15px;
            padding: 15px;
            background-color: #f8f9fa;
            border-radius: 4px;
            display: none;
        }
        
        .add-question-form {
            background-color: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            max-width: 800px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        
        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 1rem;
        }
        
        .form-group textarea {
            min-height: 100px;
            resize: vertical;
        }
        
        .pagination {
            display: flex;
            justify-content: center;
            margin-top: 40px;
        }
        
        .pagination button {
            padding: 8px 16px;
            margin: 0 5px;
            background-color: white;
            border: 1px solid #ddd;
            border-radius: 4px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .pagination button.active {
            background-color: var(--primary-color);
            color: white;
            border-color: var(--primary-color);
        }
        
        .pagination button:hover:not(.active) {
            background-color: #f1f1f1;
        }
        
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 40px 0 20px;
            text-align: center;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }
        
        .footer-section {
            flex: 1;
            min-width: 250px;
            margin-bottom: 20px;
            padding: 0 20px;
        }
        
        .footer-section h3 {
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-section h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 2px;
            background-color: var(--primary-color);
        }
        
        .footer-section p, .footer-section a {
            color: #bbb;
            margin-bottom: 10px;
            display: block;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .footer-section a:hover {
            color: white;
            padding-left: 5px;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 15px;
        }
        
        .social-links a {
            color: white;
            background-color: rgba(255, 255, 255, 0.1);
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        
        .social-links a:hover {
            background-color: var(--primary-color);
            transform: translateY(-3px);
        }
        
        .copyright {
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            color: #bbb;
        }
        
        /* Modal styles */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            z-index: 1000;
            justify-content: center;
            align-items: center;
        }
        
        .modal-content {
            background-color: white;
            padding: 30px;
            border-radius: 8px;
            max-width: 500px;
            width: 90%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
        }
        
        .close-modal {
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 1.5rem;
            cursor: pointer;
            color: #777;
            transition: all 0.3s ease;
        }
        
        .close-modal:hover {
            color: var(--danger-color);
            transform: rotate(90deg);
        }
        
        /* Responsive styles */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 15px;
                justify-content: center;
            }
            
            nav ul li {
                margin: 0 10px;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .questions-container {
                grid-template-columns: 1fr;
            }
            
            .footer-content {
                flex-direction: column;
                align-items: center;
                text-align: center;
            }
            
            .footer-section h3::after {
                left: 50%;
                transform: translateX(-50%);
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <header>
        <div class="container header-content">
            <div class="logo">
                <i class="fas fa-brain"></i>
                GK Master
            </div>
            <nav>
                <ul>
                    <li><a href="#" class="active">Home</a></li>
                    <li><a href="#questions">Questions</a></li>
                    <li><a href="#add-question">Add Question</a></li>
                    <li><a href="#categories">Categories</a></li>
                    <li><a href="#about">About</a></li>
                </ul>
            </nav>
        </div>
    </header>
    
    <section class="hero">
        <div class="hero-content">
            <h1>1000+ General Knowledge Questions</h1>
            <p>Test your knowledge with our extensive collection of GK questions across various categories</p>
            <a href="#questions" class="btn btn-secondary">Explore Questions</a>
        </div>
    </section>
    
    <section class="main-content">
        <div class="container">
            <section id="questions">
                <div class="section-title">
                    <h2>General Knowledge Questions</h2>
                </div>
                
                <div class="search-container">
                    <input type="text" id="search-input" placeholder="Search questions...">
                    <button id="search-btn"><i class="fas fa-search"></i></button>
                </div>
                
                <div class="category-filter" id="category-filter">
                    <button class="category-btn active" data-category="all">All</button>
                    <button class="category-btn" data-category="history">History</button>
                    <button class="category-btn" data-category="science">Science</button>
                    <button class="category-btn" data-category="geography">Geography</button>
                    <button class="category-btn" data-category="sports">Sports</button>
                    <button class="category-btn" data-category="arts">Arts</button>
                    <button class="category-btn" data-category="politics">Politics</button>
                    <button class="category-btn" data-category="technology">Technology</button>
                </div>
                
                <div class="questions-container" id="questions-container">
                    <!-- Questions will be loaded here -->
                </div>
                
                <div class="pagination" id="pagination">
                    <!-- Pagination will be loaded here -->
                </div>
            </section>
            
            <section id="add-question" style="margin-top: 80px;">
                <div class="section-title">
                    <h2>Add New Question</h2>
                </div>
                
                <div class="add-question-form">
                    <form id="question-form">
                        <div class="form-group">
                            <label for="question">Question</label>
                            <input type="text" id="question" required placeholder="Enter your question">
                        </div>
                        
                        <div class="form-group">
                            <label for="answer">Answer</label>
                            <textarea id="answer" required placeholder="Enter the answer"></textarea>
                        </div>
                        
                        <div class="form-group">
                            <label for="category">Category</label>
                            <select id="category" required>
                                <option value="">Select a category</option>
                                <option value="history">History</option>
                                <option value="science">Science</option>
                                <option value="geography">Geography</option>
                                <option value="sports">Sports</option>
                                <option value="arts">Arts</option>
                                <option value="politics">Politics</option>
                                <option value="technology">Technology</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                        
                        <div class="form-group">
                            <label for="difficulty">Difficulty</label>
                            <select id="difficulty" required>
                                <option value="easy">Easy</option>
                                <option value="medium">Medium</option>
                                <option value="hard">Hard</option>
                            </select>
                        </div>
                        
                        <button type="submit" class="btn btn-secondary">Add Question</button>
                    </form>
                </div>
            </section>
        </div>
    </section>
    
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>About GK Master</h3>
                    <p>GK Master is a comprehensive platform for general knowledge enthusiasts with 1000+ questions across various categories.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
                
                <div class="footer-section">
                    <h3>Quick Links</h3>
                    <a href="#questions">Questions</a>
                    <a href="#add-question">Add Question</a>
                    <a href="#categories">Categories</a>
                    <a href="#about">About Us</a>
                </div>
                
                <div class="footer-section">
                    <h3>Contact Us</h3>
                    <p><i class="fas fa-envelope"></i> info@gkmaster.com</p>
                    <p><i class="fas fa-phone"></i> +1 (123) 456-7890</p>
                    <p><i class="fas fa-map-marker-alt"></i> 123 GK Street, Knowledge City</p>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 GK Master. All Rights Reserved.</p>
            </div>
        </div>
    </footer>
    
    <!-- Question Modal -->
    <div class="modal" id="question-modal">
        <div class="modal-content">
            <span class="close-modal">&times;</span>
            <div class="question-header">
                <span id="modal-category" class="question-category">History</span>
                <span id="modal-difficulty" class="question-difficulty">Medium</span>
            </div>
            <div class="question-body">
                <p class="question-text" id="modal-question">What is the capital of France?</p>
                <button class="show-answer-btn" id="modal-show-answer">Show Answer</button>
                <div class="answer-text" id="modal-answer">The capital of France is Paris.</div>
            </div>
        </div>
    </div>
    
    <script>
        // Sample questions data (in a real app, this would come from a database)
        const questions = [
            {
                id: 1,
                question: "What is the capital of France?",
                answer: "The capital of France is Paris.",
                category: "geography",
                difficulty: "easy"
            },
            {
                id: 2,
                question: "Who painted the Mona Lisa?",
                answer: "The Mona Lisa was painted by Leonardo da Vinci.",
                category: "arts",
                difficulty: "medium"
            },
            {
                id: 3,
                question: "What is the largest planet in our solar system?",
                answer: "Jupiter is the largest planet in our solar system.",
                category: "science",
                difficulty: "easy"
            },
            {
                id: 4,
                question: "In which year did World War II end?",
                answer: "World War II ended in 1945.",
                category: "history",
                difficulty: "medium"
            },
            {
                id: 5,
                question: "Who is known as the father of computers?",
                answer: "Charles Babbage is known as the father of computers.",
                category: "technology",
                difficulty: "medium"
            },
            {
                id: 6,
                question: "Which country won the FIFA World Cup in 2018?",
                answer: "France won the FIFA World Cup in 2018.",
                category: "sports",
                difficulty: "easy"
            },
            {
                id: 7,
                question: "What is the chemical symbol for gold?",
                answer: "The chemical symbol for gold is Au.",
                category: "science",
                difficulty: "easy"
            },
            {
                id: 8,
                question: "Who was the first woman to win a Nobel Prize?",
                answer: "Marie Curie was the first woman to win a Nobel Prize.",
                category: "history",
                difficulty: "hard"
            },
            {
                id: 9,
                question: "What is the tallest mountain in the world?",
                answer: "Mount Everest is the tallest mountain in the world.",
                category: "geography",
                difficulty: "easy"
            },
            {
                id: 10,
                question: "Which artist released the album 'Thriller' in 1982?",
                answer: "Michael Jackson released the album 'Thriller' in 1982.",
                category: "arts",
                difficulty: "medium"
            },
            // Add more questions here to reach 1000+
            // In a real application, these would be loaded from a database
        ];
        
        // For demo purposes, we'll duplicate the questions to simulate 1000+ questions
        function generateMoreQuestions() {
            const baseCount = questions.length;
            for (let i = baseCount + 1; i <= 1000; i++) {
                const randomBase = Math.floor(Math.random() * baseCount);
                const baseQuestion = questions[randomBase];
                questions.push({
                    id: i,
                    question: `${baseQuestion.question} (Variation ${i})`,
                    answer: `${baseQuestion.answer} (Variation ${i})`,
                    category: baseQuestion.category,
                    difficulty: baseQuestion.difficulty
                });
            }
        }
        
        generateMoreQuestions();
        
        // DOM elements
        const questionsContainer = document.getElementById('questions-container');
        const paginationContainer = document.getElementById('pagination');
        const categoryFilter = document.getElementById('category-filter');
        const searchInput = document.getElementById('search-input');
        const searchBtn = document.getElementById('search-btn');
        const questionForm = document.getElementById('question-form');
        const questionModal = document.getElementById('question-modal');
        const closeModal = document.querySelector('.close-modal');
        
        // Pagination variables
        let currentPage = 1;
        const questionsPerPage = 10;
        let filteredQuestions = [...questions];
        
        // Initialize the app
        function init() {
            renderQuestions();
            renderPagination();
            setupEventListeners();
        }
        
        // Render questions based on current page and filters
        function renderQuestions() {
            questionsContainer.innerHTML = '';
            
            const startIndex = (currentPage - 1) * questionsPerPage;
            const endIndex = startIndex + questionsPerPage;
            const questionsToShow = filteredQuestions.slice(startIndex, endIndex);
            
            if (questionsToShow.length === 0) {
                questionsContainer.innerHTML = '<p style="grid-column: 1/-1; text-align: center;">No questions found matching your criteria.</p>';
                return;
            }
            
            questionsToShow.forEach(q => {
                const questionCard = document.createElement('div');
                questionCard.className = 'question-card';
                questionCard.innerHTML = `
                    <div class="question-header">
                        <span class="question-category">${capitalizeFirstLetter(q.category)}</span>
                        <span class="question-difficulty">${capitalizeFirstLetter(q.difficulty)}</span>
                    </div>
                    <div class="question-body">
                        <p class="question-text">${q.question}</p>
                        <button class="show-answer-btn" data-id="${q.id}">Show Answer</button>
                        <div class="answer-text" id="answer-${q.id}">${q.answer}</div>
                    </div>
                `;
                questionsContainer.appendChild(questionCard);
            });
            
            // Add event listeners to show answer buttons
            document.querySelectorAll('.show-answer-btn').forEach(btn => {
                btn.addEventListener('click', function() {
                    const answerId = this.getAttribute('data-id');
                    const answerElement = document.getElementById(`answer-${answerId}`);
                    
                    if (answerElement.style.display === 'block') {
                        answerElement.style.display = 'none';
                        this.textContent = 'Show Answer';
                    } else {
                        answerElement.style.display = 'block';
                        this.textContent = 'Hide Answer';
                    }
                });
            });
        }
        
        // Render pagination buttons
        function renderPagination() {
            paginationContainer.innerHTML = '';
            const totalPages = Math.ceil(filteredQuestions.length / questionsPerPage);
            
            if (totalPages <= 1) return;
            
            // Previous button
            const prevBtn = document.createElement('button');
            prevBtn.innerHTML = '&laquo;';
            prevBtn.disabled = currentPage === 1;
            prevBtn.addEventListener('click', () => {
                if (currentPage > 1) {
                    currentPage--;
                    renderQuestions();
                    renderPagination();
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                }
            });
            paginationContainer.appendChild(prevBtn);
            
            // Page buttons
            const maxVisiblePages = 5;
            let startPage = Math.max(1, currentPage - Math.floor(maxVisiblePages / 2));
            let endPage = Math.min(totalPages, startPage + maxVisiblePages - 1);
            
            if (endPage - startPage + 1 < maxVisiblePages) {
                startPage = Math.max(1, endPage - maxVisiblePages + 1);
            }
            
            if (startPage > 1) {
                const firstPageBtn = document.createElement('button');
                firstPageBtn.textContent = '1';
                firstPageBtn.addEventListener('click', () => {
                    currentPage = 1;
                    renderQuestions();
                    renderPagination();
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                });
                paginationContainer.appendChild(firstPageBtn);
                
                if (startPage > 2) {
                    const ellipsis = document.createElement('span');
                    ellipsis.textContent = '...';
                    paginationContainer.appendChild(ellipsis);
                }
            }
            
            for (let i = startPage; i <= endPage; i++) {
                const pageBtn = document.createElement('button');
                pageBtn.textContent = i;
                if (i === currentPage) {
                    pageBtn.className = 'active';
                }
                pageBtn.addEventListener('click', () => {
                    currentPage = i;
                    renderQuestions();
                    renderPagination();
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                });
                paginationContainer.appendChild(pageBtn);
            }
            
            if (endPage < totalPages) {
                if (endPage < totalPages - 1) {
                    const ellipsis = document.createElement('span');
                    ellipsis.textContent = '...';
                    paginationContainer.appendChild(ellipsis);
                }
                
                const lastPageBtn = document.createElement('button');
                lastPageBtn.textContent = totalPages;
                lastPageBtn.addEventListener('click', () => {
                    currentPage = totalPages;
                    renderQuestions();
                    renderPagination();
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                });
                paginationContainer.appendChild(lastPageBtn);
            }
            
            // Next button
            const nextBtn = document.createElement('button');
            nextBtn.innerHTML = '&raquo;';
            nextBtn.disabled = currentPage === totalPages;
            nextBtn.addEventListener('click', () => {
                if (currentPage < totalPages) {
                    currentPage++;
                    renderQuestions();
                    renderPagination();
                    window.scrollTo({ top: 0, behavior: 'smooth' });
                }
            });
            paginationContainer.appendChild(nextBtn);
        }
        
        // Filter questions by category
        function filterQuestionsByCategory(category) {
            if (category === 'all') {
                filteredQuestions = [...questions];
            } else {
                filteredQuestions = questions.filter(q => q.category === category);
            }
            currentPage = 1;
            renderQuestions();
            renderPagination();
        }
        
        // Search questions
        function searchQuestions(query) {
            if (!query) {
                filteredQuestions = [...questions];
            } else {
                const lowerQuery = query.toLowerCase();
                filteredQuestions = questions.filter(q => 
                    q.question.toLowerCase().includes(lowerQuery) || 
                    q.answer.toLowerCase().includes(lowerQuery)
                );
            }
            currentPage = 1;
            renderQuestions();
            renderPagination();
        }
        
        // Add new question
        function addQuestion(newQuestion) {
            newQuestion.id = questions.length + 1;
            questions.unshift(newQuestion); // Add to beginning
            filteredQuestions.unshift(newQuestion);
            currentPage = 1;
            renderQuestions();
            renderPagination();
            
            // Show success message
            alert('Question added successfully!');
        }
        
        // Show question in modal
        function showQuestionInModal(question) {
            document.getElementById('modal-question').textContent = question.question;
            document.getElementById('modal-answer').textContent = question.answer;
            document.getElementById('modal-category').textContent = capitalizeFirstLetter(question.category);
            document.getElementById('modal-difficulty').textContent = capitalizeFirstLetter(question.difficulty);
            
            // Reset show answer button
            const showAnswerBtn = document.getElementById('modal-show-answer');
            showAnswerBtn.textContent = 'Show Answer';
            document.getElementById('modal-answer').style.display = 'none';
            
            showAnswerBtn.onclick = function() {
                const answerElement = document.getElementById('modal-answer');
                if (answerElement.style.display === 'block') {
                    answerElement.style.display = 'none';
                    this.textContent = 'Show Answer';
                } else {
                    answerElement.style.display = 'block';
                    this.textContent = 'Hide Answer';
                }
            };
            
            questionModal.style.display = 'flex';
        }
        
        // Setup event listeners
        function setupEventListeners() {
            // Category filter buttons
            document.querySelectorAll('.category-btn').forEach(btn => {
                btn.addEventListener('click', function() {
                    document.querySelectorAll('.category-btn').forEach(b => b.classList.remove('active'));
                    this.classList.add('active');
                    const category = this.getAttribute('data-category');
                    filterQuestionsByCategory(category);
                });
            });
            
            // Search functionality
            searchBtn.addEventListener('click', () => {
                searchQuestions(searchInput.value);
            });
            
            searchInput.addEventListener('keyup', (e) => {
                if (e.key === 'Enter') {
                    searchQuestions(searchInput.value);
                }
            });
            
            // Add question form
            questionForm.addEventListener('submit', (e) => {
                e.preventDefault();
                
                const newQuestion = {
                    question: document.getElementById('question').value,
                    answer: document.getElementById('answer').value,
                    category: document.getElementById('category').value,
                    difficulty: document.getElementById('difficulty').value
                };
                
                addQuestion(newQuestion);
                questionForm.reset();
            });
            
            // Modal close button
            closeModal.addEventListener('click', () => {
                questionModal.style.display = 'none';
            });
            
            // Close modal when clicking outside
            window.addEventListener('click', (e) => {
                if (e.target === questionModal) {
                    questionModal.style.display = 'none';
                }
            });
            
            // Random question button (if added to UI)
            // document.getElementById('random-question-btn').addEventListener('click', () => {
            //     const randomIndex = Math.floor(Math.random() * questions.length);
            //     showQuestionInModal(questions[randomIndex]);
            // });
        }
        
        // Helper function to capitalize first letter
        function capitalizeFirstLetter(string) {
            return string.charAt(0).toUpperCase() + string.slice(1);
        }
        
        // Initialize the app when DOM is loaded
        document.addEventListener('DOMContentLoaded', init);
    </script>
</body>
</html>
