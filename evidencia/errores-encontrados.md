# Errores encontrados en el cajero del compañero

Mi suite (MP-1 a MP-4) atrapó sola **N** de los 5 errores: (las pruebas que fallaron en mp5-companero.txt)

| Queja | Prueba que la reproduce | Qué estaba mal en el código (la línea y por qué) | ¿Mi suite ya lo atrapaba? |
|---|---|---|---|
| 1 | sinSmsSiNoHaySaldo | Orden en la operación de retirar, avisar al final | no |
| 2 | sospechosaNoMueveDinero | El problema igual de retirar, retirar justo antes de guardar | no |
| 3 | seGuardaUnaVez | se reptia la linea de guardar igual en la operación retirar | no |
| 4 | antifraudeCaidoRechaza | cuando el anti furade fallata teniamos que regresar el excepcion y no lo hacia | no |
| 5 | limiteDiarioExacto | en el limite tenia un ">=" y solo era ">" | no |