
# Traccia
Modellizzare la struttura di una tabella per memorizzare tutti i dati 
riguardanti delle auto usate messe in vendita da un concessionario


## Tabella: AutoUsate

| Colonna           | Tipo di Dato                                                                 | 
|-------------------|------------------------------------------------------------------------------|
| AUTO_ID           | unsigned int, auto_increment, primary key                                    |  
| MARCA             | varchar(50), not null                                                        | 
| MODELLO           | varchar(50), not null                                                        | 
| ANNO              | year, not null                                                               | 
| COLORE            | varchar(20)                                                                  | 
| CHILOMETRAGGIO    | unsigned int, not null                                                       | 
| PREZZO            | decimal(10, 2), not null                                                     | 
| NUM_TELAIO        | varchar(50), not null                                                        | 
| PROPRIETARIO_ID   | unsigned int, foreign key                                                    | 
| CARBURANTE        | enum('diesel', 'benzina', 'elettrica', 'metano', 'ibrida', 'gpl'), not null  | 
| CAMBIO            | enum('automatico', 'manuale', 'semi-automatico'), not null                   | 

**PS: ho usato quel poco di rimasuglio delle superiori per enum e la foreign key**
