# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a simple, educational Snake game built as a single-file HTML application. The project is designed for an 11-year-old beginner with no programming knowledge, so all code should remain simple, well-commented, and easy to understand.

## Architecture

**Single-file structure**: The entire game is contained in `index.html` with embedded CSS and JavaScript. This design choice makes deployment trivial (just upload one file) and keeps the codebase approachable for beginners.

**Core components**:
- HTML structure with game container, canvas, score display, speed controls, and game over screen
- CSS for mobile-first responsive design with purple/blue gradient theme
- JavaScript game loop using `setInterval` for updates and rendering
- Touch event handlers for mobile swipe gestures
- Keyboard event handlers for desktop arrow key controls

## Development Guidelines

### Code Simplicity
- Keep all code in vanilla JavaScript (no frameworks or libraries)
- Use simple, descriptive variable names
- Add comments for complex logic
- Avoid advanced JavaScript features that would confuse beginners

### Mobile-First Design
- The game is optimized for mobile vertical layout
- Must support both swipe gestures (mobile) and arrow keys (desktop)
- Canvas and UI elements should scale responsively (90vw, max-width: 400px)
- Prevent backwards movement (snake can't reverse into itself)

### Game Configuration
- Grid-based movement system (20px grid size, 15x15 tiles)
- Three speed settings: Slow (250ms), Medium (150ms), Fast (80ms)
- Default speed is Medium
- Food appears as red circles, snake segments as purple/blue squares

### Running the Game
Simply open `index.html` in any modern web browser. No build process, dependencies, or server required.

### Deployment
Upload `index.html` to any web server or hosting service. The file is completely self-contained and requires no additional assets or configuration.

## Audience Considerations

When making changes or additions, remember this is designed for a child learning programming. Keep explanations simple, avoid technical jargon, and ensure any new features maintain the straightforward, single-file architecture.
