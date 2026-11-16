### MyBread

#### Context

L’idea d’aquest projecte es poder digitalitzar un Fleca. Volem crear una tecnología que faciliti la feina dels treballadors, millori l'experiència dels clients i ajudi a vendre més evitant el desperdici d’aliments.

Actualment en una fleca tradicional podem trobar diferent problemes relacionats amb l’organització de les comandes, el control dels productes, l’atenció al client i la gestió de les vendes.

##### Problemes que volem solucionar

Farem una proposta ràpida de problemes i solucions que podem donar

**Cues al comprar el pa** → Comandes anticipades i recollida, poden per exemple programar el pa cada dia a la mateixa hora

**Control de stock** → Crear un cataleg amb disponibilitat dels productes
n
**Es tira el pa a final del dia** → Ofertes d’última hora

**Les comandes van amb paper i boli** → Fer un sistema centralitzat amb la gestió de les comandes, per tindre un ordre

**S’ha de controlar l’inventari manualment** → Una gestió digital de l'estoc

**Clients que compren sempre el mateix** → Un sistema amb “comandes preferides” i recurrents, tenir un perfil dels clients amb registre de què demanen i a quines hores. També pot ajudar a fer més d’aquell producte, a posar més personal a determinades hores o a anar més ràpid alhora d’atendre

**Pot costar analitzar les vendes que es fan** → Un panell amb estadístiques, com a l’anterior, es pot ajudar a fer estadístiques sobre que compren més, a quines hores…

Amb MyBread volem solucionar aquest problemes amb una plataforma digital que conecti amb els clients i els treballadors i faciliti la gestió del negoci.




#### Abast

##### Que proposem

**Una botiga online:**

Proposem fer una botiga online, tant web com aplicació que aparegui un catàleg amb fotografíes dels productes, i on el client (i preparat també per a la gent gran, que son els principals clients del pà a primera hora) puguin de manera intuitiva el pa, l’hora de recollida i si pagar online o a botiga.

**Gestió interna:**

Fer un panell privat per als treballadors. Aquest panell estaria posat als ordinadors de la fleca, i permetria als treballadors veure comandes pendents, control·lar les existències restants, actualitzar els productes i consultar les vendes dels dies.

**Productes restants:**

A final de dia, els productes que no s’haguin venut, es poden vendre amb descompte, amb packs promoció, o ofertas d’última hora. Aixó es un programa qui et diu quins productes baixar i a quin preu. Pot arribar a estar conectat amb les estadístiques per a saber els productes que s’acaben de vendre a última hora i els que no, i baixar el necessari els que calguin.

**Fidelització:**

A la mateixa web / aplicació per a la botiga online, es pot afegir un programa de punts, cupons, descomptes al dia d’aniversari i recompenses per a clients habituals.

**Estadístiques:**

Tenir estadístiques de tot el que passi a la botiga. Poder veure les ventes del dia, quins productes s’han venut més, les hores de màxima demanda, i per exemple els productes que s’han perdut per fer de més.

**Recollida ràpida**:

El client quan fa la reserva del pa per exemple reb un codi QR, per quan vagi a la botiga a recollir la comanda, únicament calgui escanejar el codi, i treure la bossa préviament preparada, per anar molt més ràpid.

##### Objectius

Els nostres principals objectius son:

* Digitalitzar la gestió d’una panaderia
* Reduir els errors humans en les comandes i en l’inventari
* Millorar l'experiència de compra per al client
* Disminuir el desperdici d’aliments amb promocions al final de dia
* Modernitzar i reinventar un nou negoci de fleca, més modern i fàcil.

##### Arquitectura del sistema

[https\://www\.odoo.com/ca\_ES](https://www.odoo.com/ca_ES)

S’ha de tindre 2 web, una al núvol per tota la part frontend i una en local per a tota la part backend, que es connectin.

**FRONTEND \- Web per als clients**

HTML CSS

Aquesta part permetrà als clients consultar els productes, fer comandes online i gestionar les seves reserves

**BACKEND- Logística del projecte**

Amb això farem la gestió interna, les comandes i la connexió amb la base de dades.

**Base de dades**

MySQL: Clients, Productes, Comandes i Stock

També s’ha d’afegir seguretat, copias de seguretat diàries, protegir les contrasenyes, i un sistema de permisos per als treballadors i l’administrador.
