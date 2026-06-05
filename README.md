/* === SECTIONS === */
.section { 
  margin-bottom: 30px; 
}

.section-title {
  font-family: 'Syne', sans-serif;
  font-size: 11px;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: var(--text);
  font-weight: 700;
  margin-bottom: 20px;
  display: flex;
  align-items: center;
  gap: 12px;
  position: relative;
}

/* Стильный минималистичный разделитель в линию с градиентной точкой */
.section-title::after {
  content: '';
  flex: 1;
  height: 1px;
  background: linear-gradient(90deg, rgba(78,205,230,0.2) 0%, rgba(255,255,255,0.02) 100%);
  display: block;
}

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

/* Настройки для боковой панели (Sidebar) — меняем цвет точки */
.sidebar .section-title::before { 
  background: linear-gradient(135deg, var(--accent-pink), var(--accent-purple)); 
  box-shadow: 0 0 8px var(--accent-pink);
}
