# EXTRA: DIRETÓRIOS E EXPORTAÇÃO
## DIRETÓRIOS:
A estrutura de pastas em projetos na CryEngine pode variar um pouco dependendo da versão específica da engine e das preferências da equipe de desenvolvimento. No entanto, há uma estrutura de diretórios comum que é frequentemente utilizada para organizar os assets e outros arquivos do projeto. Aqui está uma visão geral genérica:

1. **Assets:**
   - **/Game:**
     - Contém todos os ativos do jogo, incluindo modelos 3D, texturas, materiais, animações, e assim por diante.
   - **/Levels:**
     - Armazena os arquivos de level criados no Editor, cada level pode ter sua própria pasta.
   - **/Scripts:**
     - Contém scripts Lua usados para implementar lógica de jogo e comportamentos específicos.
   - **/UI:**
     - Guarda arquivos relacionados à interface do usuário, como texturas de botões e layouts.

2. **Engine:**
   - **/Config:**
     - Configurações específicas do projeto ou modificações nas configurações padrão da engine.
   - **/Libs:**
     - Bibliotecas ou módulos adicionais usados no projeto.
   - **/Scripts:**
     - Scripts Lua específicos da engine.

3. **Bin:**
   - Contém os executáveis do jogo após a compilação.

4. **GameSDK:**
   - Este é um exemplo de projeto que acompanha a CryEngine e pode ser usado como ponto de partida. Contém assets, scripts e outros elementos básicos.

5. **Screenshots:**
   - Pode conter capturas de tela geradas durante o desenvolvimento.

6. **.git:**
   - Se o controle de versão Git for utilizado, esta pasta conterá os arquivos relacionados.

7. **Logs:**
   - Armazena logs e mensagens de depuração geradas durante a execução do jogo.

8. **Other Directories:**
   - Dependendo das necessidades do projeto, podem existir diretórios adicionais, como para armazenar plugins, documentação ou recursos específicos.

Lembre-se de que a organização pode ser adaptada com base nas necessidades específicas do seu projeto e nas preferências da equipe de desenvolvimento. O uso de controle de versão, como Git, também é altamente recomendado para rastrear alterações ao longo do tempo. Sempre consulte a documentação da CryEngine e as melhores práticas para obter informações mais detalhadas e específicas sobre a organização de projetos.

## EXPORTAÇÃO:
Exportar um jogo para diferentes plataformas na CryEngine envolve etapas específicas para cada sistema operacional ou console alvo. Abaixo, fornecerei uma visão geral geral, mas esteja ciente de que detalhes específicos podem variar dependendo da versão da CryEngine e das ferramentas de desenvolvimento específicas para cada plataforma. Certifique-se de consultar a documentação oficial e recursos específicos para obter as informações mais atualizadas e detalhadas.

### Exportar para Plataformas Específicas:
1. **Windows:**
   - No Editor da CryEngine, vá para `File` (Arquivo) > `Export Game Launcher` (Exportar Lançador do Jogo).
   - Selecione a plataforma desejada (por exemplo, Windows).
   - Configure as opções de build, incluindo resolução, qualidade gráfica e outros detalhes específicos do seu jogo.
   - Clique em "Export" para gerar os arquivos do jogo para o Windows.
   - Execute o executável gerado para testar o jogo.

2. **PlayStation (PS4):**
   - Consulte a documentação específica da CryEngine para integração com o PlayStation Development Kit (PDK).
   - Configure as opções do projeto para a plataforma PS4 no Editor.
   - Compile o código e recursos específicos do PS4 usando as ferramentas fornecidas pela CryEngine e pela Sony.

3. **Xbox (Xbox One):**
   - Assim como no PS4, consulte a documentação específica da CryEngine para integração com o Xbox Development Kit (XDK).
   - Configure as opções do projeto para a plataforma Xbox no Editor.
   - Compile o código e recursos específicos do Xbox usando as ferramentas fornecidas pela CryEngine e pela Microsoft.

4. **Linux:**
   - No Editor, vá para `File` (Arquivo) > `Export Game Launcher` (Exportar Lançador do Jogo).
   - Escolha a plataforma Linux e configure as opções relevantes.
   - Clique em "Export" para gerar os arquivos do jogo para Linux.
   - Teste o jogo no ambiente Linux correspondente.

### Considerações Importantes:
- **SDKs e Ferramentas de Desenvolvimento:**
  Certifique-se de ter os SDKs e as ferramentas de desenvolvimento necessárias instaladas para cada plataforma alvo. Isso inclui o PlayStation Development Kit (PDK), o Xbox Development Kit (XDK), ou qualquer SDK específico para a plataforma.

- **Licenças e Certificação:**
  Para plataformas de console, certifique-se de atender a todos os requisitos de licenciamento e certificação impostos pelos fabricantes dos consoles.

- **Testes e Depuração:**
  Realize testes extensivos em cada plataforma para garantir que o jogo funcione corretamente e atenda aos padrões de desempenho esperados.

- **Atualizações de Plataforma:**
  Esteja ciente de que as plataformas podem ter atualizações e requisitos específicos ao longo do tempo. Mantenha-se informado sobre as diretrizes de desenvolvimento de cada plataforma.

Antes de iniciar o processo de exportação, recomenda-se fortemente revisar as diretrizes e documentação oficiais da CryEngine e das plataformas alvo para garantir uma integração e exportação suaves.