# Práctica de Git y Git Hub de Cristian Varela Casas. Bootcamp Web XIV.

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

6. ¿Qué comando o comandos utilizaste en el paso 25?

**git log --graph**

