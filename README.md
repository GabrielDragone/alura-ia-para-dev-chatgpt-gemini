# alura-ia-para-dev-chatgpt-gemini
IA para Dev: Desenvolvendo Códigos com ChatGPT, Grok, Claude e Gemini

https://cursos.alura.com.br/course/ia-para-dev-chatgpt-gemini

# 01. Geração de Código:
## 01 - Apresentação:
* A ideia do curso não é ensinar o básico que já sabemos, é ir um pouco além, mostrando como podemos usar essas IAs para acelerar o desenvolvimento de software.

## 02 - Preparando o ambiente:
* Utilizar o projeto LLM para facilitar: https://github.com/alura-cursos/5185-Desenvolvendo-e-Otimizando-Codigos-LLMs

## 03 - Usando o jeito tradicinal:
* Site para testarmos códigos: https://codepen.io/pen/
* Geralmente fazemos solicitação, correção da solicitação e assim por diante até conseguirmos acertar o código que queremos.
* Dentro das ferramentas IA, existe um lugar que faz isso de maneira mais efetiva.

## 04 - A lousa ChatGPT e Canva do Gemini:
* Em ambas as IAs, se formos em + e procurarmos as opções, teremos a opção de Lousa (ChatGPT) e Canva (Gemini).
* Essas opções nos permitem trabalhar de uma maneira diferente. O prompt enviado é entendido de forma diferente.
* Conseguimos editar, realizar prévia dessa lousa/canvas e até executar o código.
* Essa ferramenta foi pensada exatamente para desenvolvedores utilizarem.

## 05 - Para saber mais: Construindo bons prompts:
* Tão importante quanto escolher a ferramenta de Inteligência Artificial e definir o modelo LLM é saber como instruir a IA para realizar uma tarefa. 
* E não se trata apenas de ser específico ou dar contexto, embora isso seja essencial. Existem também técnicas de prompting que ajudam a esclarecer como algo deve ser feito, qual formato deve ser retornado, qual linha de raciocínio ou cadeia de passos a IA deve seguir ao elaborar uma resposta, entre outros aspectos.
* Um bom prompt é o primeiro passo para uma boa resposta. Quanto mais clara for a sua instrução, mais precisos e úteis serão os resultados gerados pela IA.
* Para saber mais:
  * https://www.alura.com.br/artigos/engenharia-prompt
  * https://www.alura.com.br/curso-online-engenharia-prompt-criando-prompts-eficazes-ia-generativa

## 06 - Inovando com ferramentas de desenvolvimento colaborativo:
* Pergunta:
  * A empresa fictícia Fokus, tem a ideia de um aplicativo para aumentar a produtividade utilizando a técnica Pomodoro, e está buscando maneiras de melhorar seu processo de desenvolvimento. Considerando as capacidades das ferramentas de desenvolvimento colaborativo, qual abordagem a equipe pode adotar para otimizar seu fluxo de trabalho e quais desafios podem surgir?
* Resposta:
  * Integrar a Lousa do ChatGPT e o Canvas do Google Gemini no fluxo de trabalho diário, permitindo colaboração em tempo real na criação e teste de novas funcionalidades, e realizar treinamentos para garantir que todos estejam familiarizados com as ferramentas.
  * Correta, pois essa abordagem permite que a equipe colabore de forma eficaz, prototipando ideias rapidamente e visualizando resultados sem ambientes complexos, enquanto os treinamentos ajudam a superar o desafio da familiarização com as ferramentas.

## 07 - Otimizando respostas de consultas culinárias:
* Pergunta:
  * A EasyFood, uma plataforma digital que oferece um clube de vantagens e recompensas personalizadas por meio de parcerias com diversas empresas, está desenvolvendo uma nova funcionalidade para recomendar receitas culinárias baseadas nos ingredientes que as pessoas usuárias têm em casa. A equipe de desenvolvimento decidiu explorar quatro ideias diferentes de layout para a tela inicial dessa nova funcionalidade. No entanto, criar protótipos detalhados para todas as opções levaria tempo e atrasaria a validação com as pessoas usuárias. Qual estratégia a equipe pode adotar para prototipar essas ideias de forma mais rápida e eficiente?
* Resposta:
  * Utilizar ferramentas de IA como ChatGPT Lousa ou Canva do Gemini para gerar rapidamente protótipos de baixa fidelidade, permitindo que a equipe compare ideias visuais em minutos antes de investir em refinamentos detalhados.
  * Correta, pois essa abordagem acelera o processo criativo, favorece a experimentação ágil e garante que apenas as ideias mais promissoras avancem para protótipos de maior fidelidade.

## 09 - Criando resumos com o NotebookLM:
* Uma ferramenta de IA do Google que nos ajuda a sintetizar e organizar as ideias centrais de cada etapa do curso.
* Funciona com base nas informações que nós fornecemos, então ele se torna especialista nessas informações.
* Resumir seus textos: Transformar anotações longas em resumos práticos. 
* Responder perguntas: Tirar dúvidas com base exclusiva nos seus documentos. 
* Gerar novas ideias: Criar roteiros de estudo, glossários ou fazer um brainstorming sobre seus próprios projetos.
* https://notebooklm.google.com/


# 02. Da demanda a Protótipo:
## 01 - Explorando a Lusa do ChatGPT:
* Criação de tela de feedback pós compra de acordo com documentação de demanda.
* Evitar utilizar o mesmo contexto de conversa que foi utilizado para outro cenário.
* Na parte inferior direita do ChatGPT, existe um botção de revisão de código, onde podemos portar linguagem, corrigir bugs, adicionar registros ou comentários.

## 02 - Explorando o Canva do Gemini:
* Prompt:
  * ```
    Crie uma tela usando HTML, CSS e Javascript.
    Essa tela deve conter:
    - Um titulo "Avalie sua compra"
    - Um campo para digitar um comentário.
    - Um botão para enviar.
    - Um slider interativo com 3 pontos: Se o slider ficar no ponto inicial, o fundo da tela deve ser verde, se ficar no meio, amarelo, no ultimo vermelho. Cada vez que o usuário mover o slider a tela deve mudar de cor com uma animação suave.
    - Aoós o envio do comentário, ele deve ser exibido em tela junto de uma mensagem de agradecimento pelo Feedback.
    ```
* Código:
  * [exemplo-02-02-gemini.html](exemplo-02-02-gemini.html)
* Também existem opções no canto inferior direito, porém um pouco diferentes, como opções de selecionar e perguntar e adicionar recursos do gemini dentro do código (aqui no exemplo do HTML, foi adicionado um botão de melhorar texto e quando o comentário é enviado, a gente memde o nível de satisfação para o Gemini melhorar o texto do comentário).
* Existe um prompt que é passado pro Gemini para ele entender o contexto do que está sendo feito:
  * ```
    const systemPrompt = "Você é um assistente de escrita. Sua tarefa é reescrever o feedback de um cliente para torná-lo mais claro, educado e gramaticalmente correto, mantendo o sentimento original. Responda APENAS com o texto melhorado em português.";
    ```
* Também temos opções de retornar versões de histórico.

## 03 - Refatorando código e histórico:
* Dentro do Gemini, quando reaalizamos a verificaçãao do Código, podemos selecionar o trecho que queremos refatorar e pedir pro Gemini alterar o mesmo através de um novo prompt. Modifica o código diretamente. Experiencia mais fluida.
* No ChatGPT temos algo similar, onde podemos selecionar o trecho e pedir para melhorar o código. Deixa a visualização como um DIff, parecido com Pull Request. Melhor versionamento.

## 04 - Criando uma tela de feedback:
* Pergunta: A Hermex Log, empresa de logística especializada em entregas, decidiu criar uma tela de feedback para que os clientes avaliem o serviço. A tela deve permitir escolher entre "boa", "regular" ou "ruim", mudar a cor de fundo conforme a escolha e exibir uma mensagem de agradecimento após o envio.
  Durante o desenvolvimento, a equipe percebeu que usava o mesmo chat de IA para assuntos distintos, como prazos de entrega e a tela de feedback, o que gerava respostas confusas. O que a equipe deve fazer para garantir que a IA compreenda apenas a demanda atual e não misture contextos anteriores?
* Resposta: Abrir sempre um novo chat ao iniciar uma demanda, garantindo que apenas o contexto atual seja considerado pela IA. Correta, pois ao limpar o histórico e começar um chat dedicado, evita-se mistura de contextos e aumenta a precisão das respostas.

## 05 - Melhorando a coleta de feedback n Meteora:
* Perguntaa: A Meteora, uma loja online de roupas e acessórios, está desenvolvendo um código de lógica para calcular descontos em compras. Durante os testes, um membro da equipe selecionou todo o código e pediu ao Gemini para “reescrever tudo de forma mais simples”. O resultado foi uma versão que perdeu parte das regras de negócio, como a aplicação correta do desconto progressivo por quantidade de itens. O que esse caso mostra sobre os riscos de usar a função de edição de forma indiscriminada?
* Resposta: Que, para ajustes pontuais, selecionar todo o código e pedir alterações específicas não faz sentido e pode gerar a perda de regras importantes. Correta, pois o uso indiscriminado da edição amplia o escopo da alteração e compromete trechos que não precisavam ser modificados.

## 06 - Resumo com NotebookLM:
* Velocidade: Do conceito ao protótipo funcional em tempo recorde.
* Eficiência: Automatiza código repetitivo, focnado na lógica complexa.
* Prototipagem Rápida: Permite iteração e testes rápidos de ideias.
* Acessibilidade: Reduz a barreira para implementar novos recursos.
* Precisão: Refatoração assistida por IA minimiza o risto de novos bugs.
* Nova forma de construir software, com colaboração entre humanos e IAs.