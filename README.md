.section-title {
  font-family: 'Syne', sans-serif;
  font-size: 11px;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: var(--text);
  font-weight: 700;
  margin-bottom: 20px;
  
  /* Включаем флекс, чтобы линия шла строго в ряд с текстом */
  display: flex;
  align-items: center;
  gap: 12px;
}

/* Красивая светящаяся неоновая точка СЛЕВА от текста */
.section-title::before {
  content: '';
  width: 5px; 
  height: 5px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--accent-purple), var(--accent-blue));
  display: block;
  flex-shrink: 0;
  box-shadow: 0 0 8px var(--accent-blue);
}

/* Тонкая футуристичная линия, уходящая в прозрачность СПРАВА от текста */
.section-title::after {
  content: '';
  flex: 1;
  height: 1px;
  background: linear-gradient(90deg, rgba(78,205,230,0.25) 0%, rgba(255,255,255,0.02) 100%);
  display: block;
}

/* Если заголовок находится в боковой панели (левой колонке) — меняем цвета на розовый неон */
.sidebar .section-title::before { 
  background: linear-gradient(135deg, var(--accent-pink), var(--accent-purple)); 
  box-shadow: 0 0 8px var(--accent-pink);
}

.sidebar .section-title::after {
  background: linear-gradient(90deg, rgba(255,95,160,0.25) 0%, rgba(255,255,255,0.02) 100%);
}
