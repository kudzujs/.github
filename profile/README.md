<p align="center">
  <a href="https://kudzujs.cloud">
    <img src="https://raw.githubusercontent.com/kudzujs/kudzu/main/public/icon-128.png" width="112" alt="Kudzu">
  </a>
</p>

<h1 align="center">Build like React. Ship like HTML.</h1>

<p align="center">
  React-shaped TSX with synchronous state, direct DOM patches, and no virtual DOM or hydration.
</p>

<p align="center">
  <a href="https://kudzujs.cloud">Website</a>
  &nbsp;&middot;&nbsp;
  <a href="https://kudzujs.cloud/docs">Documentation</a>
  &nbsp;&middot;&nbsp;
  <a href="https://github.com/kudzujs/kudzu">Source</a>
  &nbsp;&middot;&nbsp;
  <a href="https://www.npmjs.com/package/@kudzujs/core">npm</a>
</p>

---

Kudzu executes components at build time and emits complete HTML. Interactive pages receive only the capabilities they use: ordered state commands, reactive attributes, conditional ranges, keyed list moves, or external ESM handlers.

```tsx
import { useState } from "@kudzujs/core"

export default function Counter() {
  const [count, setCount] = useState(0)

  return (
    <button onClick={() => setCount(count + 1)}>
      Count: {count}
    </button>
  )
}
```

| HTML first | Direct updates | Capability based |
|:---|:---|:---|
| Static pages ship zero client JavaScript. | State targets text, properties, attributes, conditions, and keyed ranges directly. | Pages include only the runtime modules required by their behavior. |

## Start growing

```bash
npm create kudzu@latest my-app
cd my-app
npm run dev
```

## Projects

| Project | Purpose |
|:---|:---|
| [`kudzujs/kudzu`](https://github.com/kudzujs/kudzu) | Framework, compiler, runtime, documentation, and project generator |
| [`@kudzujs/core`](https://www.npmjs.com/package/@kudzujs/core) | Core package and `kudzu` CLI |
| [`create-kudzu`](https://www.npmjs.com/package/create-kudzu) | Minimal project scaffolding |

<p align="center">
  <sub>Static HTML first. Behavior grows only where it is needed.</sub>
</p>
