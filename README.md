Esercizio di oggi: Primo DB
nome repo: db-first
Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

## "Parco Auto Concessionario" TABLE STRUCTURE

| FIELD            | TYPE         | ATTRIBUTES                                 | INDEXES     |
| ---------------- | ------------ | ------------------------------------------ | ----------- |
| id               | INT          | NOT NULL, UNSIGNED, UNIQUE, AUTO INCREMENT | PRIMARY KEY |
| constructor      | VARCHAR(30)  | NOT NULL                                   |             |
| model            | VARCHAR(100) | NOT NULL                                   |             |
| licensePlate     | CHAR(7)      | NOT NULL, UNIQUE                           | INDEX       |
| fuel             | VARCHAR(30)  | NOT NULL                                   |             |
| registrationDate | DATE         | NOT NULL                                   |             |
| gearbox          | VARCHAR(30)  | NULL, DEFAULT("MANUAL")                    |             |
| cost             | FLOAT(8,2)   | NULL, UNSIGNED                             |             |
| price            | FLOAT(8,2)   | NOT NULL, UNSIGNED                         |             |
| mileage          | MEDIUMINT    | NOT NULL, UNSIGNED                         |             |
| displacement     | SMALLINT     | NOT NULL, UNSIGNED                         |             |
| color            | VARCHAR(50)  | NULL                                       |             |
| door             | TINYINT      | NULL, default ("4")                        |             |
| parkingSlot      | TINYINT      | NOT NULL, UNSIGNED                         |             |
