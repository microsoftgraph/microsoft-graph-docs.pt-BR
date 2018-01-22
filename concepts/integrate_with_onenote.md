# <a name="use-microsoft-graph-to-integrate-with-onenote"></a>Usar o Microsoft Graph para integração com o OneNote

Integrando os aplicativos ao OneNote, você pode criar experiências para capacitação em várias plataformas que alcançam milhões de usuários em todo o mundo. Você pode usar o Microsoft Graph para acessar blocos de anotações, seções e páginas no OneNote para criar soluções que ajudam os usuários a planejar e organizar informações e ideias.

## <a name="why-create-onenote-apps"></a>Por que criar aplicativos do OneNote?

Você pode usar o Microsoft Graph para criar e gerenciar anotações, listas, imagens, arquivos e muito mais em blocos de anotações do OneNote.

### <a name="collect-and-organize-notes-and-ideas"></a>Coletar e organizar anotações e ideias  
Use o OneNote com uma tela em que os usuários podem adicionar e organizar conteúdo. O Microsoft Graph facilita a criação de aplicativos que ajudam os alunos a fazer anotações e pesquisas, as famílias a compartilhar planos e ideias ou os compradores a compartilhar imagens. O aplicativo pode obter as informações que as pessoas desejam, enviá-las ao OneNote e ajudar a organizá-las.

### <a name="capture-information-in-many-formats"></a>Capturar informações em muitos formatos
Capture HTML, insira imagens (originadas localmente ou em uma URL pública), vídeo, áudio, mensagens de email e outros tipos de arquivos comuns. O OneNote pode até mesmo renderizar páginas da Web e arquivos PDF como instantâneos. O Microsoft Graph dá suporte a um conjunto de HTML e CSS padrão para layout de página do OneNote. Portanto, você pode usar tabelas, imagens embutidas e formatação básica para obter a aparência desejada. 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>Usar o ecossistema do OneNote para aprimorar seus cenários principais
Aproveite outros recursos poderosos do OneNote. As APIs do OneNote no Microsoft Graph executam OCR em imagens, dão suporte à pesquisa de texto completo, sincronizam clientes automaticamente, processam imagens e extraem capturas de cartões de visita e listagens de receitas e produtos online. Use o OneNote como seu repositório de memória digital na nuvem para anotações e mídia leve ou como um feed de dados para dados específicos de domínio. 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>Alcance milhares de usuários do OneNote em todas as principais plataformas
Use o OneNote para aumentar o uso do aplicativo. O OneNote vem pré-instalado no novos dispositivos Windows e está disponível para a maioria das plataformas, online e como parte do Office 365. Ao publicar aplicativos que usam o ambiente do OneNote repleto de recursos, você tem acesso a um amplo potencial de mercado em várias plataformas.

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: https://developer.microsoft.com/en-us/graph/docs/concepts/featured_scenarios. You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>O que posso fazer com as APIs do OneNote no Microsoft Graph?

A seguir, estão algumas das solicitações mais populares para trabalhar com os recursos do OneNote.

|Operação|URL|
|:--------|:--|
|GET meus blocos de anotações|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/pt-BR/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|GET minhas seções|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/pt-BR/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|GET minhas páginas|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/pt-BR/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="explore-the-onenote-apis"></a>Explorar as APIs do OneNote
Use o [Microsoft Graph Explorer](https://developer.microsoft.com/pt-BR/graph/graph-explorer) para experimentar as APIs do OneNote com seus próprios blocos de anotações do OneNote.

Para fazer chamadas à API do OneNote por meio do Explorador do Graph, escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para **Ativar** o OneNote. Você também precisará habilitar as permissões apropriadas. No nome da conta no menu à esquerda, escolha **modificar permissões**. Para saber mais sobre as permissões do OneNote, confira [Permissões de anotações](permissions_reference.md#notes-permissions).

Para começar a usar as APIs do OneNote no Microsoft Graph, confira o [conteúdo de referência do OneNote](../api-reference/v1.0/resources/onenote.md).

## <a name="see-also"></a>Confira também

* [Diretrizes de identidade visual](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-branding)
* [Obter a estrutura e o conteúdo do OneNote](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-get-content)
* [Adicionar imagens, vídeos e arquivos](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-images-files)
* [Criar elementos posicionados absolutos](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-abs-pos)
* [Extrair dados](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-extract-data)
* [Usar marcas de anotação](https://msdn.microsoft.com/pt-BR/office/office365/howto/onenote-note-tags)

