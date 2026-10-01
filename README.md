# Cajero automático — pruebas con JUnit 5 y Mockito

**Autor:** Andrés Juárez Garduño

## Cómo correr las pruebas

    ./probar.sh final

## Qué prueba cada clase

| Clase de prueba | Qué prueba | Qué dobles usa | Cuántas pruebas |
|---|---|---|---|
| CajeroConDoblesAManoTest | retiro bajo saldo y cuenta que no existe | fakes hechos a mano y una lambda | 2 |
| StubsTest | operaciones sospechosas, retiros funcionen, mock sin configurar, etc. | uso de stubs y when...then... | 7 |
| InteraccionesTest | que, cuanto y en que orden | uso del verify, argument captor y order | 7 |
| AnotacionesTest | parecido al anterior pero con menores pruebas | uso del mock captor | 3 |
| QuejasCajeroTest | quejas de los usarios sobre el cajero | los stubs y el verify | 5 |
| RelojTest | uso de fechas/dias | usando el when/then y fechas | 3 |

## Boleto de salida

1. ¿Qué diferencia hay entre un stub y un mock? Da un ejemplo de cada uno de hoy.
Como lo entendí yo es que los stubs nos dan datos o estados y los mock verifican comportamiento, usando el when...then... y verify respectivamente.
2. ¿Por qué la prueba inútil de la MP-6 salía en verde con el cajero roto?
Como se mencionó en la práctica, solamente está comprobando que regrese 1500.00.
3. ¿Qué NO mockearías en un proyecto de Spring Boot como el de la Semana 3, y por qué?
Cuentas de banco y transacciones. por qué se están simulando información que debe estar protegida.