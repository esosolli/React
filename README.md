import React, { useState } from 'react';

function App() {
  const [count, setCount] = useState(0); // Initialize count state to 0

  const increment = () => {
    setCount(count + 1); // Increment count
  };

  const decrement = () => {
    setCount(count - 1); // Decrement count
  };

  const reset = () => {
    setCount(0); // Reset count to 0
  };

  return (
    <div className="App">
      <h1>Click Counter App</h1>
     
      <button onClick={+1}>+</button>
      <button onClick={-1}>-</button>
      <button onClick={reset}>Reset</button>
    </div>
  );
}

export default App;