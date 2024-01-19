st=>start: Inicio
op1=>operation: Poner agua en la cafetera
op2=>operation: Encender la cafetera
op3=>operation: Verter café en una taza
cond1=>condition: ¿Hay leche en la nevera?
op4=>operation: Calentar leche en el microondas
op5=>operation: Verter leche en la taza
op6=>operation: Añadir azúcar al gusto
e=>end: Fin

st->op1->op2->op3->cond1
cond1(yes)->op4->op5->op6->e
cond1(no)->op6->e
