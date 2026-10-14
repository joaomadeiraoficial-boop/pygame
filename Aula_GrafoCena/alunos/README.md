# Atividade 2 — Braço Robótico

**Disciplina:** Computação Gráfica  
**Atividade:** Braço Robótico — Grafo de cena  
**Integrantes:** João Alberto Madeira Soares Filho e **[NOME COMPLETO DO SEGUNDO INTEGRANTE]**  

## Descrição da solução

Construímos um braço robótico tridimensional usando objetos organizados em uma hierarquia. A base é cinza, o braço é laranja, o antebraço é azul e a garra é cinza. Para representar as articulações, usamos pivôs `Object3D` no ombro e no cotovelo. Com isso, cada parte acompanha o movimento da articulação à qual está ligada, e os controles permitem movimentar o robô pelo teclado.

## Resposta da questão conceitual

Os pivôs foram necessários porque as caixas são criadas com seu centro na origem local. Se girássemos diretamente o braço e o antebraço, eles rodariam em torno do centro das caixas, e não no ponto correto das articulações. Os pivôs ficam no ombro e no cotovelo e permitem fazer a rotação nesses pontos. Além disso, a hierarquia garante que as partes filhas acompanhem os movimentos das partes às quais estão conectadas.

## Como executar

Abra o terminal nesta pasta `alunos` e execute:

```powershell
py -3.12 -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe atividade_braco.py
```

**Controles:** A/D giram a base; W/S movimentam o ombro; I/K movimentam o cotovelo; P salva a captura; Esc fecha.

## Captura de tela

![Resultado do Braço Robótico](capturas/resultado.png)

> Registre o braço dobrado durante a execução, pressionando P.
