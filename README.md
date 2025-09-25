# Chess Engine

## Features

- **Graphical User Interface**: Built with X11 Graphics for smooth gameplay experience
- **5 Difficulty Levels**: From beginner-friendly to expert-level AI opponents
- **Advanced AI**: Implements alpha-beta pruned minimax algorithm with dynamic position evaluation
- **Deep Analysis**: Up to 8-turn lookahead on highest difficulty setting
- **Clean Architecture**: Follows MVC (Model-View-Controller) design pattern for maintainable code
- **Full Chess Rules**: Complete implementation of standard chess rules including castling, en passant, and pawn promotion

## Technologies Used

- **Language**: C++
- **Graphics**: X11 Graphics Library
- **Architecture**: Model-View-Controller (MVC)
- **AI Algorithm**: Alpha-Beta Pruned Minimax with Dynamic Position Evaluation

## Architecture

The project follows a clean MVC architecture:

- **Model**: Chess game logic, board state, move validation, and AI engine
- **View**: X11-based graphical interface for rendering the board and pieces
- **Controller**: Handles user input, game flow, and communication between model and view

## AI Difficulty Levels

1. **Level 1 (Beginner)**: Basic move evaluation with minimal lookahead
2. **Level 2 (Easy)**: Improved position evaluation with 2-turn lookahead
3. **Level 3 (Medium)**: Enhanced strategy with 4-turn lookahead
4. **Level 4 (Hard)**: Advanced positioning with 6-turn lookahead
5. **Level 5 (Expert)**: Full alpha-beta pruned minimax with 8-turn lookahead and dynamic position evaluation

# Installation

## Clone the repository
git clone https://github.com/yourusername/chess-engine.git
cd chess-engine

## Install X11 development libraries (Ubuntu/Debian)
sudo apt-get install libx11-dev

## Compile the project
g++ -o chess-engine *.cpp -lX11

## Run the game
./chess-engine


## Usage

1. Launch the game using `./chess-engine`
2. Select your preferred difficulty level (1-5)
3. Click on pieces to select them, then click on valid destination squares to move
4. The AI will automatically respond with its move
5. Continue playing until checkmate or stalemate

# Technical Details

## Alpha-Beta Pruning
The AI uses alpha-beta pruning to optimize the minimax algorithm, significantly reducing the number of positions evaluated while maintaining perfect play.

## Position Evaluation
Dynamic position evaluation considers:
- Material balance
- Piece positioning and mobility
- King safety
- Pawn structure
- Control of center squares
