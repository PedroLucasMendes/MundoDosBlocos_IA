# :hammer_and_wrench: MundoDosBlocos_IA
Trabalho 1 da disciplina de Inteligência Artificial - UFAM

| Integrantes |
|:-------:|
| **Alcir Heber** |
| **Maria Luiza** |
| **Pedro Lucas** |

## :books: Sobre o projeto

Este programa em Prolog é um planejador para o domínio do Mundo dos Blocos, onde blocos podem ser movidos entre posições (lugares) com base em certas regras. O Mundo dos Blocos é 
representado por um conjunto de predicados descrevendo o estado atual do mundo, ações que podem ser realizadas e metas a serem alcançadas.

## :book: Como Executar passo a passo:

1. **Ambiente Prolog:**
   Certifique-se de ter um ambiente Prolog instalado. Este código foi testado no SWI-Prolog.

2. **Carregar o Código:**
   Abra seu ambiente Prolog e consulte/carregue o arquivo Prolog fornecido (por exemplo, `blocks_world.pl`).

3. **Definir o Estado Inicial**
   Descomente ou defina o estado inicial (state1 predicado) no arquivo Prolog com base no seu problema, conforme o exemplo abaixo.

4. **Definir metas**
   Defina as metas que você deseja alcançar (plan predicado) na área de consulta conforme o exemplo abaixo.

5. **Execute o planejador**


## :heavy_check_mark: Exemplo de Uso:

Aqui está um exemplo de como usar o planejador para um problema específico:

```prolog        
   %        c c c a b d
   %        -----------
   % place  1 2 3 4 5 6
  
   % definação do estado inicial
   state1([on(c,p([1,3])),on(a,b),on(b,p([5,5])),on(d,a),clear(c),clear(d),clear(4),clear(6)]).
```

```prolog
   % definação das metas
   state1(S) , plan(S, [on(a,c)], Plan).
```
















