# 21
from random import sample

def creadorBaraja ():
    return sample([(x,y) for x in [2,3,4,5,6,7,8,9,10,'J','Q','K','A'] for y in ['DIAMANTE','TREBOL','PICAS','CORAZONES']],52)

def repartir(mazo,casa,jugador):
    mazo[2:],casa+[mazo[0]],jugador+[mazo[1]]
    print (casa)
    

def repartirIni(mazo,casa,jugador):
    if casa != [] and len(casa)<3: 
        print("casa ", casa)
        print ("jugador ", jugador)
    if len(mazo)>2:
        jugar(mazo[2:],casa+[mazo[0]],jugador+[mazo[1]])

    if input("QUIERE OTRA CARTA Y/N")=='Y':
        repartir(mazo,casa,jugador)

def valorLetra():
    pass
    

def jugar(mazo,casa,jugador):
    repartirIni(mazo,casa,jugador)


jugar(creadorBaraja(),[],[])
