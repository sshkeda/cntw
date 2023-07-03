# cntw (classnames + tailwind-merge)

A simple JavaScript utility for conditionally joining [Tailwind CSS]("https://tailwindcss.com/") classes together.

## Installation

```bash
pnpm add cntw
```

## Usage

```tsx
import { cn } from "cntw";

export default function ButtonExample() {
  const disabled = true;

  return (
    <button
      className={cn(
        "rounded-md bg-green-500 px-4 py-2 font-bold text-white",
        disabled && "bg-red-500"
      )}
    >
      Click me
    </button>
  );
}
```
