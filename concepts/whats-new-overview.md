---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 4bc0a5f571b172bbcbb7e2ae74c6dfd854ba645b
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364387"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](changelog.md). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.


## <a name="september-2020-new-and-generally-available"></a>Setembro de 2020: novo e disponível para o público geral

### <a name="calendar"></a>Calendário
O GA da propriedade **transactionId** do recurso de [evento](/graph/api/resources/event), que é definido opcionalmente por um aplicativo cliente para evitar operações de POSTAGEM redundantes em caso de o cliente tentar criar o mesmo evento. Isso é útil quando a conectividade de rede baixa faz com que o cliente expire antes de receber uma resposta do servidor para a solicitação anterior de criação de evento do cliente.

### <a name="cloud-communications"></a>Comunicações na nuvem
[Remover um participante](/graph/api/participant-delete) do [bate-papo](/graph/api/resources/call). Você pode usar essa operação mesmo em situações em que é necessário excluir um participante de uma chamada ativa.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
As atualizações de [setembro](changelog.md#september-2020) do Intune para a versão v1.0.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
Os [APIs das unidades administrativas](/graph/api/resources/administrativeunit) permitem às organizações subdividir seu Azure Active Directory e delegar tarefas administrativas a essas subdivisões. As subdivisões podem representar regiões, departamentos, centros de custo e assim por diante.

### <a name="reports"></a>Relatórios
[Obtenha um relatório que inclua o número de usuários exclusivos](/graph/api/reportroot-getemailappusageversionsusercounts) do Outlook 2019 e do Outlook no Microsoft 365.

### <a name="teamwork"></a>Trabalho em equipe
- Obtenha a propriedade **lastEditedDateTime** para descobrir quando um remetente editar pela última vez uma [mensagem de chat](/graph/api/resources/chatmessage).
- Obtenha a propriedade **lastModifiedDateTime** para descobrir quando um remetente cria uma mensagem de bate-papo ou quando alguém a altera de outras maneiras, incluindo a adição ou a remoção de uma reação. 
- [Receba notificações sobre alterações](webhooks.md) em [mensagens de chat](/graph/api/resources/chatmessage).
- [Atualizar](/graph/api/chatmessage-update?view=graph-rest-beta&preserve-view=true) propriedade **policyViolation** de uma [chatMessage](/graph/api/resources/chatmessagepreserve-view=true) em um [canal](/graph/api/resources/channel&preserve-view=true) ou [chat](/graph/api/resources/chat&preserve-view=true), permitindo que os aplicativos de prevenção contra perda de dados (DLP) monitorem [violação de política da mensagem de chat](/graph/api/resources/chatmessagepolicyviolation?preserve-view=true) para evitar que as mensagens contenham dados que os usuários não devem enviar.

### <a name="use-the-sdks"></a>Use os SDKs
Com o lançamento do [SDK do Microsoft Graph PowerShell](https://github.com/microsoftgraph/msgraph-sdk-powershell) o acesso a toda a superfície do Microsoft Graph agora é simples e consistente.

### <a name="use-the-toolkit"></a>Usar o kit de ferramentas
Experimente o novo tutorial de introdução passo a passo para o Microsoft Graph Toolkit e experimente a comodidade que o Toolkit oferece:
- [Criar um aplicativo Web (JavaScript)](./toolkit/get-started/build-a-web-app.md)
- [Criar uma web part do Microsoft Office SharePoint Online](./toolkit/get-started/build-a-sharepoint-web-part.md)
- [Criar uma guia do Microsoft Teams](./toolkit/get-started/build-a-microsoft-teams-tab.md)
- [Usar o kit de ferramentas com reagir](./toolkit/get-started/use-toolkit-with-react.md)
- [Usar o kit de ferramentas com o Angular](./toolkit/get-started/use-toolkit-with-angular.md)

### <a name="users"></a>Usuários
Além de obter o endereço SMTP de um [usuário](/graph/api/resources/user) por meio da propriedade de **email**, você pode definir essa propriedade e atualizar o endereço de email do usuário. 

## <a name="september-2020-new-in-preview-only"></a>Setembro de 2020: novidades somente na pré-visualização

### <a name="cloud-communications"></a>Comunicações na nuvem
- A substituição da propriedade **autoAdmittedUsers** do[ onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Em vez disso, use a propriedade **lobbyBypassSettings** e seus [valores](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
- Use configurações adicionais sobre como anunciar os chamadores que ingressam em uma reunião online (propriedade**isEntryExitAnnounced**) e permitir apresentadores específicos na reunião (propriedade**allowedPresenters**).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- [Obtenha os documentos para cada um dos trabalhos de impressão associados a uma impressora](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true), aplicando uma `$expand` [opção de consulta do sistema OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters). 
- Filtre trabalhos de impressão pelo usuário que os criou, aplicando uma opção de`$filter` [consulta do sistema OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
As atualizações de [setembro](changelog.md#september-2020) do Intune para a versão beta.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
[Obtenha uma chave de recuperação do BitLocker](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true) em nome do usuário conectado que é o proprietário do dispositivo ou em uma função adequada. Obter uma chave de recuperação gera um [log de auditoria](/azure/active-directory/reports-monitoring/concept-audit-logs), em paridade com a experiência do usuário final.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
É possível incluir uma [agenda](/graph/api/resources/requestschedule?view=graph-rest-beta&preserve-view=true) ao solicitar ou remover uma [atribuição de um usuário para um pacote do Access](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true), que especifica o acesso aos grupos, aplicativos ou sites do SharePoint.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
As organizações podem [obter](/graph/api/continuousaccessevaluationpolicy-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/continuousaccessevaluationpolicy-update?view=graph-rest-beta&preserve-view=true) a [política de avaliação de acesso contínuo](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) para gerenciar sessões de autenticação em tempo real.

### <a name="search"></a>Pesquisar

- Use recursos adicionais no [API de Pesquisa da Microsoft](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) para OneDrive, SharePoint, conectores do Microsoft Graph: 

  - Obtenha [tipos adicionais](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types) de conteúdo do OneDrive e do Microsoft Office SharePoint Online: **unidade**, **lista**, **listItem** e **site**. 
  - Propriedades de escopo nos resultados da pesquisa para [propriedades selecionadas](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#get-selected-properties). 
  - Obtenha propriedades personalizadas no recurso [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true).
  - [Classifique](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#sort-search-results) os resultados da pesquisa do OneDrive e do Microsoft Office SharePoint Online em qualquer propriedade classificável.
  - [Refine os resultados usando agregações](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#refine-results-using-aggregations) para o OneDrive e o Microsoft Office SharePoint Online.
- Consultar dados externos ingeridos pelos conectores do Microsoft Graph em [mais de um de conexão](./search-concept-custom-types.md).
- Aproveite o conteúdo aprimorado para os conectores do Microsoft Graph para saber mais sobre:
  - [Gerenciando Conectores](search-index-manage-connections.md)
  - [Gerenciar esquema](search-index-manage-schema.md)
  - [Gerenciar itens](search-index-manage-items.md)
- Acompanhe o estado de uma[conexão](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true)do Microsoft Graph.
- Defina um [grupo externo](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) a fim de definir permissões em objetos de [item externo](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) adicionados a uma [conexão](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) do Microsoft Graph. Os grupos externos podem representar os grupos do Active Directory que não sejam do Azure ou construções similares, como unidades de negócios, que determinam permissões sobre o conteúdo na fonte de dados externa.

### <a name="teamwork"></a>Trabalho em equipe
- Obtenha a data e a hora em que um [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true)do Teams ou [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) é criada.


## <a name="august-2020-new-and-generally-available"></a>Agosto de 2020: novo e disponível para o público geral

### <a name="change-notifications"></a>Notificações de alteração
[Controle de alterações](delta-query-overview.md) de recursos com suporte para a nuvem nacional do Microsoft Graph para o Governo dos EUA.

### <a name="cloud-communications"></a>Comunicações na nuvem
- [Cancele](/graph/api/call-cancelmediaprocessing) as ações de IVR (Resposta de Voz Interativas) que estão sendo processadas ou na fila, estejam elas [reproduzindo um prompt de áudio](/graph/api/call-playprompt) ou [gravando uma resposta](/graph/api/call-record).
- Obtenha [informações sobre as transcrições da chamada](/graph/api/resources/calltranscriptioninfo) por meio da propriedade **transcrição**.

### <a name="teamwork"></a>Trabalho em equipe
- Use uma maneira alternativa de [criar uma equipe](/graph/api/team-post) diretamente sem criar um grupo primeiro.
- Use a propriedade de navegação**members** para adicionar membros a uma equipe com maior confiabilidade e latência menor.
- Obtenha o status de publicação de um [aplicativo](/graph/api/resources/teamsapp) do Microsoft Teams através da propriedade **publishingState** da [definição do aplicativo](/graph/api/resources/teamsappdefinition). Os valores de status possíveis são `submitted`, `published` e `rejected`. Veja um [exemplo](/graph/api/teamsapp-list?view=graph-rest-beta&preserve-view=true#example-3-list-applications-with-a-given-id-and-return-the-submission-review-state).
- Use a permissão delegada `AppCatalog.Submit` para permitir que um usuário [envie um aplicativo](/graph/api/teamsapp-publish) e solicite a revisão do administrador. Use a mesma permissão para um usuário [cancelar](/graph/api/teamsapp-delete) um aplicativo enviado anteriormente que não foi publicado. 


## <a name="august-2020-new-in-preview-only"></a>Agosto de 2020: novidade apenas na versão prévia

### <a name="applications"></a>Aplicativos
Ofereça suporte a logon único baseado em senha para recursos de aplicativos de [entidade de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) e especifique essas [configurações](/graph/api/resources/passwordsinglesignonsettings?view=graph-rest-beta&preserve-view=true) na propriedade **passwordSingleSignOnSettings**. Para obter informações sobre logon único baseado em senha no Azure AD, confira [configurar logon único baseado em senha](/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).

### <a name="calendar"></a>Calendário
Melhore o suporte programático para cenários que envolvem um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) recorrente:
- Identifique com confiança qualquer ocorrência em uma série recorrente, incluindo uma ocorrência modificada ou cancelada, usando a propriedade **occurrenceId**.
- Obtenha qualquer exceção em uma série recorrente usando a propriedade **exceptionOccurrences**.
- Obtenha qualquer cancelamento em uma série usando a propriedade **cancelledOccurrences**.

### <a name="change-notifications"></a>Alterar notificações
- Use a propriedade **includeResourceData** de uma [assinatura](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) para [configurar notificações de alteração que incluam dados de recursos](webhooks-with-resource-data.md). Não use a propriedade **includeProperties**.
- Receba [notificações de alteração via Hub de Eventos](change-notifications-delivery.md).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Conceda acesso para todos os usuários e grupos a um [compartilhamento de impressora](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) usando a propriedade **allowAllUser**.
- Use novas permissões delegadas e de aplicativo para acessar ou gerenciar um [documento de impressão](/graph/api/resources/printDocument?view=graph-rest-beta&preserve-view=true), [trabalho de impressão](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true), [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true), [compartilhamento de impressora](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) ou [definição de tarefa de impressão](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true). Para obter detalhes, confira as atualizações de [agosto](changelog.md#august-2020) da impressão em nuvem.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [agosto](changelog.md#august-2020) do Intune na versão beta.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
- Personalize um [contrato de termos de uso](/graph/api/resources/agreement?view=graph-rest-beta&preserve-view=true) para oferecer suporte a uma data de vencimento e cadência de contrato, exigir que o usuário aceite o contrato por dispositivo ou aceite novamente o contrato em uma frequência definida. 
- Use a propriedade do**arquivo** para navegar até um [contrato personalizado](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) para termos de uso. Não use a propriedade de **arquivos**.
- Adicione, remova e liste patrocinadores internos ou externos que podem aprovar solicitações de uma [organização conectada](/graph/api/resources/connectedorganization?view=graph-rest-beta&preserve-view=true) para acessar um grupo, aplicativo ou site do SharePoint Online. Para saber mais, confira [gerenciamento de direitos](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Habilite a personalização de uma [política de autorização](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) para um locatário, como autorizar que a [função de usuário padrão](/graph/api/resources/defaultuserrolepermissions?view=graph-rest-beta&preserve-view=true) crie aplicativos, grupos de segurança ou leia outros usuários, e autorizar que os usuários se inscrevam em assinaturas baseadas em email, associem o locatário por validação de email ou permita que os usuários redefinam senhas de maneira autônoma.
- Gerenciar [políticas configuráveis e predefinidas como fluxos de usuário em um locatário do Azure Active Directory B2C](/graph/api/resources/b2cuserflows?view=graph-rest-beta&preserve-view=true). Confira mais informações sobre o [fluxo do usuário B2C](/azure/active-directory-b2c/user-flow-overview).
- Habilite a [experiência de inscrição de maneira autônoma como o fluxo de usuário B2X em um locatário do Azure Active Directory](/graph/api/resources/b2xuserflows?view=graph-rest-beta&preserve-view=true). Confira mais informações sobre a [entrada autônoma](/azure/active-directory/external-identities/self-service-sign-up-overview).

### <a name="people-and-workplace-intelligence--profile"></a>Inteligência de pessoas e do local de trabalho | Perfil
Adicione e gerencie as seguintes propriedades adicionais no [perfil](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true) de um usuário, e que podem ser exibidas em experiências pessoais compartilhadas no Microsoft 365 e em aplicativos de terceiros:
- [addresses](/graph/api/resources/itemAddress?view=graph-rest-beta&preserve-view=true)
- [anniversaries](/graph/api/resources/personAnniversary?view=graph-rest-beta&preserve-view=true)
- [awards](/graph/api/resources/personAward?view=graph-rest-beta&preserve-view=true)
- [certifications](/graph/api/resources/personCertification?view=graph-rest-beta&preserve-view=true)
- [notes](/graph/api/resources/personAnnotation?view=graph-rest-beta&preserve-view=true)
- [patents](/graph/api/resources/itemPatent?view=graph-rest-beta&preserve-view=true)
- [publications](/graph/api/resources/itemPublication?view=graph-rest-beta&preserve-view=true)


### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Obtenha [relatórios sobre o uso de aplicativos do Microsoft 365](/graph/api/resources/microsoft-365-apps-usage-report?view=graph-rest-beta&preserve-view=true), especificamente sobre detalhes de usuários, contagens de usuários e contagens de usuários da plataforma.

### <a name="teamwork"></a>Trabalho em equipe
Obtenha [conteúdo hospedado em uma mensagem de chat](/graph/api/resources/chatMessageHostedContent?view=graph-rest-beta&preserve-view=true), como imagens ou trechos de códigos. Veja um [exemplo](/graph/api/chatmessagehostedcontent-get?view=graph-rest-beta&preserve-view=true&branch=master#example-2-get-hosted-content-bytes-for-an-image) para obter os bytes de conteúdo de uma imagem.

### <a name="to-do-tasks"></a>Tarefas To do
- Lançamento de um novo conjunto de API para o [Microsoft To Do](todo-concept-overview.md), permitindo aos usuários de aplicativos a organizar e acompanhar tarefas pessoais através de aplicativos do cliente Microsoft 365. Confira [Usar a API do Microsoft To Do](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true) para mais informações.
- Preterido a [API de tarefas do Outlook](/graph/api/resources/outlooktask?view=graph-rest-beta&preserve-view=true).


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_**. As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de**_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
