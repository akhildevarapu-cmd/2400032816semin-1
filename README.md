import React, { useState } from "react";
import "./Counter.css"; // optional: for custom styling

const Counter = () => {
  const [count, setCount] = useState(0);

  const increment = () => setCount(count + 1);
  const decrement = () => setCount(count - 1);
  const reset = () => setCount(0);

  return (
    <div className="counter-container">
      <h1>Counter: {count}</h1>
      <div className="button-group">
        <button className="btn increment" onClick={increment}>Increment</button>
        <button className="btn decrement" onClick={decrement}>Decrement</button>
        <button className="btn reset" onClick={reset}>Reset</button>
      </div>
    </div>
  );
};

export default Counter;
# 2400032816semin-1
