# Atividade 1 — Mini Sistema Solar

**Disciplina:** Computação Gráfica  
**Atividade:** Mini Sistema Solar — Transformações geométricas  
**Integrantes:** João Alberto Madeira Soares Filho e **[NOME COMPLETO DO SEGUNDO INTEGRANTE]**  

## Descrição da solução

Nesta atividade, usamos transformações geométricas com matrizes para representar um pequeno sistema solar em 2D. O Sol gira em torno do próprio centro, enquanto um planeta realiza uma órbita ao seu redor e também gira sobre seu eixo. A Lua acompanha o movimento do planeta e possui uma órbita própria. As velocidades são atualizadas com `deltaTime`, e as setas permitem aumentar ou diminuir a velocidade orbital sem deixá-la negativa.

## Resposta da questão conceitual

A órbita usa `R @ T` porque primeiro deslocamos o planeta para a distância escolhida do Sol e depois giramos essa posição em torno da origem. Como as operações são aplicadas da direita para a esquerda, a translação acontece antes da rotação orbital. A rotação própria do planeta fica à direita da translação para ser aplicada enquanto ele ainda está em sua origem local. Assim, o planeta gira em torno do próprio centro sem mudar a distância de sua órbita.

## Como executar

Abra o terminal nesta pasta `alunos` e execute:

```powershell
py -3.12 -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe atividade_sistema_solar.py
```

**Controles:** ↑ aumenta a velocidade; ↓ diminui; P salva a captura; Esc fecha.

## Captura de tela

![Resultado do Mini Sistema Solar](capturas/resultado.png)

> A imagem deve ser capturada durante a execução, pressionando P.
