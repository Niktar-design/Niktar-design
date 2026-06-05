/* === SECTIONS & HEADINGS === */
.section { 
  margin-bottom: 35px; 
  clear: both; /* Защита от наплывания плавающих элементов */
}

.section-title {
  font-family: 'Syne', sans-serif;
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: #ffffff; /* Базовый белый, поменяйте на var(--text), если нужно */
  
  position: relative;
  padding-left: 15px; /* Место под точку */
  margin-bottom: 20px;
  line-height: 1.4;
}

/* Элегантная светящаяся точка слева от заголовка */
.section-title::before {
  content: '';
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
  width: 6px; 
  height: 6px;
  border-radius: 50%;
  background: #4ecde6; /* Акцентный голубой */
  box-shadow: 0 0 8px rgba(78, 205, 230, 0.6);
}

/* Тонкая линия подчеркивания, уходящая в прозрачность */
.section-title::after {
  content: '';
  display: block;
  width: 100%;
  height: 1px;
  margin-top: 8px;
  background: linear-gradient(90deg, rgba(78, 205, 230, 0.3) 0%, rgba(255, 255, 255, 0) 100%);
}

/* Стилизация для боковой панели (Sidebar) — меняем цвет на розовый/фиолетовый */
.sidebar .section-title::before { 
  background: #ff79c6; /* Розовый акцент */
  box-shadow: 0 0 8px rgba(255, 121, 198, 0.6);
}

.sidebar .section-title::after {
  background: linear-gradient(90deg, rgba(255, 121, 198, 0.3) 0%, rgba(255, 255, 255, 0) 100%);
}
