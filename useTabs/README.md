# Usage

```js
import useTabs from '@nooks/use-tabs';
const App = () => {
  const { currentItem, changeItem } = useTabs(0, content);

  return (
    <div className='App'>
      <h1>Hello</h1>
      {content.map((section, index) => (
        <button onClick={() => changeItem(index)}>{section.tab}</button>
      ))}
      <div>{currentItem.content}</div>
    </div>
  );
};
```
