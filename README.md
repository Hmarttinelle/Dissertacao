# Análise e dimensionamento de elementos estruturais em betão armado

Este repositório contém o documento da dissertação associado ao desenvolvimento de uma aplicação **M.J. Structural Tools**.

## Resumo

A presente dissertação tem como objetivo o desenvolvimento de uma ferramenta computacional de apoio ao dimensionamento de elementos estruturais em betão armado, nomeadamente vigas, pilares e sapatas isoladas, em conformidade com o Eurocódigo 2.

Para esse efeito, foram formulados e implementados algoritmos de cálculo para cada um destes elementos estruturais, incorporando procedimentos iterativos que permitem obter soluções, construtivamente adequadas e otimizadas. Os modelos teóricos foram traduzidos para uma aplicação web desenvolvida em Python com recurso à framework Django, capaz de realizar o dimensionamento automático, gerar memórias de cálculo detalhadas e apresentar representações gráficas das soluções obtidas.

A fiabilidade da aplicação foi avaliada através de testes unitários automatizados e da comparação com exemplos de referência da literatura técnica, permitindo confirmar a coerência dos resultados produzidos. O trabalho desenvolvido demonstra, assim, a viabilidade da utilização de ferramentas computacionais no apoio ao dimensionamento estrutural, contribuindo para a digitalização e sistematização de procedimentos de cálculo em betão armado.

**Palavras-chave:** Betão Armado; Eurocódigo 2; Dimensionamento Estrutural; Algoritmos; Python; Django; SVG; Validação Computacional.

## Aplicação Web e Código Fonte

A aplicação web mencionada no resumo, desenvolvida em Python e Django para a realização dos cálculos estruturais e geração dos relatórios gráficos e analíticos, encontra-se armazenada num repositório independente.

* **Código Fonte da Aplicação:** [https://github.com/Hmarttinelle/Tese_Final.git](https://github.com/Hmarttinelle/Tese_Final.git)
* **Aplicação Online (Live Demo):** [https://pv27108.pythonanywhere.com/](https://pv27108.pythonanywhere.com/)

### Como Correr a Aplicação Localmente

Para executar a aplicação web no seu computador, deverá obter o código fonte no repositório indicado acima e seguir as instruções padrão de um ambiente Django. De forma geral, os passos resumem-se a:

1. **Clonar o repositório da aplicação:**
   ```bash
   git clone https://github.com/Hmarttinelle/Tese_Final.git
   cd Tese_Final
   ```

2. **Criar e ativar o ambiente virtual (Recomendado):**
   ```bash
   python -m venv venv
   # No Windows:
   venv\Scripts\activate
   # No Linux/Mac:
   source venv/bin/activate
   ```

3. **Instalar as dependências (Requirements):**
   ```bash
   pip install -r requirements.txt
   ```

4. **Aplicar as migrações à base de dados:**
   ```bash
   python manage.py migrate
   ```

5. **Iniciar o servidor de desenvolvimento:**
   ```bash
   python manage.py runserver
   ```
Após estes passos, a aplicação estará disponível e a correr no seu browser em `http://127.0.0.1:8000/`.
