# 21
from random import sample


def creadorBaraja (): return sample([(x,y) for x in [2,3,4,5,6,7,8,9,10,'J','Q','K','A'] for y in ['DIAMANTE','TREBOL','PICAS','CORAZONES']],52)

def repartir(): pass

def repartirIni(mazo,casa,jugador): 
    if casa != [] and len(casa)<3:
        print("casa",casa[-1])
        print("jugador", jugador[-1])
    if len(mazo)>2:
        repartirIni(mazo[2:],casa+[mazo[0]],jugador+[mazo[1]])

def repartir(mazo,casa,jugador):
    



repartirIni(creadorBaraja(),[],[])
