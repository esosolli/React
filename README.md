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
   setCount(0);// Reset count to 0
  };

  return (
    <div className="App">
      <h1>Click Counter App</h1>

      <button onClick={"() => setCount(count + 1)"}>Increment</button>

      <button onClick={"() => setCount(count - 1)"}>Dncrement</button>

      <button onClick={"() => setCount(0)"}>Reset</button>
 

      
      
    </div>
  );
}

export default App;