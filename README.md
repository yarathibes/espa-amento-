 <section class="slide active">

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

        <div class="icone">
            💻
        </div>

    </section>


    <!-- SLIDE 2 -->

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
                        Pessoas e sistemas cada vez mais conectados.
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


    <!-- SLIDE 3 -->

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
                A tecnologia pode transformar problemas
                em oportunidades.
            </p>

            <div class="fluxo">

                <div class="etapa">
                    🔎
                    <strong>Problema</strong>
                </div>

                <div class="seta">
                    →
                </div>

                <div class="etapa">
                    💡
                    <strong>Ideia</strong>
                </div>

                <div class="seta">
                    →
                </div>

                <div class="etapa">
                    🛠️
                    <strong>Solução</strong>
                </div>

                <div class="seta">
                    →
                </div>

                <div class="etapa">
                    📈
                    <strong>Resultado</strong>
                </div>

            </div>

        </div>

    </section>


    <!-- SLIDE 4 -->

    <section class="slide">

        <div class="ia">

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
                        Analisar dados
                    </li>

                    <li>
                        Criar experiências personalizadas
                    </li>

                    <li>
                        Ajudar nas decisões
                    </li>

                </ul>

            </div>

            <div class="cerebro">
                🧠
            </div>

        </div>

    </section>


    <!-- SLIDE 5 -->

    <section class="slide">

        <div class="conteudo">

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


    <!-- SLIDE 6 -->

    <section class="slide final">

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

            <div class="frase">
                Imagine. Inove. Transforme.
            </div>

        </div>

    </section>


    <div class="botoes">

        <button onclick="voltar()">
            ←
        </button>

        <button onclick="avancar()">
            →
        </button>

    </div>


    <script>

        const slides = document.querySelectorAll(".slide");

        let atual = 0;


        function mostrarSlide(numero) {

            slides.forEach(function(slide) {
                slide.classList.remove("active");
            });

            slides[numero].classList.add("active");
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


        document.addEventListener("keydown", function(event) {

            if (event.key === "ArrowRight") {
                avancar();
            }

            if (event.key === "ArrowLeft") {
                voltar();
            }

        });

    </script>

</body>

</html>
