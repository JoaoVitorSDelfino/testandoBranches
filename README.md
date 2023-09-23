![image](https://github.com/JoaoVitorSDelfino/testandoBranches/assets/103132209/75403950-a176-4786-bdab-a91d99910ed4)# Avaliação Sprint 1 - Programa de Bolsas Compass UOL / AWS e UTFPR

***

## Como utilizar

__Primeiro passo__ - Abrir o arquivo index.html, localizado na pasta src

__Segundo passo__ - Digitar um número de quatro digitos qualquer na caixa de texto

__Terceiro passo__ - Apertar o botão "Enviar"

<img width="450" alt="imagemSistemas" src="https://github.com/JoaoVitorSDelfino/gitTreino/assets/103132209/0b788368-e94d-4a1a-82e0-031d54d00411">
<img width="450" alt="imageSistema" src="https://github.com/JoaoVitorSDelfino/testandoBranches/assets/103132209/dcab97e9-8236-48dd-9f67-4da159167ff6">


***

## Funcionamento
- O sistema gera um número PIN randômico, entre 0000 e 9999
- O usuário informa um número qualquer de 4 digitos e recebe uma resposta
- Há três tipos de respostas
  - Acerto (verde): Quando o usuário acerta o PIN
  - Erro (laranja): Quando o usuário não acerta o PIN
    - *Muito menor =  numeroDigitado < (numeroResposta - 150)*
    - *Menor = (numeroResposta - 150) ≤ numeroDigitado <  numeroResposta*
    - *Muito maior = numeroDigitado > (numeroResposta + 150)* 
    - *Maior = (numeroResposta + 150) ≥ numeroDigitado > numeroResposta*
  - Entrada inválida (vermelho): Quando o valor informado pelo o usuário 
    - Valores string como "bom dia"
    - Valores negativos como "-2131"
    - Valores com mais/menos que 4 digitos como "123"

***

## Desenvolvimento
1. Iniciei o projeto desenvolvendo a parte frontend do programa, o index.html e style.css
2. Desenvolvi a parte de javascript, contendo funções básicas como:
    - Criar de um PIN estático (3636);
    - Verificar se o valor digitado é realmente um número;
    - Oferecer feedback de quão perto o usuário está de acertar o PIN;
3. Após as implementações básicas, foi desenvolvido funções mais avançadas:
    - Verificar se o valor digitado não é nulo, possui 4 digitos e não é negativo;
    - Substituição do PIN estático por um gerado aleatoriamente;
4. Pequenos fixes envolvendo lógica
5. Pequenas modificações e otimizações envolvendo a interface (.css)
6. Criação da documentação (README.md e commits)
7. Envio da branch para o repositório remoto

***

## Dificuldades
Tive certa dificuldade na hora de definir um limite para quando se deve mostrar uma mensagem de quão perto o usuário estava de acertar o PIN. Primeiro tive a ideia de criar limites baseados em uma fração do número, entretanto era imprático para números muito grandes e aqueles que chegavam muito perto dos limites (0000 e 9999). Por fim, optei por utilizar um limite estático de 150

Tive problemas também em relação aos commits, estava com um pouco de dúvida se os meus commits estavam seguindo o padrão semântico mostrado, mas com um pouco a mais de pesquisa fui capaz de resolver o problema.
