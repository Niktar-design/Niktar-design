<style>
.section { 
  margin-bottom: 40px; 
  clear: both; 
}

.section-title {
  font-family: 'Syne', sans-serif;
  font-size: 11px;
  font-weight: 700;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: #ffffff;
  position: relative;
  padding-left: 16px;
  margin-bottom: 25px;
}

.section-title::before {
  content: '';
  position: absolute;
  left: 0;
  bottom: 0.35em;
  width: 5px; 
  height: 5px;
  border-radius: 50%;
  background: #4ecde6;
  box-shadow: 0 0 10px rgba(78, 205, 230, 0.8);
}

.section-title::after {
  content: '';
  display: block;
  width: 120px;
  height: 1px;
  margin-top: 10px;
  background: linear-gradient(90deg, rgba(78, 205, 230, 0.4) 0%, rgba(78, 205, 230, 0) 100%);
}

.sidebar .section-title::before { 
  background: #ff79c6;
  box-shadow: 0 0 10px rgba(255, 121, 198, 0.8);
}

.sidebar .section-title::after {
  background: linear-gradient(90deg, rgba(255, 121, 198, 0.4) 0%, rgba(255, 121, 198, 0) 100%);
}
</style>
