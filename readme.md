# Práctica de Git y Git Hub de Cristian Varela Casas. Bootcamp Web XIV.

> Nota: la rama master, al haber creado el repositorio desde Github, ha sido renombrada a main. No estoy deacuerdo con estas
> estas tonterías de lo políticamente correcto (incluyendo las censuras en las películas de Disney de toda la vida), no obstante,
> para no complicarme la vida renombrando en Github, pasaré por el aro. 

1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?

**git reset --hard HEAD~1**
Porque se retorna al commit anterior perdiendo los cambios realizados en el working copy, a diferencia de *git reset HEAD~1*,
que tan solo deshace el commit, manteniendo el working copy.

2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

**git reset** (o **git reset HEAD** ya que Git traga igual) + **HASH del commit**
Porque para progresar hacia commits más recientes no podemos utilizar el *~1*.

3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No, porque se trato de un merge fast-fordward. Porque *"Los conflictos solo se pueden crear en los merge NO fast-forward y 
realizdos de manera forzada"* (Casero, A., 2022).

> Alberto, estuve pensando pero no comprendo lo de "manera forzada" ¿A qué te referiste?¿A aquellos que por defecto harían
> fast-fordward pero que nosotros decidimos un NO f-f? Te lo pregunto porque creo que un NO fast-fordward, sin ser forzado,
> ya puede crear un conflicto, es decir, modifico el mismo archivo en sus mismas líneas y en dos ramas bifurcadas
> (no es posible ya un merge f-f) y mergeo NO f-f (no fuerzo nada) ¿Me equivoco?

4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Sí, porque habíamos modificado las mismas líneas del mismo archivo (git-nuestro.md) y a continuación habíamos mergeado ambas ramas
tratándose de un NO fast-fordward.

> Aquí no he leído bien el paréntesis del paso y he mergeado al reves, por lo que he tenido que montar un cristo para deshacer la
> la CAGADA con git reset --hard HEAD~1 y luego apañármelas como he podido. Al final he salido del lío.
>> Alberto nuestro, perdona mis cagadas como yo perdono a los que creen que la tierra es plana.

5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No, porque se trataba de un merge fast-fordwar donde main avanzaba hasta "pillar" a styled.


6. ¿Qué comando o comandos utilizaste en el paso 25?

**git log --graph**

7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

No, porque ambas ramas están ya bifurcadas y una no puede "alcanzar linealmente a la otra"; además, he hecho *git merge* 'normal' 
para ver si creaba conflicto con las variaciones en el readme.md de ambas para cerciorarme, y lo creaba.

8. ¿Qué comando o comandos utilizaste en el paso 27?

**git reset HEAD~1**

9. ¿Qué comando o comandos utilizaste en el paso 28?

**git restore . **

10. ¿Qué comando o comandos utilizaste en el paso 29?

**git branch -D title**

11. ¿Qué comando o comandos utilizaste en el paso 30?

**git reset** + **HASH del commit** (viendo previamente el "rastro de migas" con git reflog).

12. ¿Qué comando o comandos usaste en el paso 32?

**git checkout** + **HASH del commit inicial** (solo va hasta ahí la "cabeza").

13. ¿Qué comando o comandos usaste en el punto 33?

**git checkout main** (porque el puntero de rama ya lo teníamos situado en ese commit).
