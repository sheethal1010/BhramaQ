# BhramaQ - Quantum Computing Quiz

A static web application for learning quantum computing concepts through interactive quizzes.

## Features

- **3 Progressive Levels**: Qubit Basics, Bloch Sphere, and Dirac Notation
- **Interactive Quizzes**: 5 questions per level with up to 3 extra questions if needed
- **Chocolate Reward System**: Earn chocolates for passing each level (4+ correct answers)
- **Beautiful UI**: Quantum-themed design with particle animations
- **Progress Tracking**: LocalStorage-based progress tracking across levels

## Live Demo

Visit the live application: [https://sheethal1010.github.io/BhramaQ/](https://sheethal1010.github.io/BhramaQ/)

## Local Development

To run locally for development:

1. Clone the repository:
```bash
git clone https://github.com/sheethal1010/BhramaQ.git
cd BhramaQ
```

2. Serve the files using Python's built-in server:
```bash
# Python 3
python -m http.server 8000

# Or Python 2
python -m SimpleHTTPServer 8000
```

3. Open your browser and go to `http://localhost:8000`

## Deployment to GitHub Pages

This application is configured for automatic deployment to GitHub Pages:

1. Push your changes to the `main` branch
2. GitHub Actions will automatically deploy to `https://yourusername.github.io/BhramaQ/`
3. Make sure GitHub Pages is enabled in your repository settings

### Manual Deployment Steps

If you need to deploy manually:

1. Go to your repository on GitHub
2. Navigate to Settings → Pages
3. Select "Deploy from a branch" as the source
4. Choose `main` branch and `/ (root)` folder
5. Click Save

## Project Structure

```
BhramaQ/
├── index.html          # Home page
├── level.html          # Level selection page
├── quiz.html           # Quiz page with embedded questions
├── completed.html      # Results page
├── static/
│   └── style.css      # Styles and animations
├── data/
│   └── questions.json # Question database (for reference)
├── .github/
│   └── workflows/
│       └── deploy.yml # GitHub Actions deployment
└── README.md
```

## Learning Path

### Level 1: Qubit Basics
- Introduction to qubits and quantum states
- Difference between classical and quantum bits
- Basic quantum operations and measurements

### Level 2: Bloch Sphere Representation
- Geometric visualization of quantum states
- Understanding coordinates and angles
- Superposition states on the Bloch sphere

### Level 3: Dirac (Bra-Ket) Notation
- Mathematical notation for quantum states
- Bra-ket operations and inner products
- Expectation values and quantum measurements

## Scoring System

- **5 Initial Questions** per level
- **Up to 3 Extra Questions** if you haven't reached 4 points after the first 5
- **Passing Threshold**: 4 or more correct answers
- **Chocolate Rewards**: 1 chocolate per level when you pass
- **Live Scoring**: Immediate feedback with running score display

## Technologies Used

- Pure HTML5, CSS3, and JavaScript (no frameworks)
- LocalStorage for progress tracking
- CSS animations and particle effects
- Responsive design for mobile and desktop

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test them locally
4. Commit your changes: `git commit -m 'Add feature'`
5. Push to the branch: `git push origin feature-name`
6. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).
├── templates/
│   ├── index.html        # Landing page
│   ├── level.html        # Level selection page
│   ├── quiz.html         # Quiz interface
│   └── completed.html    # Results page
├── data/
│   └── questions.json    # Quiz questions organized by level
├── requirements.txt      # Python dependencies
└── README.md            # This file
```

## Installation

1. **Clone or download the project files**

2. **Navigate to the project directory**
   ```bash
   cd quantum_quiz
   ```

3. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**
   ```bash
   python app.py
   ```

5. **Open your browser and go to**
   ```
   http://localhost:5000
   ```

## How to Play

1. **Start**: Visit the home page to learn about quantum physics
2. **Choose Level**: Select from three difficulty levels:
   - **Level 1**: Quantum Basics (Beginner)
   - **Level 2**: Advanced Concepts (Intermediate)
   - **Level 3**: Quantum Applications (Advanced)
3. **Take Quiz**: Answer questions about quantum physics concepts
4. **Get Results**: See your score and performance breakdown

## Quiz Levels

### Level 1: Quantum Basics
- Wave-particle duality
- Superposition states
- Quantum measurement
- Heisenberg uncertainty principle

### Level 2: Advanced Concepts
- Quantum entanglement
- Bell's inequality
- Quantum tunneling
- Quantum teleportation

### Level 3: Quantum Applications
- Quantum computing
- Quantum cryptography
- Quantum sensors
- Quantum materials

## Technical Details

- **Backend**: Flask (Python)
- **Frontend**: HTML5, CSS3, JavaScript
- **Data**: JSON file with structured questions
- **Styling**: Custom quantum-themed CSS with animations
- **Responsive**: Mobile-friendly design

## Customization

### Adding New Questions
Edit `data/questions.json` to add new questions:

```json
{
  "question": "Your question here?",
  "options": [
    "Option A",
    "Option B", 
    "Option C",
    "Option D"
  ],
  "correct_answer": "Option A"
}
```

### Modifying Styles
Edit `static/style.css` to customize the appearance and animations.

### Adding New Levels
1. Add new level data to `questions.json`
2. Update the level selection template
3. Add corresponding routes in `app.py`

## Browser Compatibility

- Chrome (recommended)
- Firefox
- Safari
- Edge

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to contribute by:
- Adding new questions
- Improving the design
- Adding new features
- Reporting bugs

## Acknowledgments

- Quantum physics concepts and educational content
- Modern web design principles
- Flask framework for the backend
- CSS animations and effects

---

**Enjoy exploring the quantum realm!** ⚛️ 