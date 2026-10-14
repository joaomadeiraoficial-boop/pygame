# Computação Gráfica — Atividades Práticas

**Aluno:** João Alberto Madeira Soares Filho  
**Instituição:** UNIPAC Barbacena  
**Disciplina:** Computação Gráfica  
**Professor:** Rodrigo Fernandes dos Santos  
**Modalidade da entrega:** Individual

Este repositório reúne as três atividades práticas desenvolvidas na disciplina de Computação Gráfica com Python e OpenGL. A resolução foi feita a partir dos arquivos iniciais disponibilizados pelo professor, com foco nos trechos identificados como `TODO`.

## Atividades desenvolvidas

| Atividade | Conteúdo | Código | Explicação | Captura |
|---|---|---|---|---|
| 1. Mini Sistema Solar | Composição de matrizes e transformações geométricas | [Python](Aula_Transformacoes/alunos/atividade_sistema_solar.py) | [README](Aula_Transformacoes/alunos/README.md) | [Imagem](Aula_Transformacoes/alunos/capturas/resultado.png) |
| 2. Braço Robótico | Grafo de cena, pivôs e hierarquia | [Python](Aula_GrafoCena/alunos/atividade_braco.py) | [README](Aula_GrafoCena/alunos/README.md) | [Imagem](Aula_GrafoCena/alunos/capturas/resultado.png) |
| 3. Cubo com Satélite Texturizado | Texturas, coordenadas UV e transformações | [Python](Aula_Texturas/alunos/atividade_cubo.py) | [README](Aula_Texturas/alunos/README.md) | [Imagem](Aula_Texturas/alunos/capturas/resultado.png) |

Os README de cada atividade contêm sua descrição, os controles, a resposta à questão conceitual e o registro visual do resultado.

## Resumo das soluções

**Mini Sistema Solar:** uso de matrizes de rotação, translação e escala para animar o Sol, a órbita e a rotação do planeta e a órbita da Lua. As setas controlam a velocidade orbital, sem permitir valores negativos.

**Braço Robótico:** organização da base, do ombro, do cotovelo, do antebraço e da garra em um grafo de cena. Pivôs permitem movimentar as articulações com o teclado.

**Cubo Texturizado:** aplicação de texturas em dois cubos, configuração de repetição UV no satélite, associação hierárquica, movimento orbital e rotação própria.

## Tecnologias utilizadas

- Python 3.12
- Pygame
- PyOpenGL
- NumPy

O projeto requer uma placa de vídeo com suporte compatível ao OpenGL utilizado nas atividades.

## Como executar no Windows (VS Code)

Cada pasta `alunos/` contém seu próprio código e suas dependências. Abra um terminal dentro da pasta da atividade escolhida e execute:

```powershell
py -3.12 -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe atividade_sistema_solar.py
```

Substitua o nome do programa pelo arquivo correspondente: `atividade_braco.py` na segunda atividade ou `atividade_cubo.py` na terceira.

Para capturar os resultados durante a execução, use **P** no Sistema Solar e no Braço Robótico, e **S** no Cubo Texturizado.

## Material da disciplina e créditos

Este repositório é um **fork do projeto original** de [Rodrigo Fernandes dos Santos](https://github.com/rodrygofesantos/pygame), professor da disciplina. O framework, os arquivos de apoio, as demonstrações, as imagens e os enunciados das atividades são provenientes desse material didático.

As aulas utilizam como referência o livro *Developing Graphics Frameworks with Python and OpenGL*, de Lee Stemkoski e Michael Pascale (CRC Press, 2022).

Os enunciados originais estão disponíveis em [EXERCICIOS.md](EXERCICIOS.md) e nos arquivos `ATIVIDADE.md` das respectivas pastas. O restante do repositório, incluindo `core/`, demonstrações, checkpoints e `requirements.txt`, foi preservado para permitir a execução dos exercícios.
