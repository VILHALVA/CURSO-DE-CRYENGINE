# CURSO DE CRYENGINE
👨‍⚖️A CRYENGINE É UMA ENGINE DE JOGO DESENVOLVIDA PELA CRYTEK, UTILIZADA PARA CRIAR JOGOS DE ALTA QUALIDADE COM GRÁFICOS AVANÇADOS E FÍSICA REALISTA.

[![GitHub Repo stars](https://img.shields.io/badge/VILHALVA-GITHUB-03A9F4?logo=github)](https://github.com/VILHALVA) 
[![GitHub Repo stars](https://img.shields.io/badge/VEJA%20OS-VIDEOS-03A9F4?logo=youtube)](https://www.youtube.com/@vilhalva100/search?query=CRYENGINE)

[![GitHub Repo stars](https://img.shields.io/badge/VEJA-DOCUMENTAÇÃO-03A9F4?logo=google)](https://docs.cryengine.com/) 
[![GitHub Repo stars](https://img.shields.io/badge/LINGUAGEM%20DE-PROGRAMAÇÃO-03A9F4?logo=github)](https://github.com/VILHALVA/CURSO-DE-LUA)
<br>

[![GitHub Repo stars](https://img.shields.io/badge/-PLAYLIST%20DO%20YOUTUBE-blueviolet)](https://youtube.com/playlist?list=PL3rePi75166S-_KYHjd1yLxZEWyR63nzf&si=BuYErIwRn2VRr7wD)

<img src="https://static.wikia.nocookie.net/logopedia/images/c/cf/CRYENGINE_3_Logo.png/revision/latest/scale-to-width-down/250?cb=20190309071553" align="center" width="280"> <br>

![](https://i.imgur.com/waxVImv.png)

# CONCEITO:
A CryEngine é uma poderosa engine de jogo utilizada para desenvolver jogos de alta qualidade. Vou abordar alguns conceitos básicos e fornecer um exemplo simples de código usando a CryEngine:

1. **Entity (Entidade):** No contexto da CryEngine, uma entidade é basicamente qualquer objeto no jogo. Pode ser um jogador, inimigo, item no cenário, etc. Cada entidade possui propriedades e comportamentos associados.

2. **Components (Componentes):** Os componentes são partes modulares de uma entidade que definem seu comportamento. Por exemplo, um componente de física pode ser responsável pela movimentação, enquanto um componente de renderização cuida da aparência visual.

3. **Level (Nível):** Refere-se a um ambiente ou fase do jogo. É onde as entidades existem e interagem.

4. **Flow Graph:** Um sistema visual de programação que permite criar lógica de jogo sem escrever código. Pode ser usado para definir comportamentos complexos e interações entre entidades.

**Exemplo de Código:**

Vamos criar um script simples em Lua (linguagem de script comumente usada na CryEngine) que faz uma entidade imprimir uma mensagem no console quando é inicializada.

```lua
-- Nome do arquivo: MyScript.lua

MyScript = {
  Properties = {
    Message = "Olá, Mundo!",
  }
}

function MyScript:OnActivate()
  System.Log(self.Properties.Message)
end
```

**Explicação do Código:**

- `MyScript` é uma tabela que age como a classe para nosso script.
- `Properties` define propriedades da entidade associada ao script. Neste caso, temos uma propriedade chamada `Message`.
- `OnActivate` é chamado quando a entidade é ativada no jogo. Neste exemplo, ele imprime a mensagem definida na propriedade no console do jogo.

Lembre-se de integrar este script a uma entidade na CryEngine para ver o resultado. Estes são conceitos iniciais e o desenvolvimento em CryEngine pode envolver muitos outros aspectos como design de níveis, manipulação de assets, controle de animações, entre outros.

# CARACETERISTICAS:
## Características Positivas:
1. **Gráficos de Alta Qualidade:** A CryEngine é conhecida por oferecer gráficos de alta qualidade, com efeitos visuais impressionantes, iluminação avançada e detalhes realistas.

2. **Sistema de Física Avançado:** A engine possui um sólido sistema de física que permite simulações realistas, o que é crucial para jogos que buscam autenticidade em termos de movimento e interação no ambiente.

3. **Suporte para Realidade Virtual:** A CryEngine oferece suporte para desenvolvimento de jogos em realidade virtual, o que é uma característica importante no cenário atual de desenvolvimento de jogos.

4. **Performance:** A otimização e o desempenho são pontos fortes da CryEngine, especialmente quando se trata de renderização de ambientes extensos e complexos.

5. **Sistema de Som:** A engine possui um sistema de áudio avançado, permitindo a implementação de trilhas sonoras envolventes e efeitos sonoros realistas.

## Características Negativas:
1. **Curva de Aprendizado Elevada:** A CryEngine pode ter uma curva de aprendizado mais íngreme em comparação com algumas outras engines, especialmente para desenvolvedores iniciantes.

2. **Licenciamento:** Embora a CryEngine seja gratuita para projetos não comerciais, há custos associados ao uso comercial da engine. O licenciamento pode ser mais caro do que outras opções disponíveis.

3. **Comunidade Menor:** Comparada a algumas outras engines populares, a CryEngine tem uma comunidade menor. Isso pode afetar a disponibilidade de recursos, tutoriais e suporte online.

4. **Menor Quantidade de Recursos Prontos:** Em comparação com engines mais estabelecidas, a CryEngine pode ter uma quantidade menor de recursos prontos para uso, o que pode aumentar o tempo de desenvolvimento.

5. **Menos Flexibilidade Multiplataforma:** Embora a CryEngine seja capaz de exportar para várias plataformas, pode haver desafios adicionais ao desenvolver para certas plataformas em comparação com engines que se especializam mais nisso.

