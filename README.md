* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background: #050816;
  color: white;
}

.slide {
  min-height: 100vh;
  padding: 80px 10%;
  display: flex;
  align-items: center;
  justify-content: space-between;

  background:
    radial-gradient(
      circle at 80% 20%,
      #633cff44,
      transparent 35%
    ),
    radial-gradient(
      circle at 10% 90%,
      #00d9ff33,
      transparent 30%
    );

  border-bottom: 1px solid #ffffff15;
}

.conteudo {
  max-width: 900px;
}

span {
  color: #5ee7ff;
  font-size: 15px;
  font-weight: bold;
  letter-spacing: 3px;
}

h1 {
  font-size: 80px;
  line-height: 1;
  margin: 30px 0;
}

h2 {
  font-size: 60px;
  margin: 30px 0;
}

b {
  color: #5ee7ff;
}

p {
  color: #b8c0d4;
  font-size: 22px;
  line-height: 1.5;
}

.imagem {
  font-size: 150px;
}

.imagem-grande {
  font-size: 200px;
  padding: 70px;
  border-radius: 50%;
  background: #ffffff08;
  box-shadow: 0 0 80px #4c6fff55;
}

.cards {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  margin-top: 40px;
}

.card {
  padding: 30px;
  border-radius: 20px;
  background: #ffffff08;
  border: 1px solid #ffffff15;
}

.card h3 {
  font-size: 23px;
  margin-bottom: 15px;
}

.card p {
  font-size: 17px;
}

.fluxo {
  display: flex;
  align-items: center;
  gap: 20px;
  margin-top: 50px;
}

.fluxo div {
  padding: 25px;
  min-width: 150px;
  text-align: center;
  border-radius: 18px;
  background: #ffffff0d;
  border: 1px solid #ffffff18;
  font-size: 30px;
}

.fluxo strong {
  display: block;
  font-size: 18px;
  margin-top: 10px;
}

.fluxo i {
  color: #5ee7ff;
  font-size: 30px;
}

ul {
  list-style: none;
  margin-top: 30px;
}

li {
  font-size: 24px;
  color: #d9deeb;
  padding: 15px 0;
}

blockquote {
  margin-top: 50px;
  font-size: 45px;
  line-height: 1.2;
  font-weight: bold;
  max-width: 900px;
}

.conexao {
  font-size: 50px;
  margin-top: 60px;
}

.final {
  flex-direction: column;
  justify-content: center;
  text-align: center;
}

.final h1 {
  max-width: 1000px;
}

.formula {
  margin: 40px 0;
  padding: 25px 45px;
  border-radius: 50px;
  background: linear-gradient(
    90deg,
    #00d9ff22,
    #704cff33
  );
  border: 1px solid #ffffff20;
  font-size: 25px;
  font-weight: bold;
}
