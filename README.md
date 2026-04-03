# Complex Numbers

React + Vite visualization of the complex plane and basic operations on \(a+bi\) (inputs and arithmetic in `ComplexNumbers.jsx`).

**Live site:** [https://content-interactives.github.io/complex_numbers](https://content-interactives.github.io/complex_numbers)

Curriculum alignment and placement: [Standards.md](Standards.md).

---

## Stack

| Layer | Notes |
|--------|--------|
| Build | Vite 6, `@vitejs/plugin-react` |
| UI | React 19 |
| Styling | Tailwind 3 |
| Icons | lucide-react |
| Deploy | `gh-pages -d dist`; `predeploy` runs `vite build` |

---

## Layout

```
vite.config.js          # base: '/complex_numbers/'
src/
  main.jsx → App.jsx → components/ComplexNumbers.jsx
  components/ui/
```

---

## `vite.config.js`

`base: '/complex_numbers/'` must match the GitHub Pages repository path.

---

## Scripts

| Command | Purpose |
|---------|---------|
| `npm run dev` | Vite dev server |
| `npm run build` | Production build → `dist/` |
| `npm run preview` | Preview production build |
| `npm run lint` | ESLint |
| `npm run deploy` | Build and push `dist/` to `gh-pages` |

---

## Embedding

Argand diagram size is set in `ComplexNumbers.jsx`; scale iframe to avoid clipping.
