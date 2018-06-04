# <a name="onenote-api-overview"></a>Visão geral da API do OneNote

O OneNote é um bloco de anotações digital que permite que os clientes acompanhem ideias e anotações para uso doméstico, escolar ou profissional digitando, desenhando ou falando na Web, no telefone, no tablet ou no computador. Eles podem livremente organizar anotações, alternar entre dispositivos e retomar de onde pararam, além de colaborar em anotações com outras pessoas em tempo real.

## <a name="why-integrate-with-onenote"></a>Por que integrar com o OneNote?

Integrando os aplicativos ao OneNote, você pode criar experiências para capacitação em várias plataformas que alcançam milhões de usuários em todo o mundo. Você pode usar o Microsoft Graph para acessar blocos de anotações, seções e páginas no OneNote para criar soluções que ajudam os usuários a planejar e organizar informações e ideias.

### <a name="collect-and-organize-notes-and-ideas"></a>Coletar e organizar anotações e ideias  
Use o OneNote com uma tela em que os usuários podem adicionar e organizar conteúdo. O Microsoft Graph facilita a criação de aplicativos que ajudam os alunos a fazer anotações e pesquisas, as famílias a compartilhar planos e ideias ou os compradores a compartilhar imagens. O aplicativo pode obter as informações que as pessoas desejam, enviá-las ao OneNote e ajudar a organizá-las.

### <a name="capture-information-in-many-formats"></a>Capturar informações em muitos formatos
Capture HTML, insira imagens (originadas localmente ou em uma URL pública), vídeo, áudio, mensagens de email e outros tipos de arquivos comuns. O OneNote pode até mesmo renderizar páginas da Web e arquivos PDF como instantâneos. O Microsoft Graph dá suporte a um conjunto de HTML e CSS padrão para layout de página do OneNote. Portanto, você pode usar tabelas, imagens embutidas e formatação básica para obter a aparência desejada. 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>Usar o ecossistema do OneNote para aprimorar seus cenários principais
Aproveite outros recursos poderosos do OneNote. As APIs do OneNote no Microsoft Graph executam OCR em imagens, dão suporte à pesquisa de texto completo, sincronizam clientes automaticamente, processam imagens e extraem capturas de cartões de visita e listagens de receitas e produtos online. Use o OneNote como seu repositório de memória digital na nuvem para anotações e mídia leve ou como um feed de dados para dados específicos de domínio. 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>Alcance milhares de usuários do OneNote em todas as principais plataformas
Use o OneNote para aumentar o uso do aplicativo. O OneNote vem pré-instalado nos novos dispositivos Windows e está disponível para a maioria das plataformas, online e como parte do Office 365.
 Ao publicar aplicativos que usam o ambiente do OneNote repleto de recursos, você tem acesso a um amplo potencial de mercado em várias plataformas.

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: https://developer.microsoft.com/en-us/graph/docs/concepts/featured_scenarios. You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>O que posso fazer com as APIs do OneNote no Microsoft Graph?

A seguir, estão algumas das solicitações mais populares para trabalhar com os recursos do OneNote.

|Operação|URL|
|:--------|:--|
|Obter meus blocos de anotações|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|Obter minhas seções|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|Obter minhas páginas|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="learn-more-about-onenote-apis"></a>Saiba mais sobre as APIs do OneNote

Faça uma análise aprofundada das APIs do Microsoft Graph para saber mais sobre as funcionalidades de atualização de conteúdo do OneNote. Os tópicos na lista a seguir mostram como criar novas páginas do OneNote e atualizar páginas existentes com novo conteúdo. Você também aprenderá sobre as práticas recomendadas usando o Microsoft Graph para atualizar os blocos de anotações do OneNote. 


**Trabalhar com o OneNote**

* [Usar a API REST do OneNote](../api-reference/v1.0/resources/onenote-api-overview.md)
* [Práticas recomendadas](onenote_best_practices.md)
* [Diretrizes de identidade visual](onenote-branding.md)
* [Abrir o cliente do OneNote](open_onenote_client.md)
* [Usar marcas de anotação nas páginas do OneNote](onenote-note-tags.md)
* [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote_error_codes.md)

**Trabalhar com páginas do OneNote**

* [HTML de entrada e saída nas páginas do OneNote](onenote_input_output_html.md)
* [Obter a estrutura e o conteúdo do OneNote com o Microsoft Graph](onenote-get-content.md)
* [Criar páginas do OneNote](onenote-create-page.md)
* [Atualizar o conteúdo da página do OneNote](onenote_update_page.md)

**Trabalhar com conteúdo da página do OneNote**

* [Criar elementos posicionados absolutos nas páginas do OneNote](onenote-abs-pos.md)
* [Adicionar imagens, vídeos e arquivos a páginas do OneNote](onenote_images_files.md)
* [Usar marcas DIV da API do OneNote para extrair dados de capturas](onenote-extract-data.md)



## <a name="explore-the-onenote-apis"></a>Explorar as APIs do OneNote
Use o [Microsoft Graph Explorer](https://developer.microsoft.com/pt-BR/graph/graph-explorer) para experimentar as APIs do OneNote com seus próprios blocos de anotações do OneNote.

Para fazer chamadas à API do OneNote por meio do Explorador do Graph, escolha **Mostrar mais exemplos** na coluna à esquerda. Use o menu para **Ativar** o OneNote. Você também precisará habilitar as permissões apropriadas. No nome da conta no menu à esquerda, escolha **modificar permissões**. Para saber mais sobre as permissões do OneNote, confira [Permissões de anotações](permissions_reference.md#notes-permissions).

Para começar a usar as APIs do OneNote no Microsoft Graph, confira o [conteúdo de referência do OneNote](../api-reference/v1.0/resources/onenote.md).
