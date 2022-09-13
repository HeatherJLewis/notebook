# Exporting components in React.js

[Exporting components in React.js](https://bobbyhadz.com/blog/react-export-component-function).

## Named Exports
```
// 👇️ named export
export function Button() {
  return <button>Click</button>;
}

// 👇️ named export
export const SubmitButton = () => {
  return <button type="submit">Submit</button>;
};
```
# OR
```
function Button() {
  return <button>Click</button>;
}

const SubmitButton = () => {
  return <button type="submit">Submit</button>;
};

// 👇️ named exports
export {Button, SubmitButton};
```
## Named Imports
```
// 👇️ named exports
import {Button, SubmitButton} from './Buttons';

export default function App() {
  return (
    <div>
      <Button />

      <SubmitButton />
    </div>
  );
}
```

## Mixing Default and Named Imports:
Button.js
```
// 👇️ default export
export default function Button() {
  return <button>Click</button>;
}

// 👇️ named export
export const SubmitButton = () => {
  return <button type="submit">Submit</button>;
};
```
App.js
```
// 👇️ default and named imports
import Button, {SubmitButton} from './Buttons';
```
