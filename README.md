# Jogo Quizz

Quiz de conhecimentos gerais jogado no terminal.

Projeto desenvolvido para fins acadêmicos (cadeira de Programação I).

## Funcionalidades

- **Banco de perguntas:** 27 perguntas de múltipla escolha, com 5 alternativas cada, em `perguntas.json`.
- **Partidas:** cada partida tem 5 perguntas sorteadas.
- **Pontuação por dificuldade:** fácil vale 10 pontos, médio vale 20 e difícil vale 30.
- **Registro de jogadores:** ao final, o nome e a pontuação são salvos em `player.json`.

## Tecnologias

- <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="20" alt=""> Python 3
- JSON (armazenamento das perguntas e dos resultados)

## Como executar

É necessário ter o Python 3. O projeto não usa bibliotecas externas.

Clone o repositório:

```bash
git clone https://github.com/samuelsouza-dev/projetoprog1.git
```

Entre na pasta do projeto, pois o jogo procura `perguntas.json` na pasta atual:

```bash
cd projetoprog1
```

Inicie o jogo:

```bash
python quizzprog1.py
```

## Como jogar

1. Digite seu nome.
2. Responda digitando o código exato da alternativa: `alt1`, `alt2`, `alt3`, `alt4` ou `alt5`.
3. Depois de 5 perguntas, sua pontuação é exibida e uma nova partida começa.
4. Para sair, pressione `Ctrl+C`.

## Limitações conhecidas

- **Respostas exatas:** qualquer resposta diferente do código da alternativa correta, como `2` ou `ALT2`, conta como erro.
- **Perguntas repetidas:** a verificação de repetição tem falhas, então a mesma pergunta pode aparecer mais de uma vez na partida.
- **Formato do `player.json`:** os resultados são acrescentados um após o outro, então o arquivo deixa de ser um JSON válido a partir da segunda partida.
