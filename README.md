# imersao-alura-gemini
projeto criado para a Imersão Alura Gemini

# Sistema de Agentes para Respostas Infantis

Este projeto é um sistema baseado em agentes que utiliza modelos de linguagem grandes (LLMs) e ferramentas de busca para ajudar pais, responsáveis e educadores a gerar respostas adequadas e didáticas para as perguntas curiosas de crianças entre 3 e 12 anos.

## Sobre o Projeto

O objetivo principal deste sistema é facilitar a comunicação sobre tópicos variados com crianças, fornecendo respostas que considerem a faixa etária e sejam fáceis de entender. Ele funciona através de uma sequência de agentes:

1.  **Agente Buscador:** Pesquisa informações relevantes na internet sobre o tema da pergunta.
2.  **Agente Planejador:** Com base nas informações encontradas, planeja a estrutura e o conteúdo da resposta, adaptando a linguagem para a idade da criança.

**(Observação: O código fornecido inclui apenas o Buscador e o Planejador. Se você tiver agentes adicionais como Redator ou Revisor, lembre-se de mencioná-los aqui e na seção de "Como Funciona").**

## Funcionalidades

*   Recebe a idade da criança e o tópico da pergunta como entrada.
*   Utiliza a busca do Google para encontrar informações atualizadas sobre o tópico.
*   Gera um plano de resposta considerando a idade da criança e a complexidade do assunto.
*   Apresenta os resultados de cada etapa do processo (busca e planejamento) no notebook.

## Como Configurar e Executar

Para rodar este notebook, você precisará ter o Python e o Jupyter Notebook (ou Google Colab) instalados, além de uma API Key do Google Gemini configurada.

1.  **Obtenha uma API Key do Google Gemini:** Siga as instruções na documentação oficial do Google AI para obter sua chave de API.
2.  **Configure sua API Key:** No ambiente do Google Colab, você pode usar a ferramenta `userdata.get('GOOGLE_API_KEY')` para carregar sua chave de forma segura. Se estiver rodando localmente em um Jupyter Notebook, você precisará configurar a variável de ambiente `GOOGLE_API_KEY` com sua chave.
3.  **Instale as dependências:** Execute as células do notebook que contêm os comandos de instalação
4.  **Execute as células do notebook:** Siga a ordem das células para configurar o cliente Gemini, definir os agentes e executar a lógica principal do sistema.
5.  **Interaja com o sistema:** Quando solicitado, insira a idade da criança e a pergunta no formato `idade anos tema` (por exemplo: `6 anos De onde vêm os bebês`).

## Estrutura do Código

O código está organizado em células no notebook, incluindo:

*   Instalação de bibliotecas (`google-genai`, `google-adk`).
*   Configuração da API Key do Google Gemini.
*   Configuração do cliente da SDK do Gemini.
*   Testes iniciais com o modelo Gemini (com e sem busca).
*   Definição de funções auxiliares (`call_agent`, `to_markdown`).
*   Definição da classe/função para o Agente Buscador (`agente_buscador`).
*   Definição da classe/função para o Agente Planejador (`agente_planejador`).
*   A lógica principal que coordena a execução dos agentes e processa a entrada do usuário.

## Contribuições

Contribuições são bem-vindas! Se você tiver sugestões de melhorias, correções de bugs ou novas funcionalidades, sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

## Contato

Se você tiver alguma dúvida ou sugestão, pode entrar em contato pelo meu perfil no GitHub.
