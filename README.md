# Scramble Words

A word-unscrambling game built with React + TypeScript. Guess the original word from its shuffled letters, with an error counter, limited skips, and a score.

## Stack

- React 19 + TypeScript
- Vite
- Tailwind CSS v4
- shadcn/ui (Button, Input, Card)
- lucide-react (icons)
- State managed with `useReducer`

## How to play

- A word is shown with its letters scrambled.
- Type your guess and press **Enviar Adivinanza** (Submit Guess).
- A correct guess earns a point and moves to the next word.
- A wrong guess adds to the error counter (max 3 before game over).
- You can skip a word (max 3 skips).
- Once the words run out or the max errors are reached, a summary is shown along with a **Jugar de nuevo** (Play Again) option.

## Installation

```bash
npm install
```

## Scripts

```bash
npm run dev      # start dev server
npm run build    # production build (tsc + vite build)
npm run preview  # preview the build
npm run lint     # run ESLint
```

## Project structure

```
src/
├── ScrambleWords.tsx           # Main game component
├── reducer/
│   └── scrambleWorldReducer.ts # Game state, actions, and logic
└── components/ui/              # shadcn/ui components (Button, Input, Card)
```

## Prerequisites

This project uses [shadcn/ui](https://ui.shadcn.com/docs/installation/vite) components.
