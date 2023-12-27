import React, { useState } from 'react';

const FlipTheCoin = () => {
 const [result, setResult] = useState('');

 const flipCoin = () => {
    const flipResult = Math.random() > 0.5 ? 'Heads' : 'Tails';
    setResult(flipResult);
 };

 return (
    <div>
      <button onClick={flipCoin}>Flip the Coin</button>
      <h1>{result
