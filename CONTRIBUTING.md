# 🤝 Contributing to Arcade Zone

Thank you for interest in contributing to Arcade Zone! We welcome all kinds of contributions.

## Ways You Can Help

### 🐛 Report Bugs
Found a bug? Open an issue with:
- Browser and OS you're using
- Steps to reproduce the problem
- Expected vs actual behavior
- Screenshot (if helpful)

### ✨ Suggest Features
Have an idea? Open an issue describing:
- What feature you'd like to add
- Why it would be cool
- How it would work

### 🎮 Add New Games
Want to add more games? 

1. Find an embeddable game (check codepen.io, itch.io, or github.com)
2. Get the game's URL or embed code
3. Edit `index.html` and add to the `GAMES` object:

```javascript
newgame: {
    name: 'GAME NAME',
    url: 'https://game-url.com',
    controls: '► Control instructions'
}
```

4. Add a game item to the HTML sidebar:

```html
<div class="game-item" data-game="newgame" data-tagline="Your tagline">
    <span class="game-item-icon">😀</span>
    <span class="game-item-name">GAME NAME</span>
    <span class="game-item-tagline">Your tagline</span>
</div>
```

### 🎨 Design Improvements
- Better color schemes
- New visual effects
- Mobile optimization
- Accessibility improvements (a11y)

### 📚 Documentation
- Better README sections
- Tutorial/guide additions
- Fix typos
- Translate to other languages

### 🧪 Fix Known Issues
Check the Issues page and comment to claim one!

## Development Setup

```bash
# 1. Fork the repository (GitHub button)

# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/Arcade.git
cd Arcade

# 3. Create a branch
git checkout -b my-feature

# 4. Make your changes
# Edit index.html or create new files

# 5. Test locally
python -m http.server 8000
# Visit http://localhost:8000

# 6. Commit and push
git add .
git commit -m "Add: Description of your change"
git push origin my-feature

# 7. Open a Pull Request on GitHub
```

## Code Style

- Keep HTML readable and well-commented
- Use CSS custom properties (variables) for colors
- Write vanilla JavaScript (no frameworks)
- Test in multiple browsers
- Keep file size small

## Pull Request Guidelines

When you open a PR, please include:

1. **Description**: What does this change do?
2. **Why**: Why is this change needed?
3. **Testing**: How did you test it? (browsers, devices)
4. **Screenshots**: Before/after if visual changes

## Community Guidelines

- Be respectful and welcoming
- No spam or self-promotion
- Constructive feedback only
- Help others when possible

## Questions?

- Ask in an issue
- Check existing documentation
- Look at similar contributions for examples

## Recognition

Contributors will be recognized in:
- README.md Contributors section
- GitHub contributors page
- Release notes

---

**Thank you for helping make Arcade Zone awesome! 🕹️✨**
