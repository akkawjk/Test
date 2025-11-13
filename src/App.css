import React, { useState } from 'react';
import './App.css'; // 需创建对应 CSS 文件

const App: React.FC = () => {
  const [btnIndex, setBtnIndex] = useState(1);
  const [activeBtns, setActiveBtns] = useState<number[]>([]);

  // 新增按钮点击事件
  const handleAddBtn = () => {
    setBtnIndex(prev => prev + 1);
  };

  // 列表按钮激活状态切换
  const toggleActive = (index: number) => {
    setActiveBtns(prev => 
      prev.includes(index) 
        ? prev.filter(item => item !== index) 
        : [...prev, index]
    );
  };

  // 生成列表按钮（排除 Add Button 本身）
  const renderListBtns = () => {
    const btns = [];
    for (let i = 1; i < btnIndex; i++) {
      btns.push(
        <button
          key={i}
          className={`list-btn ${activeBtns.includes(i) ? 'active' : ''}`}
          onClick={() => toggleActive(i)}
        >
          Button {i}
        </button>
      );
    }
    return btns;
  };

  return (
    <div className="app-container">
      <div className="btn-container">
        {renderListBtns()}
        <button className="add-btn" onClick={handleAddBtn}>
          Add Button
        </button>
      </div>
    </div>
  );
};

export default App;
