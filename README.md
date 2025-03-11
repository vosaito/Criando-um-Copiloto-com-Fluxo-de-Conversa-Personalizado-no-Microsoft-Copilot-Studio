
# Resumo do aprendizado - Microsoft Copilot Studio
#### *Criando um Copiloto com Fluxo de Conversa Personalizado no Microsoft Copilot Studio*

## Objetivo:
Criar um resumo das aulas e desafio de projeto que foram ministrados até o momento, com o intuito de compilar e fixar as informações aprendidas.
## Conteúdo das aulas (arquivos .txt em anexo):
- Tópicos;
- Entidades e Variáveis;
- Respostas Generativas.

## Resumo do desafio de projeto
### Projeto de criando um copilot com fluxo de conversa personalizado
### Criação do agente

Importante: deixar a linguagem do agente como Inglês(US), pois atualmente as respostas generativas estão disponíveis apenas em inglês. Porém ainda é possível escrever os prompts e descrições em português, mesmo estando na lingua inglesa.\
Para o prompt, é importante que escreva de forma claro, detalhada e mais direta possível. Ideal que estude sobre engenharia de prompts.\
Para esse exemplo, uma boa prática de construção de prompt, foi escrito da seguinte forma:
- Identificar o agente, identificamos "Agente da DIO";
- Definir o tom das respostas do agente, foi definido como formal;
- Definir o que o agente irá fazer ou ser responsável, foi definido para ele retornar informações relevantes sobre Microsoft Copilot Studio;
- Definir uma fonte de conhecimento, definido como documentação oficial da Microsoft;
- Pode também ser definido pontos para considerar em seus retornos, como buscar a melhor resposta, retornar de forma apropriada, amigável em tom formal, retornar pelo menos uma citação.
Essa parte de criação, é possível definir que o agente possa ser parte de uma solução existente em um ambiente.\
Na criação, não precisamos ser detalhado/preciso com relação aos tópicos, ações e plugins até fontes de conhecimento. É importante descrever bem o que espera que ele faça, pois assim o agente é criado já prevendo o que deve ter para executar o que foi descrito, assim poderá poupar tempo de configuração, mas ainda é importante se verifique todas as configurações para que não haja falhas ou comportamentos indesejados.

### Customizando o agente

Após a criação do agente, podemos customizar dele conforme desejar para que ele se comporte da maneira que espera.

#### Criação/customização de tópicos

#### Customizando para gerar respostas generativas
Adicionar o "Create generative answers" para que ele retorne uma resposta gerada por IA. Nessa etapa é preciso que ele considere a mensagem do usuário, ativando a "Activity.text". Assim garantimos que ele retorne uma resposta com base na pergunta do usuário.

#### Customizando mensagens de erro 
Também é possível customizar as mensagens de erro de um tópico, em "conversational boosting" e em "fallback".\
Erro em "Conversational boosting", é quando o agente não encontra uma resposta nas fontes de conhecimento. Por padrão, o agente retorna uma mensagem genérica como erro. Podemos personalizar escrevendo uma mensagem, informando o erro e o motivo, e até formas de contato para tentar resolver o problema do usuário.
