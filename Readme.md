
# GRAFO DE FLUXO

![image](https://github.com/WesleyAndradi/Caixa-Branca/assets/80072933/e4034c71-08d6-4129-b21e-1aa10f7042dc)


## Complexidade ciclomática
A complexidade ciclomática se resume em possibilidades diferentes que o gráfico tem de completar seu percurso, sendo calculado com:

C = A - N + 2
(Arestas - nós + 2)

26 arestas - 24 nos = 2 + 2 = 4 (caminhos possíveis)

sendo eles:

Caminho 1: 1-2-3-4-5-6-7-10-11-12-13-14-15-16-17-18-19-20-23-24
Todos o caminho ocorre normalmente sem nenhum problema

Caminho 2: 1-2-3-4-5-8-9-10-11-12-13-14-15-16-17-18-19-20-23-24
Por este caminho o "conectarBD" gera uma excessão e verificar usuario funciona normalmente

Caminho 3: 1-2-3-4-5-6-7-10-11-12-13-14-15-21-22-23-24
Uma excessão ocorre em "verificarUsuario"

Caminho 4: 1-2-3-4-5-8-9-10-11-12-13-14-15-16-20-23-24
Usuário não encontrado
