<!DOCTYPE html>
<!-- saved from url=(0089)file:///Users/Zhuanz/Desktop/Portfolio%20Application/03%20DigiTrove/DigiTrove%20Test.html -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Memory Preservation Engine | No-Code Solution</title>
    <style>
        :root {
            --primary: #4361ee;
            --secondary: #3f37c9;
            --accent: #4895ef;
            --light: #f8f9fa;
            --dark: #212529;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            min-height: 100vh;
            padding: 20px;
            color: var(--dark);
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            overflow: hidden;
        }
        
        header {
            background: linear-gradient(120deg, var(--primary), var(--secondary));
            color: white;
            padding: 30px 40px;
            text-align: center;
        }
        
        h1 {
            font-size: 2.2rem;
            margin-bottom: 10px;
        }
        
        .subtitle {
            font-size: 1.1rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }
        
        main {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            padding: 30px;
        }
        
        @media (max-width: 768px) {
            main {
                grid-template-columns: 1fr;
            }
        }
        
        .panel {
            background: var(--light);
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }
        
        .panel:hover {
            transform: translateY(-5px);
        }
        
        .panel h2 {
            color: var(--secondary);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--accent);
        }
        
        textarea {
            width: 100%;
            height: 150px;
            padding: 15px;
            border: 2px solid #e0e0e0;
            border-radius: 10px;
            font-size: 1rem;
            resize: vertical;
            transition: border-color 0.3s;
        }
        
        textarea:focus {
            outline: none;
            border-color: var(--accent);
        }
        
        button {
            background: linear-gradient(to right, var(--primary), var(--accent));
            color: white;
            border: none;
            padding: 12px 25px;
            font-size: 1rem;
            border-radius: 50px;
            cursor: pointer;
            margin-top: 15px;
            font-weight: 600;
            transition: transform 0.3s, box-shadow 0.3s;
            display: block;
            width: 100%;
        }
        
        button:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(67, 97, 238, 0.4);
        }
        
        .result-box {
            background: white;
            border-radius: 10px;
            padding: 20px;
            margin-top: 20px;
            border-left: 4px solid var(--accent);
            min-height: 100px;
        }
        
        .question {
            background: #e3f2fd;
            padding: 12px 15px;
            border-radius: 8px;
            margin-bottom: 10px;
            display: flex;
            align-items: flex-start;
        }
        
        .question:before {
            content: "❓";
            margin-right: 10px;
            font-size: 1.2rem;
        }
        
        .entity {
            display: inline-block;
            background: #bbdefb;
            padding: 3px 8px;
            border-radius: 4px;
            margin: 3px;
            font-size: 0.9rem;
        }
        
        .entity.person { background: #c8e6c9; }
        .entity.place { background: #ffecb3; }
        .entity.time { background: #e1bee7; }
        
        .visualization {
            background: white;
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
            text-align: center;
        }
        
        .node {
            display: inline-block;
            padding: 8px 15px;
            border-radius: 20px;
            margin: 5px;
            font-weight: 600;
        }
        
        .node.person { background: #c8e6c9; }
        .node.place { background: #ffecb3; }
        .node.time { background: #e1bee7; }
        .node.object { background: #bbdefb; }
        
        .connection {
            height: 2px;
            background: #90a4ae;
            margin: 10px auto;
            max-width: 200px;
        }
        
        footer {
            text-align: center;
            padding: 20px;
            color: #666;
            font-size: 0.9rem;
            border-top: 1px solid #eee;
        }
        
        .instructions {
            background: #fff8e1;
            padding: 15px;
            border-radius: 10px;
            margin: 20px 0;
            font-size: 0.95rem;
        }
        
        .instructions h3 {
            color: var(--secondary);
            margin-bottom: 10px;
        }
        
        .instructions ul {
            padding-left: 20px;
        }
        
        .instructions li {
            margin-bottom: 8px;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>DigiTrove AIGC Prototype Test</h1>
            <p class="subtitle">AI Guided Memory Archiving - Emotion enhancement engine &amp; Memory graph builder</p>
        </header>
        
        <main>
            <div class="panel">
                <h2>Emotion Enhancement Engine</h2>
                <div class="instructions">
                    <h3>Instructions</h3>
                    <ul>
                        <li>Enter an item story (English)</li>
                        <li>System analyzes emotional depth automatically</li>
                        <li>Generates guided questions to enrich details</li>
                        <li>Perfect for: family history, personal memoirs, oral history</li>
                    </ul>
                </div>
                
                <textarea id="storyInput" placeholder="Enter your story here... Example: This wicker chair was handcrafted by my father in 1958 as a wedding gift for my mother.">This wicker chair was handcrafted by my father in 1958 as a wedding gift for my mother.</textarea>
                <button onclick="analyzeStory()">Analyze Story &amp; Generate Questions</button>
                
                <div class="result-box">
                    <h3>Emotion Enhancement Questions:</h3>
                    <div id="emotionResults"><div class="question">Could you share more about your father? What inspired him/her to create/obtain this item?</div><div class="question">How did you feel when you received this gift? What was special about that moment?</div></div>
                </div>
            </div>
            
            <div class="panel">
                <h2>Memory Graph Builder</h2>
                <div class="instructions">
                    <h3>Instructions</h3>
                    <ul>
                        <li>Automatically identifies people, places, times</li>
                        <li>Visualizes relationships between memory elements</li>
                        <li>Generates questions to expand memory network</li>
                        <li>Perfect for: family trees, historical events, memory training</li>
                    </ul>
                </div>
                
                <div class="result-box">
                    <h3>Memory Graph:</h3>
                    <div id="memoryGraph"><div class="visualization"><div class="node person">People: Father, Mother</div><div class="connection"></div><div class="node time">Times: 1958</div><div class="connection"></div><div class="node object">Objects: Chair, Gift</div></div></div>
                    
                    <h3 style="margin-top: 20px;">Memory Expansion Questions:</h3>
                    <div id="memoryQuestions"><div class="question">What special interactions did you have with Father in this story?</div><div class="question">What was life like during 1958?</div></div>
                </div>
            </div>
        </main>
        
        <footer>
            <p>Emotion Enhancement Engine &amp; Memory Graph Builder | Ruiyang Chen's Prortfolio project test</p>
            <p>DigiTrove</p>
        </footer>
    </div>

    <script>
        // Emotion Analysis Engine Core Logic
        function analyzeSentiment(story) {
            // Simplified sentiment analysis logic
            const positiveWords = ['happy', 'joy', 'love', 'cherish', 'like', 'treasure', 'blessed', 'moved', 'warm', 'special'];
            const negativeWords = ['sad', 'pain', 'loss', 'regret', 'hurt', 'grief', 'disappointed'];
            
            let sentimentScore = 0;
            let positiveCount = 0;
            let negativeCount = 0;
            
            // Check for positive and negative words
            positiveWords.forEach(word => {
                const regex = new RegExp(`\\b${word}\\b`, 'gi');
                if (story.match(regex)) {
                    positiveCount += story.match(regex).length;
                }
            });
            
            negativeWords.forEach(word => {
                const regex = new RegExp(`\\b${word}\\b`, 'gi');
                if (story.match(regex)) {
                    negativeCount += story.match(regex).length;
                }
            });
            
            // Calculate sentiment score
            sentimentScore = (positiveCount - negativeCount) / 10;
            sentimentScore = Math.max(-1, Math.min(1, sentimentScore));
            
            return sentimentScore;
        }
        
        // Generate Emotion-Guided Questions
        function generateEmotionQuestions(story, sentimentScore) {
            const questions = [];
            
            // Generate questions for neutral content
            if (sentimentScore > -0.2 && sentimentScore < 0.3) {
                if (story.includes('father') || story.includes('dad') || story.includes('mother') || story.includes('mom')) {
                    const person = story.includes('father') || story.includes('dad') ? 'father' : 'mother';
                    questions.push(`Could you share more about your ${person}? What inspired him/her to create/obtain this item?`);
                }
                
                if (story.includes('gift') || story.includes('present')) {
                    questions.push("How did you feel when you received this gift? What was special about that moment?");
                }
                
                if (questions.length === 0) {
                    questions.push("What detail of this story is most important for you to remember?");
                    questions.push("Can you describe the environment where this happened?");
                }
            }
            
            // Generate questions for positive content
            if (sentimentScore > 0.6) {
                questions.push("What was the most touching moment in this wonderful memory?");
                questions.push("Why was this moment so special to you?");
            }
            
            // Generate questions for negative content
            if (sentimentScore < -0.4) {
                questions.push("What did this difficult experience teach you?");
                questions.push("Looking back now, how do you view this experience differently?");
            }
            
            // Add generic questions if needed
            if (questions.length < 2) {
                questions.push("What special moments does this item remind you of?");
                questions.push("What detail of this item do you cherish most and why?");
            }
            
            return questions.slice(0, 3); // Return max 3 questions
        }
        
        // Build Memory Graph
        function buildMemoryGraph(story) {
            const entities = {
                persons: [],
                places: [],
                times: [],
                objects: []
            };
            
            // Extract people
            const personKeywords = ['father', 'mother', 'grandfather', 'grandmother', 'friend', 'uncle', 
                                  'aunt', 'brother', 'sister', 'husband', 'wife', 'son', 'daughter'];
            personKeywords.forEach(keyword => {
                const regex = new RegExp(`\\b${keyword}\\b`, 'gi');
                if (story.match(regex)) {
                    entities.persons.push(keyword.charAt(0).toUpperCase() + keyword.slice(1));
                }
            });
            
            // Extract places
            const placeKeywords = ['home', 'school', 'park', 'garden', 'village', 'city', 'town', 
                                  'house', 'beach', 'church', 'kitchen', 'room', 'country'];
            placeKeywords.forEach(keyword => {
                const regex = new RegExp(`\\b${keyword}\\b`, 'gi');
                if (story.match(regex)) {
                    entities.places.push(keyword.charAt(0).toUpperCase() + keyword.slice(1));
                }
            });
            
            // Extract times
            const timePattern = /(19|20)\d{2}s?|\d{4}|years ago|childhood|youth|summer|winter|spring|autumn|fall/gi;
            const times = story.match(timePattern);
            if (times) {
                entities.times = [...new Set(times)]; // Remove duplicates
            }
            
            // Extract objects
            const objectKeywords = ['chair', 'table', 'photo', 'clothes', 'book', 'letter', 'ring', 
                                   'watch', 'painting', 'gift', 'toy', 'dress', 'tool'];
            objectKeywords.forEach(keyword => {
                const regex = new RegExp(`\\b${keyword}\\b`, 'gi');
                if (story.match(regex)) {
                    entities.objects.push(keyword.charAt(0).toUpperCase() + keyword.slice(1));
                }
            });
            
            return entities;
        }
        
        // Generate Memory-Guided Questions
        function generateMemoryQuestions(entities) {
            const questions = [];
            
            if (entities.persons.length > 0) {
                questions.push(`What special interactions did you have with ${entities.persons[0]} in this story?`);
            }
            
            if (entities.places.length > 0) {
                questions.push(`What memories do you associate with ${entities.places[0]}?`);
            }
            
            if (entities.times.length > 0) {
                questions.push(`What was life like during ${entities.times[0]}?`);
            }
            
            if (questions.length === 0) {
                questions.push("What was the most important object in this story and why?");
                questions.push("Where did this story take place? Can you describe that location?");
            }
            
            return questions.slice(0, 2); // Return max 2 questions
        }
        
        // Main analysis function
        function analyzeStory() {
            const story = document.getElementById('storyInput').value;
            
            if (!story.trim()) {
                alert('Please enter your story');
                return;
            }
            
            // Emotion analysis
            const sentimentScore = analyzeSentiment(story);
            const emotionQuestions = generateEmotionQuestions(story, sentimentScore);
            
            // Display emotion analysis results
            let emotionHTML = '';
            emotionQuestions.forEach(question => {
                emotionHTML += `<div class="question">${question}</div>`;
            });
            
            document.getElementById('emotionResults').innerHTML = emotionHTML;
            
            // Memory graph analysis
            const entities = buildMemoryGraph(story);
            const memoryQuestions = generateMemoryQuestions(entities);
            
            // Display memory graph
            let graphHTML = '<div class="visualization">';
            
            if (entities.persons.length > 0) {
                graphHTML += '<div class="node person">People: ' + entities.persons.join(', ') + '</div>';
            }
            
            if (entities.places.length > 0) {
                graphHTML += '<div class="connection"></div>';
                graphHTML += '<div class="node place">Places: ' + entities.places.join(', ') + '</div>';
            }
            
            if (entities.times.length > 0) {
                graphHTML += '<div class="connection"></div>';
                graphHTML += '<div class="node time">Times: ' + entities.times.join(', ') + '</div>';
            }
            
            if (entities.objects.length > 0) {
                graphHTML += '<div class="connection"></div>';
                graphHTML += '<div class="node object">Objects: ' + entities.objects.join(', ') + '</div>';
            }
            
            if (entities.persons.length === 0 && entities.places.length === 0 && 
                entities.times.length === 0 && entities.objects.length === 0) {
                graphHTML += '<p>No key entities identified. Try adding more details to your story.</p>';
            }
            
            graphHTML += '</div>';
            document.getElementById('memoryGraph').innerHTML = graphHTML;
            
            // Display memory questions
            let memoryQuestionsHTML = '';
            memoryQuestions.forEach(question => {
                memoryQuestionsHTML += `<div class="question">${question}</div>`;
            });
            
            document.getElementById('memoryQuestions').innerHTML = memoryQuestionsHTML;
        }
        
        // Initialize on page load
        window.onload = function() {
            // Auto-analyze example story
            setTimeout(analyzeStory, 500);
        };
    </script>

</body></html>
