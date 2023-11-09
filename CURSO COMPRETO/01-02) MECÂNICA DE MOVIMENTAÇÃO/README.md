# MECÂNICA DE MOVIMENTAÇÃO
A implementação da mecânica de movimentação é uma parte crucial no desenvolvimento de jogos, e a CryEngine oferece ferramentas e funcionalidades para tornar esse processo mais acessível. Abaixo, vou abordar alguns conceitos e dar um exemplo simples de como implementar a movimentação de um personagem em um jogo CryEngine usando Lua, que é a linguagem de script comumente utilizada.

**1. Entidades e Componentes:**
   - Em CryEngine, a movimentação geralmente envolve trabalhar com entidades e seus componentes. Por exemplo, você pode ter uma entidade representando o jogador e componentes relacionados à física e à renderização.

**2. Criação da Entidade do Jogador:**
   - Primeiro, você precisa criar uma entidade para representar o jogador. Isso pode ser feito através do Editor da CryEngine.

**3. Adição de Componentes:**
   - Adicione componentes relevantes à entidade do jogador. Isso pode incluir um componente de física para lidar com a movimentação física e um componente de renderização para a aparência visual.

**4. Scripting para Movimentação:**
   - Crie um script em Lua para lidar com a movimentação do jogador. Aqui está um exemplo simples que usa a entrada do teclado para mover a entidade para frente e para trás:

```lua
-- Nome do arquivo: PlayerMovement.lua

PlayerMovement = {
  speed = 5.0,  -- Velocidade do movimento
}

function PlayerMovement:OnActivate()
  Input:SetActionMap(1, "Player")
end

function PlayerMovement:OnDeactivate()
  Input:SetActionMap(0, "Player")
end

function PlayerMovement:OnUpdate(frameTime)
  local moveDirection = { x = 0, y = 0, z = 0 }

  -- Verifica as teclas de movimento
  if (Input:IsKeyDown("w")) then
    moveDirection.y = 1
  elseif (Input:IsKeyDown("s")) then
    moveDirection.y = -1
  end

  -- Move a entidade
  local moveAmount = self.speed * frameTime
  self.entity:Move(moveDirection.x * moveAmount, moveDirection.y * moveAmount, moveDirection.z * moveAmount)
end
```

**Explicação do Código:**
- `OnActivate`: Configura o mapeamento de ação para o jogador quando a entidade é ativada.
- `OnDeactivate`: Desativa o mapeamento de ação quando a entidade é desativada.
- `OnUpdate`: Chamado a cada quadro para atualizações contínuas. Move a entidade com base nas teclas de movimento pressionadas.

Lembre-se de que este é apenas um exemplo básico. Dependendo das necessidades do seu jogo, você pode precisar adicionar detecção de colisão, animações, ou lógica mais complexa para uma experiência de movimentação mais sofisticada. Consulte a documentação da CryEngine para obter informações detalhadas sobre a movimentação e interação de entidades.