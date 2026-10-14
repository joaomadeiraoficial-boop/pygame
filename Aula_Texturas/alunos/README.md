# Atividade 3 — Cubo com Satélite Texturizado

**Disciplina:** Computação Gráfica  
**Atividade:** Cubo com Satélite Texturizado — Texturas  
**Integrante:** João Alberto Madeira Soares Filho  
**Modalidade:** Individual

## Descrição

Nesta atividade, utilizei a textura `mosaico.png` no cubo principal e a textura `grade_uv.png` no satélite, configurada com `repeatUV = [2,2]`. O satélite foi adicionado como filho do cubo principal, a uma distância de `1.3` unidade e com escala de `0.4`. Ele acompanha o movimento do cubo principal e gira em torno do próprio eixo X, enquanto as setas controlam a velocidade da rotação principal.

## Resposta da questão conceitual

As coordenadas UV determinam como uma imagem bidimensional é aplicada na superfície de um objeto tridimensional. A coordenada U indica a posição horizontal na textura, e a coordenada V indica a posição vertical. Ao usar `repeatUV = [2,2]`, a textura é repetida duas vezes em cada direção, formando um padrão de quatro repetições na superfície, em vez de ser exibida uma única vez.

## Controles

- **↑ / ↓:** aumentam e diminuem a velocidade do cubo principal.
- **S:** salva a captura de tela.
- **Esc:** fecha o programa.

## Execução

Abra um terminal dentro desta pasta `alunos/`:

```powershell
py -3.12 -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe atividade_cubo.py
```

## Captura do resultado

![Cubo com Satélite Texturizado](capturas/resultado.png)
