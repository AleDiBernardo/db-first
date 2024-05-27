
# Traccia
Modellizzare la struttura di una tabella per memorizzare tutti i dati 
riguardanti delle auto usate messe in vendita da un concessionario


## Tabella: AutoUsate

| Colonna           | Tipo di Dato                                                       | 
|-------------------|--------------------------------------------------------------------|
| AUTO_ID           | unsigned int, auto_increment, primary key                          |  
| MARCA             | varchar(50)                                                        | 
| MODELLO           | varchar(50)                                                        | 
| ANNO              | year                                                               | 
| COLORE            | varchar(20)                                                        | 
| CHILOMETRAGGIO    | unsigned int                                                       | 
| PREZZO            | decimal(10, 2)                                                     | 
| NUM_TELAIO        | varchar(50)                                                        | 
| PROPRIETARIO_ID   | int foreign key                                                    | 
| CARBURANTE        | enum('diesel', 'benzina', 'elettrica', 'metano', 'ibrida', 'gpl')  | 
| CAMBIO            | enum('automatico', 'manuale', 'semi-automatico')                   | 

**PS: ho usato quel poco di rimasuglio delle superiori per enum e la foreign key**
