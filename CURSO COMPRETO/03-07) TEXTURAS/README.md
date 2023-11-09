# TEXTURAS
O uso de texturas é essencial para dar vida aos objetos e ambientes em um jogo. Na CryEngine, a aplicação de texturas envolve alguns passos básicos. Aqui estão alguns conceitos e um exemplo simples de como você pode aplicar texturas em um objeto usando a CryEngine:

**1. Importação de Texturas:**
   - Antes de aplicar texturas, você precisa importar as texturas desejadas para o seu projeto. Isso pode ser feito através do Editor da CryEngine.

**2. Materiais:**
   - Em CryEngine, os materiais são usados para definir como as superfícies dos objetos respondem à luz e quais texturas são aplicadas. Crie ou edite materiais para especificar as propriedades visuais de um objeto.

**3. Configuração do Material:**
   - Configure o material do objeto para incluir as texturas desejadas. Você pode fazer isso no Editor, definindo propriedades como difusão, normal e emissão.

**4. Scripting para Aplicar Texturas:**
   - Você pode usar scripts para dinamicamente modificar as propriedades do material em tempo de execução. Aqui está um exemplo simples em Lua:

```lua
-- Nome do arquivo: ApplyTexture.lua

ApplyTexture = {}

function ApplyTexture:OnActivate()
  -- Obtém o material da entidade
  local material = self.entity:GetMaterial(0)  -- 0 representa o primeiro submaterial

  -- Carrega a textura
  local texturePath = "Textures/ExampleTexture.dds"
  local textureId = Game.LoadTexture(texturePath)

  -- Define a textura no material
  material:SetTexture(0, textureId)  -- 0 representa o primeiro slot de textura
end
```

**Explicação do Código:**
- `OnActivate`: Chamado quando a entidade é ativada. Este é um exemplo simples que aplica uma textura ao material da entidade.

Lembre-se de que este é um exemplo básico e a aplicação de texturas pode ser mais complexa dependendo do contexto do seu jogo. A CryEngine suporta uma variedade de tipos de texturas, incluindo mapas de difusão, normais, especulares, entre outros. Além disso, você pode usar o Editor para configurar materiais visualmente sem a necessidade de scripting em alguns casos. Consulte a documentação oficial da CryEngine para obter informações mais detalhadas sobre texturas e materiais.