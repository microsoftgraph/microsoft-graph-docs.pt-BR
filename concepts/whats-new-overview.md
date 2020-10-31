---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 8b5794dac0017e8e876837d9058b5d2248186fc1
ms.sourcegitcommit: adc36691fd77544eeb1ec061ccfa59abffbfea9a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/31/2020
ms.locfileid: "48819673"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](changelog.md). 

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_ , podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status DG. Não use os recursos de visualização em aplicativos de produção.

## <a name="october-2020-new-and-generally-available"></a>Outubro de 2020: novo e geralmente disponível

### <a name="application"></a>Aplicativo
- Permitir [email como uma ID de login alternativa para o Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin), usando uma política de [Descoberta de Realm Inicial](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery). Uma política de Descoberta de Realm Inicial determina, depois que um usuário fornece uma ID de entrada, se deve solicitar a autenticação do usuário. Nesse caso, definir a propriedade **AlternateIdLogin** de um recurso [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) pode habilitar que um usuário conecte-se com um endereço de email.
- Obtenha as informações verificadas do editor para um [aplicativo](/graph/api/resources/application) ou [servicePrincipal](/graph/api/resources/serviceprincipal) e [ defina](/graph/api/application-setverifiedpublisher) ou [ remova](/graph/api/application-unsetverifiedpublisher) as informações verificadas do editor para um **aplicativo** .

### <a name="change-notifications"></a>Mudar notificações
Os aplicativos de produção agora podem assinar notificações de ciclo de vida do Outlook [mensagem](/graph/api/resources/message), [evento](/graph/api/resources/event) e [contato](/graph/api/resources/contact) e do Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) em ordem a [reduzir a falta de assinaturas e alterar as notificações](webhooks-lifecycle.md).

### <a name="identity-and-access"></a>Identidade e acesso
- GA de opções avançadas de consulta do sistema OData (`$count`,`$search` e `$filter`) em objetos de diretório.
- Confira exemplos que mostram o elenco do OData em objetos de diretório.
- Confira a seção Identidade e acesso das atualizações de [outubro](changelog.md#october-2020) no log de mudanças para obter as listas de APIs aprimoradas.

### <a name="teamwork"></a>Trabalho em equipe
- O GA do conjunto completo de operações CRUD para [chatMember](/graph/api/resources/conversationmember) e [aadUserConversationMember](/graph/api/resources/aaduserconversationmember). Esses recursos representam um membro em um chat ou conversa de canal, que pode ou não ser um usuário no Microsoft Azure Active Directory.
- O GA de notificações de ciclo de vida para recursos do Teams de [chatMessage](/graph/api/resources/chatmessage), para [reduzir assinaturas ausentes e notificações de alteração](webhooks-lifecycle.md).

### <a name="to-do-tasks"></a>Tarefas pendentes
O GA da [API Microsoft To-Do](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true) - use a API de tarefas em um aplicativo de produção para criar e gerenciar tarefas que fazem parte do fluxo de trabalho de um usuário, como criar uma tarefa de um email.  

### <a name="users"></a>Comercial
Obtenha novas propriedades aplicáveis ​​a um [usuário](/graph/api/resources/user) que é funcionário corporativo: data de contratação, associação organizacional, como divisão e centro de custo, e tipo de funcionário, como consultor, contratado ou fornecedor. Essas propriedades requerem a especificação do `$select`parâmetro de consulta OData na operação GET.

## <a name="october-2020-new-in-preview-only"></a>Outubro de 2020: novo apenas na pré-visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações em nuvem | Reunião online
- Diferencie a função de um participante em uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) como um participante ou apresentador, usando a propriedade **função** do tipo [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo?view=graph-rest-beta&preserve-view=true).
- Obtenha uma [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) ao [filtrar na propriedade joinWebUrl da reunião](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true#example-3-retrieve-an-online-meeting-by-joinweburl).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem

- Descontinue a ação **uploadData** em favor de [criar uma sessão de upload](/graph/api/printdocument-createuploadsession?view=graph-rest-beta&preserve-view=true) para [fazer upload de um documento](upload-data-to-upload-session.md) para uma impressora ou compartilhamento de impressora.
- Cancele a propriedade **configuração** em [printDocument](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true) em favor de uma propriedade de **configuração** semelhante em [printJob](/graph/api/resources/printjob?view=graph-rest-beta&preserve-view=true).
- Obtenha o URL do trabalho de origem ou de destino para um **printJob** que está sendo redirecionado, usando a propriedade **redirectedFrom** ou **redirectedTo** .
- Obtenha o status atual de um **printJob** usando a propriedade **estado** e a nova propriedade **detalhes** .
- Obtenha a coleção de compartilhamentos de impressora associados a uma [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) usando a relação **compartilhamentos** . 
- Substitua a propriedade **processingStateReasons** da **impressora** em favor da propriedade **status** . A propriedade **status** é do tipo [status da impressora](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) e expõe uma propriedade **detalhes** . Use a propriedade **detalhes** para identificar o motivo de uma impressora estar no estado atual.
- Cancele a propriedade **feedDirections** em [printerCapabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true) em favor da propriedade **feedOrientations** , para obter orientações de alimentação suportadas por uma impressora.
- Confira a seção de impressão na nuvem das atualizações de [outubro](changelog.md#october-2020) no log de mudanças para algumas renomeações de API, propriedades e algumas outras descontinuações.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gestão corporativa
Atualizações do Intune de [outubro](changelog.md#october-2020) para a versão beta.

### <a name="files"></a>Arquivos
[Revogar](/graph/api/permission-revokegrants?view=graph-rest-beta&preserve-view=true) o acesso à para um [listItem](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true) ou [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) concedido por meio de um link de compartilhamento.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Gerenciar [políticas de método de autenticação](/graph/api/resources/authenticationmethodspolicies-overview?view=graph-rest-beta&preserve-view=true) para identificar os usuários que podem usar métodos de autenticação multifator específicos para entrar no Azure Active Directory. Configure políticas para definir o seguinte:
  - Os tipos de chaves de segurança FIDO2 que podem ser usadas no locatário do Azure AD.
  - Os usuários ou grupos de usuários que têm permissão para usar chaves de segurança FIDO2 ou a Entrada por Telefone sem Senha para entrar no Azure AD.
- Configure um [método de autenticação de email](/graph/api/resources/emailauthenticationmethod?view=graph-rest-beta&preserve-view=true) para que os usuários possam redefinir a senha sozinhos.
- Use o [Azure AD B2C](/azure/active-directory-b2c/overview) e [escolha um mecanismo para configurar e permitir que os usuários finais se autentiquem por contas locais](/graph/api/resources/b2cauthenticationmethodspolicy?view=graph-rest-beta&preserve-view=true).
- Use o `Policy.ReadWrite.AuthenticationMethod` para ler ou gravar as políticas do método de autenticação de uma organização, como uma permissão delegada em nome de um usuário conectado ou como uma permissão de aplicativo sem ter um usuário conectado.
- Especifique em uma [política de autorização](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true) se e quem pode convidar usuários externos para uma organização.

### <a name="people-and-workplace-intelligence--insights"></a>Inteligência de pessoas e local de trabalho | Intuições 
Os administradores podem ver os [exemplos de uso de cmdlets do Windows PowerShell](insights-customize-item-insights-privacy.md#how-to-configure-item-insights-setting-via-powershell) para personalizar as configurações de percepção do item para uma organização.

### <a name="teamwork"></a>Trabalho em equipe
- Use o atributo de instância **channelCreationMode** para indicar que um [canal](https://docs.microsoft.com/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true#instance-attributes) está sendo criado para servir à migração de dados. Use o [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true) para indicar que a migração terminou, de forma que os membros possam postar e ler mensagens.
- Use o atributo de instância **teamCreationMode** para indicar que uma [equipe](https://docs.microsoft.com/graph/api/resources/team?view=graph-rest-beta&preserve-view=true#instance-attributes) está sendo criada para atender à migração. Use o [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true) para indicar que a migração terminou, de forma que as operações dos membros podem acontecer e os membros podem postar mensagens.


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
Além de obter o endereço SMTP de um [usuário](/graph/api/resources/user) por meio da propriedade de **email** , você pode definir essa propriedade e atualizar o endereço de email do usuário. 

## <a name="september-2020-new-in-preview-only"></a>Setembro de 2020: novidades somente na pré-visualização

### <a name="application"></a>Aplicativo
Crie, liste ou exclua [classificações de permissões delegadas](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true) que uma [entidade de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) expõe. Use as classificações de permissão delegada em combinação com as [configurações de consentimento do usuário](/azure/active-directory/manage-apps/configure-user-consent) para definir limites sobre quando os usuários finais têm permissão para dar consentimento aos aplicativos.

### <a name="cloud-communications"></a>Comunicações na nuvem
- A substituição da propriedade **autoAdmittedUsers** do [ onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Em vez disso, use a propriedade **lobbyBypassSettings** e seus [valores](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
- Use configurações adicionais sobre como anunciar os chamadores que ingressam em uma reunião online (propriedade **isEntryExitAnnounced** ) e permitir apresentadores específicos na reunião (propriedade **allowedPresenters** ).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- [Obtenha os documentos para cada um dos trabalhos de impressão associados a uma impressora](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true), aplicando uma `$expand` [opção de consulta do sistema OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters). 
- Filtre trabalhos de impressão pelo usuário que os criou, aplicando uma opção de`$filter` [consulta do sistema OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
As atualizações de [setembro](changelog.md#september-2020) do Intune para a versão beta.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Obtenha uma chave de recuperação do BitLocker](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true) em nome do usuário conectado que é o proprietário do dispositivo ou em uma função adequada. Obter uma chave de recuperação gera um [log de auditoria](/azure/active-directory/reports-monitoring/concept-audit-logs), em paridade com a experiência do usuário final.
- Obtenha a quantidade total e usada da [cota do diretório](/graph/api/resources/directorysizequota?view=graph-rest-beta&preserve-view=true) de uma [organização](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true), por meio da propriedade **directorySizeQuota** .

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
É possível incluir uma [agenda](/graph/api/resources/requestschedule?view=graph-rest-beta&preserve-view=true) ao solicitar ou remover uma [atribuição de um usuário para um pacote do Access](/graph/api/resources/accesspackageassignment?view=graph-rest-beta&preserve-view=true), que especifica o acesso aos grupos, aplicativos ou sites do SharePoint.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
As organizações podem [obter](/graph/api/continuousaccessevaluationpolicy-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/continuousaccessevaluationpolicy-update?view=graph-rest-beta&preserve-view=true) a [política de avaliação de acesso contínuo](/graph/api/resources/continuousAccessEvaluationPolicy?view=graph-rest-beta&preserve-view=true) para gerenciar sessões de autenticação em tempo real.

### <a name="search"></a>Pesquisar

- Use recursos adicionais no [API de Pesquisa da Microsoft](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true) para OneDrive, SharePoint, conectores do Microsoft Graph: 

  - Obtenha [tipos adicionais](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true#scope-search-based-on-entity-types) de conteúdo do OneDrive e do Microsoft Office SharePoint Online: **unidade** , **lista** , **listItem** e **site** . 
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


## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote em novos recursos no [Microsoft Graph User Voice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de visualização **_prévia_** . As atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)** , se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
