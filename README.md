.section { 
  margin-bottom: 35px; 
  clear: both; 
}

.section-title {
  font-family: 'Syne', sans-serif;
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: #ffffff;
  position: relative;
  padding-left: 15px;
  margin-bottom: 20px;
  line-height: 1.4;
}

.section-title::before {
  content: '';
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
  width: 6px; 
  height: 6px;
  border-radius: 50%;
  background: #4ecde6;
  box-shadow: 0 0 8px rgba(78, 205, 230, 0.6);
}

.section-title::after {
  content: '';
  display: block;
  width: 100%;
  height: 1px;
  margin-top: 8px;
  background: linear-gradient(90deg, rgba(78, 205, 230, 0.3) 0%, rgba(255, 255, 255, 0) 100%);
}

.sidebar .section-title::before { 
  background: #ff79c6;
  box-shadow: 0 0 8px rgba(255, 121, 198, 0.6);
}

.sidebar .section-title::after {
  background: linear-gradient(90deg, rgba(255, 121, 198, 0.3) 0%, rgba(255, 255, 255, 0) 100%);
}
