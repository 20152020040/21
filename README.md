# 21
from random import sample

def creadorBaraja ():
    return sample([(x,y) for x in [2,3,4,5,6,7,8,9,10,'J','Q','K','A'] for y in ['DIAMANTE','TREBOL','PICAS','CORAZONES']],52)

def repartir():
    pass

def repartirIni():
    pass

def jugar(mazo,casa,jugador,x):
    if casa != []:
        print(casa)
    if len(mazo)>2:
        jugar(mazo[2:],casa+[mazo[0]],jugador+[mazo[1]])


jugar(creadorBaraja(),[],[])

