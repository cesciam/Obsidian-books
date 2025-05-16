Non votalite registers: son los registros guardados a través de las llamadas de función. (R12 -R15)
Fastcall registers: Registros que se utilizan para enviar parametros a funciones. (RCS, RDX, R8, R9)

## Inline expansion: 
es una optimización del compilador que reemplaza una llamada a función, con el código de la función misma, para evitar el pasar argumentos, cargar registros, etc. 
Ocurre cuando se define como "inline", aunque no siempre, o cuando la función es pequeña. También se puede forzar al compilador para que NO lo haga. 

## Tail Call Elimination:

Es una optimización que reemplaza una llamada recursiva en la última posición (la última línea), con un jmp, para evitar crear un nuevo stack frame. Eso es útil cuando la función que llama a la otra función comparte los parámetros. Debido a que comparten los parametros, no hay necesidad de volver a cargar estos valores en el stack .

## Frame Pointer Omission
