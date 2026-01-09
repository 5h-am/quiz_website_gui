# Akashic Records Quiz 📚✨

A beautiful, interactive quiz application that tests your knowledge across various categories and subcategories. Built with vanilla HTML, CSS, and JavaScript.

## 🌐 Live Demo

**Website Link:** [https://5h-am.github.io/quiz_website_gui/]

---

## 📖 About

Akashic Records is a knowledge-testing quiz platform featuring a mystical theme and elegant design. The name "Akashic Records" refers to a compendium of all universal events, thoughts, and knowledge—making it the perfect name for a comprehensive quiz application!

---

## ✨ Features

### Core Functionality
- **User Registration**: Personalized quiz experience with name registration
- **Multiple Categories**: Choose from various quiz categories
- **Dynamic Subcategories**: Each category contains specialized subcategories
- **20 Questions Per Quiz**: Comprehensive testing on selected topics
- **Randomized Questions**: Questions are shuffled for each session
- **Answer Checking**: Optional "Check Answer" feature for learning mode
- **Real-time Feedback**: Visual highlighting of selected answers
- **Detailed Results**: Complete breakdown of performance including:
  - Correct answers
  - Wrong answers
  - Skipped questions
  - Answers checked (transparency feature)

### User Experience
- **Intuitive Navigation**: Step-by-step flow from registration to results
- **Responsive Design**: Clean, centered layout that works on various screen sizes
- **Visual Feedback**: Hover effects and active states for all interactive elements
- **Session Management**: Progress saved using sessionStorage
- **Play Again**: Easy restart functionality after completing a quiz

---

## 🎨 Design Highlights

- **Custom Typography**: 
  - "Playwrite IT Moderna Guides" for headers
  - "Italianno" for subtitles
  - "Itim" for buttons and labels
  - "Noto Sans Old Italic" for quiz content
  
- **Color Palette**:
  - Primary: Teal (#48C9B0)
  - Accent: Purple shades (#E8DAEF, #BB8FCE)
  - Quiz UI: Soft pink (#FADBD8, #EC7063)
  - Clean white containers with subtle shadows

- **Smooth Animations**: Hover effects with transforms and color transitions

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Basic understanding of file structure

### Installation

1. **Clone or download this repository**
   ```bash
   git clone [your-repo-link]
   cd akashic-records-quiz
   ```

2. **File Structure**
   ```
   project-folder/
   ├── index.html          # Landing page
   ├── quiz_page.html      # Quiz interface
   ├── style.css           # Styling
   ├── script.js           # Core logic
   └── [data-file]         # Your quiz questions data
   ```

3. **Add Your Quiz Data**
   - Create a JavaScript file with your quiz data
   - Structure it as referenced in `script.js` (see Data Format section)
   - Link it in both HTML files before `script.js`

4. **Launch**
   - Simply open `index.html` in your browser
   - Or use a local server for better performance

---

## 📊 Data Format

Your quiz data should follow this structure:

```javascript
// Categories list
const categories: ["History", "Science", "Geography"];
const records = {  
  // Questions by category and subcategory
  History_questions: {
    "Ancient Civilizations": [
      "Question 1?",
      "Question 2?",
      // ... 20 questions total
    ]
  },
  
  // Options (4 per question)
  History_options: {
    "Ancient Civilizations": [
      ["Option A", "Option B", "Option C", "Option D"],
      ["Option A", "Option B", "Option C", "Option D"],
      // ... matching the questions
    ]
  },
  
  // Correct answers
  History_answers: {
    "Ancient Civilizations": [
      "Correct Answer 1",
      "Correct Answer 2",
      // ... matching the questions
    ]
  }
};
```

---

## 🎮 How to Play

1. **Start**: Click the "START" button on the homepage
2. **Register**: Enter your name (will be displayed on results)
3. **Select Category**: Choose your preferred quiz category from dropdown
4. **Select Subcategory**: Pick a specific topic within that category
5. **Answer Questions**: 
   - Click on your chosen answer (A, B, C, or D)
   - Use "Check Answer" if you want to see the correct answer (tracked in results)
   - Click "Next" to proceed
   - Skip questions by clicking "Next" without selecting
6. **Submit**: After question 20, click "Submit" to see your results
7. **Review**: Check your performance breakdown
8. **Play Again**: Click to start a new quiz

---

## 🛠️ Technical Details

### Technologies Used
- **HTML5**: Semantic structure
- **CSS3**: Custom styling with Google Fonts
- **Vanilla JavaScript**: Core functionality, no frameworks

### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Storage
- Uses `sessionStorage` for temporary data persistence
- Data clears when browser tab/window is closed

---

## 🔧 Customization

### Changing Colors
Edit `style.css` and modify the color variables in relevant selectors:
```css
body {
    background-color: #48C9B0; /* Change main background */
}
```

### Adding More Questions
Simply extend your data file with more categories, subcategories, and questions following the established format.

### Modifying Question Count
In `script.js`, change the condition from `if (i < 19)` to your desired number minus 1.

---

## 📝 Known Limitations

- Questions must be exactly 20 per subcategory
- No timer functionality
- Results not saved permanently (session only)
- No answer review after submission
- Single-player mode only

---

## 🚧 Future Enhancements

- [ ] Timer for each question
- [ ] Difficulty levels
- [ ] Leaderboard system
- [ ] Answer review after quiz completion
- [ ] Multiplayer mode
- [ ] Score history tracking
- [ ] Question bookmarking
- [ ] Hint system
- [ ] Mobile app version

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👤 Author

**Shubham Kumar**

- GitHub: [5h-am]
- Website: [https://5h-am.github.io/quiz_website_gui/]
- Email: shame06rxl@gmail.com

---

## 🙏 Acknowledgments

- Google Fonts for the beautiful typography
- Inspiration from various quiz platforms
- The concept of Akashic Records from spiritual philosophy

---

**Enjoy testing your knowledge! 🎓**

*Made with ❤️ and JavaScript*