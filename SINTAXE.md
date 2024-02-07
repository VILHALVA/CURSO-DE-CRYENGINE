# SINTAXE
Na CryEngine, os scripts são escritos principalmente em [C++](https://github.com/VILHALVA/CURSO-DE-C-PLUS-PLUS), embora também haja suporte para a linguagem de script [Lua](https://github.com/VILHALVA/CURSO-DE-LUA). Abaixo está um exemplo de como mover um objeto usando teclas de seta em um projeto da CryEngine que usa Lua como linguagem de script:

```lua
function OnUpdate(deltaTime)
    -- Verificar se a tecla de seta direita está sendo pressionada
    if Input:GetKeyValue(eKI_Right) then
        -- Mover o objeto para a direita
        entity:SetWorldPos(entity:GetWorldPos() + Vec3(5 * deltaTime, 0, 0))
    end

    -- Verificar se a tecla de seta esquerda está sendo pressionada
    if Input:GetKeyValue(eKI_Left) then
        -- Mover o objeto para a esquerda
        entity:SetWorldPos(entity:GetWorldPos() - Vec3(5 * deltaTime, 0, 0))
    end

    -- Verificar se a tecla de seta para baixo está sendo pressionada
    if Input:GetKeyValue(eKI_Down) then
        -- Mover o objeto para baixo
        entity:SetWorldPos(entity:GetWorldPos() + Vec3(0, 0, 5 * deltaTime))
    end

    -- Verificar se a tecla de seta para cima está sendo pressionada
    if Input:GetKeyValue(eKI_Up) then
        -- Mover o objeto para cima
        entity:SetWorldPos(entity:GetWorldPos() - Vec3(0, 0, 5 * deltaTime))
    end
end
```

Vou explicar o código:

1. **Evento `OnUpdate`**:
   - No CryEngine, o método `OnUpdate` é chamado a cada quadro.

2. **Verificando Teclas Pressionadas**:
   - O método `Input:GetKeyValue(key)` é usado para verificar se uma determinada tecla está sendo pressionada.
   - No exemplo, estamos verificando as teclas de seta direita, esquerda, para baixo e para cima.

3. **Movendo o Objeto**:
   - Se uma tecla de seta correspondente estiver pressionada, o objeto é movido na direção apropriada.
   - A posição do objeto é modificada usando o método `SetWorldPos`, que recebe um vetor de posição no espaço 3D.

Este é um exemplo simples de como mover um objeto usando teclas de seta na CryEngine com Lua como linguagem de script. Lembrando que, se estiver usando C++, o processo será diferente, envolvendo manipulação de entidades e outros conceitos específicos dessa linguagem e dessa engine.