# Prog_Conjunt
## El conjunt
Volem definir una classe anomenada Conjunt per a implementar una estructura per a simular el
comportament d’un conjunt https://es.wikipedia.org/wiki/Conjunto.  
En paraules nostres, anem a definir un conjunt com: - És una col·lecció d’elements de tamany ilimitat.
En aquesta pràctica anem a represenar un conjunt de enters - No importa l’ordre entre ells, és a dir, no
hi ha un primer, ni un consecutiu. - No poden haver-hi elements repetits
Son exemples de conjunts:  
- P = {6,13,1,7,14,5,9,11,8,2,4}
- Q = {12,3,7,5,16,8}
- R = {}
- T = {5,3,7}
Les operacions i mètodes que ha d’implementar el nostre Conjunt és:  
- **constructor un conjunt** → Es crearà el conjunt buit, aquell que no te elements.
- **constructor de còpia**, a partir d’altre conjunt ja creat.
- **constructor(int [])** a partir d’un array d’enters. Fixar-se que no poden haver elements
repetits. Cas de hi haure no odnarà error, però evitarà duplicats.not
- **size** → retorna el número d’elements del conjunt. Per exemple Q.size()=6
- **contains(element)** → retorna un boolean indicant si l’element pertany o no al conjunt. Per
exemple Q.contains(8)= true, Q.contains(4)=false.
- **afegir(element)** → afig el element al nostre conjunt, cas de no estar ja. Retorna el número
d’elements del conjunt un cop afegit el nom element o el que tenia.
- **eliminar(element)** → elimina, cas d’estar el element. Retorna true si ha pogut eliminar-se o
false en cas contrari.
- **esBuit** → ens diu si el conjunt està buit. Retorna un booleà. Per exemple P.esBuit()=false,
R.esBuit()=true
- **equals(Conjunt)** → ens diu si un conjunt és igual o no respecte a altre donat
- **toString()** → el mostra per pantalla, separant els elements per comes i tancats entre claus.
- **unio(Conjunt)** → crea un nou conjunt amb tots els elements del primer i del que passem com
argument. Per exemple P.unio(Q)={6, 13, 1, 7, 14, 5, 9, 11, 8, 2, 4, 12, 3,
16}
- **interseccio(Conjunt)** → crea un nou conjunt amb els elements que pertanyen a els dos
conjnts. Per exemple P.interseccio(Q)={7,5,8}
- **diferencia(Conjunt)** → crea un noun conjunt amb els element que pertanyan al primer conjunt però no al segon, com si fora una resta. Per exemple P.diferencia(Q)
={6,13,1,14,9,11,2,4}
- **diferenciaSimetrica(Conjunt)** → crea un nou conjunt amb els elemnts que pertanyan al
primer conjunt però no al segon, afegint-li els que pertanyan al segon conjunt però no al primer.
P.diferenciaSimetrica(Q)={6,13,1,14,9,11,2,4,12,3,16}. De manera senzilla la
diferència simètrica és la unió menys la intersecció
- **inscrit(Conjunt)** → retorna un boolea quan el primer conjunt està dins del passat com a
argument, és a dir, quan tots els elements del conjunt pertanyen al segon conjunt també. Per
exemple T.inscrit(P)=true, Q.inscrit(P)=false, T.inscrit(Q)=true
