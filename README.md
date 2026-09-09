Sim. Essas palavras são apenas **comentários dentro do código** e não aparecem no slide, mas removi todas para deixar o código mais limpo.

```
<!DOCTYPE html>
<html lang="pt-BR">

<head>

    <meta charset="UTF-8">

    <meta name="viewport"
          content="width=device-width, initial-scale=1.0">

    <title>Visão para Tecnologia</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #050816;
            color: white;
            overflow: hidden;
        }

        .slide {
            width: 100vw;
            height: 100vh;

            display: none;

            align-items: center;
            justify-content: center;

            padding: 80px 9vw;

            position: relative;
            overflow: hidden;

            background:
                radial-gradient(
                    circle at 85% 20%,
                    #704cff55,
                    transparent 35%
                ),
                radial-gradient(
                    circle at 10% 90%,
                    #00d9ff33,
                    transparent 30%
                ),
                #050816;
        }

        .slide.active {
            display: flex;
        }

        .conteudo {
            width: 100%;
            max-width: 1100px;
            position: relative;
            z-index: 2;
        }

        .tag {
            color: #5ee7ff;
            font-size: 15px;
            font-weight: bold;
            letter-spacing: 3px;
            text-transform: uppercase;
        }

        h1 {
            font-size: clamp(55px, 7vw, 100px);
            line-height: 0.95;
            margin: 30px 0;
        }

        h2 {
            font-size: clamp(42px, 5vw, 70px);
            line-height: 1;
            margin: 30px 0 45px;
        }

        b {
            color: #5ee7ff;
        }

        p {
            color: #b8c0d4;
            font-size: 23px;
            line-height: 1.5;
        }

        .slide-capa {
            justify-content: flex-start;
        }

        .linha {
            width: 110px;
            height: 5px;

            margin: 35px 0;

            border-radius: 10px;

            background:
                linear-gradient(
                    90deg,
                    #00d9ff,
                    #704cff
                );
        }

        .icone-capa {
            position: absolute;

            right: 10%;
            top: 32%;

            font-size: 180px;

            filter:
                drop-shadow(
                    0 0 35px #00d9ff88
                );
        }

        .cards {
            display: grid;

            grid-template-columns:
                repeat(4, 1fr);

            gap: 20px;

            margin-top: 40px;
        }

        .card {
            min-height: 210px;

            padding: 30px;

            border-radius: 22px;

            background: #ffffff08;

            border:
                1px solid #ffffff18;

            backdrop-filter: blur(15px);

            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-8px);
            border-color: #5ee7ff;
        }

        .card-icon {
            font-size: 42px;
            margin-bottom: 25px;
        }

        .card h3 {
            font-size: 21px;
            margin-bottom: 12px;
        }

        .card p {
            font-size: 16px;
        }

        .fluxo {
            display: flex;

            align-items: center;
            justify-content: center;

            gap: 18px;

            margin-top: 55px;
        }

        .etapa {
            min-width: 170px;

            padding: 28px 20px;

            text-align: center;

            border-radius: 20px;

            background: #ffffff08;

            border:
                1px solid #ffffff18;

            font-size: 38px;
        }

        .etapa strong {
            display: block;

            margin-top: 12px;

            font-size: 19px;
        }

        .seta {
            color: #5ee7ff;
            font-size: 35px;
        }

        .ia-layout {
            width: 100%;

            display: grid;

            grid-template-columns:
                1fr 1fr;

            align-items: center;

            gap: 100px;
        }

        .lista {
            list-style: none;
            margin-top: 20px;
        }

        .lista li {
            color: #dce2ef;

            font-size: 22px;

            padding: 18px 0;

            border-bottom:
                1px solid #ffffff15;
        }

        .lista li::before {
            content: "✓";

            color: #5ee7ff;

            font-weight: bold;

            margin-right: 15px;
        }

        .cerebro {
            width: 400px;
            height: 400px;

            margin: auto;

            display: flex;

            align-items: center;
            justify-content: center;

            border-radius: 50%;

            font-size: 140px;

            background:
                radial-gradient(
                    circle,
                    #172b55,
                    #091126 60%,
                    transparent 70%
                );

            border:
                1px solid #5ee7ff55;

            box-shadow:
                0 0 80px #4264ff55,
                inset 0 0 60px #00d9ff22;
        }

        .visao {
            max-width: 1050px;
        }

        blockquote {
            max-width: 950px;

            margin-top: 40px;

            font-size:
                clamp(38px, 5vw, 65px);

            line-height: 1.15;

            font-weight: bold;
        }

        .conexao {
            margin-top: 55px;

            font-size: 50px;

            color: #5ee7ff;
        }

        .slide-final {
            text-align: center;
        }

        .slide-final .conteudo {
            display: flex;

            flex-direction: column;

            align-items: center;
        }

        .formula {
            margin: 40px 0;

            padding: 25px 45px;

            border-radius: 50px;

            background:
                linear-gradient(
                    90deg,
                    #00d9ff22,
                    #704cff33
                );

            border:
                1px solid #ffffff20;

            font-size: 25px;

            font-weight: bold;
        }

        .frase-final {
            color: #5ee7ff;

            font-size: 25px;

            font-weight: bold;
        }

        .navegacao {
            position: fixed;

            right: 35px;
            bottom: 30px;

            display: flex;

            gap: 10px;

            z-index: 100;
        }

        .navegacao button {
            width: 50px;
            height: 50px;

            border-radius: 50%;

            border:
                1px solid #ffffff30;

            background: #ffffff10;

            color: white;

            font-size: 22px;

            cursor: pointer;

            transition: 0.3s;
        }

        .navegacao button:hover {
            background: #5ee7ff;
            color: #050816;
        }

        @media (max-width: 900px) {

            .cards {
                grid-template-columns:
                    repeat(2, 1fr);
            }

            .ia-layout {
                grid-template-columns: 1fr;
                gap: 30px;
            }

            .cerebro {
                width: 250px;
                height: 250px;
                font-size: 90px;
            }

            .fluxo {
                flex-wrap: wrap;
            }

            .icone-capa {
                opacity: 0.2;
            }
        }

    </style>

</head>

<body>

    <section class="slide active slide-capa">

        <div class="conteudo">

            <div class="tag">
                Tecnologia • Inovação • Futuro
            </div>

            <h1>
                Visão para<br>
                <b>Tecnologia</b>
            </h1>

            <div class="linha"></div>

            <p>
                Tecnologia que transforma o presente
                e constrói o futuro.
            </p>

        </div>

        <div class="icone-capa">
            💻
        </div>

    </section>

    <section class="slide">

        <div class="conteudo">

            <div class="tag">
                Futuro digital
            </div>

            <h2>
                O futuro é <b>digital</b>
            </h2>

            <div class="cards">

                <div class="card">

                    <div class="card-icon">
                        🌐
                    </div>

                    <h3>
                        Conexão
                    </h3>

                    <p>
                        Mais pessoas e sistemas conectados.
                    </p>

                </div>

                <div class="card">

                    <div class="card-icon">
                        ⚙️
                    </div>

                    <h3>
                        Automação
                    </h3>

                    <p>
                        Tarefas mais rápidas e inteligentes.
                    </p>

                </div>

                <div class="card">

                    <div class="card-icon">
                        🧠
                    </div>

                    <h3>
                        Inteligência
                    </h3>

                    <p>
                        Dados transformados em decisões.
                    </p>

                </div>

                <div class="card">

                    <div class="card-icon">
                        🚀
                    </div>

                    <h3>
                        Oportunidades
                    </h3>

                    <p>
                        Novas formas de criar e inovar.
                    </p>

                </div>

            </div>

        </div>

    </section>

    <section class="slide">

        <div class="conteudo">

            <div class="tag">
                Solução de problemas
            </div>

            <h2>
                Tecnologia para
                <b>resolver problemas</b>
            </h2>

            <p>
                Inovar é encontrar maneiras melhores
                de resolver problemas reais.
            </p>

            <div class="fluxo">

                <div class="etapa">
                    🔎
                    <strong>
                        Problema
                    </strong>
                </div>

                <div class="seta">
                    →
                </div>

                <div class="etapa">
                    💡
                    <strong>
                        Tecnologia
                    </strong>
                </div>

                <div class="seta">
                    →
                </div>

                <div class="etapa">
                    🛠️
                    <strong>
                        Solução
                    </strong>
                </div>

                <div class="seta">
                    →
                </div>

                <div class="etapa">
                    📈
                    <strong>
                        Impacto
                    </strong>
                </div>

            </div>

        </div>

    </section>

    <section class="slide">

        <div class="ia-layout">

            <div class="conteudo">

                <div class="tag">
                    Inteligência Artificial
                </div>

                <h2>
                    Da informação à
                    <b>decisão</b>
                </h2>

                <ul class="lista">

                    <li>
                        Automatizar tarefas
                    </li>

                    <li>
                        Analisar grandes volumes de dados
                    </li>

                    <li>
                        Personalizar experiências
                    </li>

                    <li>
                        Apoiar decisões
                    </li>

                </ul>

            </div>

            <div class="cerebro">
                🧠
            </div>

        </div>

    </section>

    <section class="slide">

        <div class="conteudo visao">

            <div class="tag">
                Nossa visão
            </div>

            <h2>
                Criar tecnologia
                <b>com propósito</b>
            </h2>

            <blockquote>

                “Não basta criar algo novo.
                Precisamos criar algo que
                <b>faça diferença.</b>”

            </blockquote>

            <div class="conexao">
                👤 ───── 💻 ───── 🌎
            </div>

        </div>

    </section>

    <section class="slide slide-final">

        <div class="conteudo">

            <div class="tag">
                Próximo passo
            </div>

            <h1>
                O futuro
                <b>começa agora.</b>
            </h1>

            <div class="formula">
                Tecnologia + Pessoas + Criatividade = Futuro
            </div>

            <div class="frase-final">
                Imagine. Inove. Transforme.
            </div>

        </div>

    </section>

    <div class="navegacao">

        <button onclick="voltar()">
            ←
        </button>

        <button onclick="avancar()">
            →
        </button>

    </div>

    <script>

        const slides =
            document.querySelectorAll(".slide");

        let atual = 0;

        function mostrarSlide(indice) {

            slides.forEach(function(slide) {

                slide.classList.remove("active");

            });

            slides[indice]
                .classList.add("active");
        }

        function avancar() {

            atual++;

            if (atual >= slides.length) {
                atual = 0;
            }

            mostrarSlide(atual);
        }

        function voltar() {

            atual--;

            if (atual < 0) {
                atual = slides.length - 1;
            }

            mostrarSlide(atual);
        }

        document.addEventListener(
            "keydown",
            function(event) {

                if (event.key === "ArrowRight") {
                    avancar();
                }

                if (event.key === "ArrowLeft") {
                    voltar();
                }

            }
        );

    </script>

</body>

</html>
```
