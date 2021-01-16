---
title: Destaques de versões anteriores no Microsoft Graph
description: O que havia de novo no Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 0414c2414a6765c7e0c29114c2239d15bbe71cea
ms.sourcegitcommit: 8f156a80b2f76cefa271a536c238721aff6931bf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883414"
---
# <a name="highlights-of-earlier-releases"></a>Destaques de versões anteriores

## <a name="november-2020-new-and-generally-available"></a>Novembro de 2020: Novo e geralmente disponível

### <a name="cloud-communications"></a>Comunicações na nuvem
- O GA da propriedade **função** do tipo [meetingParticipantInfo](/graph/api/resources/meetingParticipantInfo), que distingue a função de um participante em uma [reunião online](/graph/api/resources/onlinemeeting) como um participante ou apresentador.
- O GA da propriedade **lobbyBypassSettings** e seus [valores](/graph/api/resources/lobbybypasssettings#lobbybypassscope-values) para admitir usuários para uma reunião online.
- O GA da propriedade **isEntryExitAnnounced** para personalizar as configurações de apresentação de autores de chamada ou de sair de uma reunião online.
- O GA da propriedade **allowedPresenters** para permitir apresentadores específicos na reunião.

### <a name="search"></a>Pesquisar
- O GA da [consulta da API](/graph/api/resources/search-api-overview) Pesquisa da Microsoft, oferecendo suporte à pesquisa em escopo dos seguintes tipos de dados:
  - [Mensagens do Outlook](./search-concept-messages.md)
  - [Eventos do calendário do Outlook](./search-concept-events.md)
  - [Recursos do Microsoft OneDrive e do Microsoft Office SharePoint Online](./search-concept-files.md).

### <a name="teamwork"></a>Trabalho em equipe

- GA de permissões de consentimento específicas de recurso (RSC). As permissões RSC permitem que os proprietários da equipe concedam consentimento granular a um aplicativo de produção para acessar e/ou modificar dados específicos de uma equipe, como por exemplo, ler as configurações da equipe ou modificar nomes de canal, descrições e outras configurações.
- GA de APIs que se aplicam a um [canal](/graph/api/resources/channel) ou mensagens dentro de um canal. As APIs incluem:
  - [Criar](/graph/api/conversationmember-add) ou [excluir](/graph/api/conversationmember-delete) um membro de conversa de um canal.
  - [Atualizar a função de um membro](/graph/api/conversationmember-update) em um canal.
  - Receber uma mensagem específica ou todas as mensagens em um canal.
  - Receber uma resposta específica ou todas as respostas em um canal.
  - [Acompanhar mensagens novas ou atualizadas em um canal](/graph/api/chatmessage-delta).


## <a name="november-2020-new-in-preview-only"></a>Novembro de 2020: Novidades somente na pré-visualização

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
Estreia da [API de computador na nuvem](/graph/api/resources/virtualendpoint?view=graph-rest-beta&preserve-view=true) que permite que as organizações provisionem e gerenciem as máquinas virtuais para os funcionários. Use-o em conjunto com a API do Intune para gerenciar os pontos de extremidade físicos e virtuais.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
[Inscreva-se para alterar as notificações](webhooks.md) em uma [definição de tarefa de impressão](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gestão corporativa
As atualizações de [Novembro](changelog.md#november-2020) do Intune para a versão beta.

### <a name="identity-and-access"></a>Identidade e acesso
- Especificar URLs para envio de tokens de entrada de usuário e URIs de códigos de autorização e tokens de acesso, na propriedade **spa** de [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true).
- Personalize a aparência das telas de entrada do Azure Active Directory usando as [propriedades de identidade visual organização](/graph/api/resources/organizationalbrandingproperties?view=graph-rest-beta&preserve-view=true). As organizações podem personalizar com base na localidade para usuários específicos.

### <a name="identity-and-access--governance"></a>Identidade e acesso | Governança
A estreia da [API de revisão de acesso para a associação de grupo](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) para revisar regularmente o acesso de usuários, certifique-se de que apenas as pessoas certas tenham acesso contínuo e gerenciem os membros do grupo de forma eficiente.

### <a name="search"></a>Pesquisar
Você pode agregar resultados de pesquisa de tipo numérico ou cadeia de caracteres que são importados por [conectores do Microsoft Graph](/microsoftsearch/connectors-overview) e que são configurados para serem refináveis no [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Veja mais informações sobre [refinar resultados de pesquisa usando agregações](search-concept-aggregation.md).

## <a name="october-2020-new-and-generally-available"></a>Outubro de 2020: novo e geralmente disponível

### <a name="application"></a>Aplicativo
- Permitir [email como uma ID de login alternativa para o Azure Active Directory](/azure/active-directory/authentication/howto-authentication-use-email-signin), usando uma política de [Descoberta de Realm Inicial](/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#home-realm-discovery). Uma política de Descoberta de Realm Inicial determina, depois que um usuário fornece uma ID de entrada, se deve solicitar a autenticação do usuário. Nesse caso, definir a propriedade **AlternateIdLogin** de um recurso [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy) pode habilitar que um usuário conecte-se com um endereço de email.
- Obtenha as informações verificadas do fornecedor para um [aplicativo](/graph/api/resources/application) ou [servicePrincipal](/graph/api/resources/serviceprincipal) e [defina](/graph/api/application-setverifiedpublisher) ou [remova](/graph/api/application-unsetverifiedpublisher) as informações verificadas do fornecedor para um **aplicativo**.

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
- Obtenha o URL do trabalho de origem ou de destino para um **printJob** que está sendo redirecionado, usando a propriedade **redirectedFrom** ou **redirectedTo**.
- Obtenha o status atual de um **printJob** usando a propriedade **estado** e a nova propriedade **detalhes**.
- Obtenha a coleção de compartilhamentos de impressora associados a uma [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) usando a relação **compartilhamentos**. 
- Substitua a propriedade **processingStateReasons** da **impressora** em favor da propriedade **status**. A propriedade **status** é do tipo [status da impressora](/graph/api/resources/printerstatus?view=graph-rest-beta&preserve-view=true) e expõe uma propriedade **detalhes**. Use a propriedade **detalhes** para identificar o motivo de uma impressora estar no estado atual.
- Cancele a propriedade **feedDirections** em [printerCapabilities](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true) em favor da propriedade **feedOrientations**, para obter orientações de alimentação suportadas por uma impressora.
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
- Use o atributo de instância **channelCreationMode** para indicar que um [canal](/graph/api/resources/channel?preserve-view=true&view=graph-rest-beta#instance-attributes) está sendo criado para servir à migração de dados. Use o [completeMigration](/graph/api/channel-completemigration?view=graph-rest-beta&preserve-view=true) para indicar que a migração terminou, de forma que os membros possam postar e ler mensagens.
- Use o atributo de instância **teamCreationMode** para indicar que uma [equipe](/graph/api/resources/team?preserve-view=true&view=graph-rest-beta#instance-attributes) está sendo criada para atender à migração. Use o [completeMigration](/graph/api/team-completemigration?view=graph-rest-beta&preserve-view=true) para indicar que a migração terminou, de forma que as operações dos membros podem acontecer e os membros podem postar mensagens.

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

### <a name="application"></a>Aplicativo
Crie, liste ou exclua [classificações de permissões delegadas](/graph/api/resources/delegatedpermissionclassification?view=graph-rest-beta&preserve-view=true) que uma [entidade de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) expõe. Use as classificações de permissão delegada em combinação com as [configurações de consentimento do usuário](/azure/active-directory/manage-apps/configure-user-consent) para definir limites sobre quando os usuários finais têm permissão para dar consentimento aos aplicativos.

### <a name="cloud-communications"></a>Comunicações na nuvem
- A substituição da propriedade **autoAdmittedUsers** do [ onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true). Em vez disso, use a propriedade **lobbyBypassSettings** e seus [valores](/graph/api/resources/lobbybypasssettings?view=graph-rest-beta&preserve-view=true#lobbybypassscope-values).
- Use configurações adicionais sobre como anunciar os chamadores que ingressam em uma reunião online (propriedade **isEntryExitAnnounced**) e permitir apresentadores específicos na reunião (propriedade **allowedPresenters**).

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- [Obtenha os documentos para cada um dos trabalhos de impressão associados a uma impressora](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true), aplicando uma `$expand` [opção de consulta do sistema OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters). 
- Filtre trabalhos de impressão pelo usuário que os criou, aplicando uma opção de`$filter` [consulta do sistema OData](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true#optional-query-parameters).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
As atualizações de [setembro](changelog.md#september-2020) do Intune para a versão beta.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Obtenha uma chave de recuperação do BitLocker](/graph/api/bitlockerrecoverykey-get?view=graph-rest-beta&preserve-view=true) em nome do usuário conectado que é o proprietário do dispositivo ou em uma função adequada. Obter uma chave de recuperação gera um [log de auditoria](/azure/active-directory/reports-monitoring/concept-audit-logs), em paridade com a experiência do usuário final.
- Obtenha a quantidade total e usada da [cota do diretório](/graph/api/resources/directorysizequota?view=graph-rest-beta&preserve-view=true) de uma [organização](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true), por meio da propriedade **directorySizeQuota**.

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
- Use a propriedade de navegação **members** para adicionar membros a uma equipe com maior confiabilidade e latência menor.
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
- Use a propriedade do **arquivo** para navegar até um [contrato personalizado](/graph/api/resources/agreementfile?view=graph-rest-beta&preserve-view=true) para termos de uso. Não use a propriedade de **arquivos**.
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


## <a name="july-2020-new-and-generally-available"></a>Julho de 2020: novos e disponíveis para o público em geral

### <a name="calendar"></a>Calendário
GA do recurso que permite aos organizadores permitir propostas de horário alternativo para reuniões ou convites para [propor novos horários para uma reunião](outlook-calendar-meeting-proposals.md) quando eles [aceitarem provisoriamente](/graph/api/event-tentativelyaccept?view=graph-rest-1.0&preserve-view=true&preserve-view=true) ou [recusarem](/graph/api/event-decline?view=graph-rest-1.0&preserve-view=true&preserve-view=true) um evento.

### <a name="change-notifications"></a>Notificações de alteração
Removida do recurso [changeNotification](/graph/api/resources/changenotification) a propriedade **sequenceNumber** introduzida erroneamente.

### <a name="groups"></a>Grupos
DG das seguintes propriedades para a entidade [group](/graph/api/resources/group): **assignedLabels**, **expirationDateTime**, **membershipRule**, **membershipRuleProcessingState**, **preferredLanguage** e **theme**.

### <a name="identity-and-access"></a>Identidade e acesso
- Remover um usuário como proprietário registrado ou usuário de um [dispositivo](/graph/api/resources/device).
- Acompanhe as alterações de representações locais de aplicativos recém-criadas, atualizadas ou deletadas (representada por recursos[servicePrincipals](/graph/api/resources/serviceprincipal)) e permissões delegadas concedidas (representadas por recursos[oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant)) sem executar uma leitura completa de toda a coleção de recursos.
- GA da [política para reforçar o padrão de segurança](/graph/api/resources/identitysecuritydefaultsenforcementpolicy) que protege as organizações contra ataques comuns.

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- GA de [políticas de acesso condicional](/graph/api/resources/conditionalAccessPolicy) que são regras personalizadas que definem um cenário de acesso.
- GA de [posições nomeadas](/graph/api/resources/namedLocation) representando regras personalizadas que definem os locais de rede usados em uma política de acesso condicional.

### <a name="schema-extensions"></a>Extensões de esquema
O recurso [extensões de esquema](/graph/api/resources/schemaextension) já está disponível para o público em geral no[Microsoft Cloud for US Government](./deployments.md).

### <a name="teamwork"></a>Trabalho em equipe
Use as permissões delegadas de `TeamsAppInstallation.ReadForTeam` ou `TeamsAppInstallation.ReadWriteForTeam` ou permissões de aplicativo de `TeamsAppInstallation.ReadForTeam.All` ou `TeamsAppInstallation.ReadWriteForTeam.All` para [listar aplicativos instalados em uma equipe](/graph/api/teamsappinstallation-list).

## <a name="july-2020-new-in-preview-only"></a>Julho de 2020: novos apenas na visualização

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use a operação [atualizar](/graph/api/onlinemeeting-update?view=graph-rest-beta&preserve-view=true&preserve-view=true) para atualizar **startDateTime**, **endDateTime**, **participantes**, ou propriedade de **assunto** de uma [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true&preserve-view=true).
- Inscreva-se para receber notificações sobre alterações na disponibilidade de um usuário do Microsoft Teams, conforme representado pelo recurso [presence](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communications--call-records"></a>Comunicação em nuvem | Gravação
- [Obtenha](/graph/api/callrecords-callrecord-getpstncalls?view=graph-rest-beta&preserve-view=true) os registros de chamadas da rede pública de telefonia comutada (PSTN).
- [Obtenha](/graph/api/callrecords-callrecord-getdirectroutingcalls?view=graph-rest-beta&preserve-view=true) os registros de chamadas de roteamento direto.

### <a name="compliance--ediscovery"></a>Conformidade | Descoberta eletrônica
Estréia dos [Casos de descoberta eletrônica](/graph/api/resources/ediscoverycase?view=graph-rest-beta&preserve-view=true) que podem conter responsáveis, bloqueios, coleções, conjuntos de revisão, e exportações que podem ser usados como evidência em casos jurídicos.
Os aplicativos agora podem [consultar](/graph/api/resources/reviewsetquery?view=graph-rest-beta&preserve-view=true) e [revisar o conjunto de dados](/graph/api/resources/reviewset?view=graph-rest-beta&preserve-view=true) coletado para uso em litígio, investigação ou solicitação regulatória. Esse estreia faz parte da [Descoberta Eletrônica Avançada](/microsoft-365/compliance/overview-ediscovery-20?view=o365-worldwide&preserve-view=true)do Microsoft 365.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Use as permissões do aplicativo `Printer.ReadWrite.All` e a [codificação do IPP (Protocolo de Impressão via Internet)](https://tools.ietf.org/html/rfc8010) para [atualizar uma impressora ](/graph/api/printer-update?view=graph-rest-beta&preserve-view=true).
- Use uma das permissões de aplicativo, `PrintJob.ReadBasic.All`, `PrintJob.Read.All`, `PrintJob.ReadWriteBasic.All`ou `PrintJob.ReadWrite.All`, para [obter um trabalho de impressão](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true) ou [listar trabalhos de impressão para uma impressora](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- Quando [obtiver um trabalho de impressão](/graph/api/printjob-get?view=graph-rest-beta&preserve-view=true), use `$expand` para obter [tarefas de impressão](/graph/api/resources/printtask?view=graph-rest-beta&preserve-view=true) que estão executando ou que foram executadas no trabalho. Imprimir tarefas, [definições de tarefas](/graph/api/resources/printtaskdefinition?view=graph-rest-beta&preserve-view=true)e [disparadores de tarefas](/graph/api/resources/printtasktrigger?view=graph-rest-beta&preserve-view=true) são usados em [impressão segura](universal-print-concept-overview.md#extending-universal-print-to-support-pull-printing).
- [Redirecione um trabalho de impressão](/graph/api/printjob-redirect?view=graph-rest-beta&preserve-view=true) para uma impressora diferente, como parte da impressão segura.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [julho](changelog.md#july-2020) em beta.

### <a name="groups"></a>Grupos
Use a propriedade **isAssignableToRole** de um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) do Microsoft 365 e a defina durante a criação de um grupo para indicar se ele pode ser atribuído a uma função do Azure AD. Isso [ajuda a gerenciar as atribuições de função no Azure AD](/azure/active-directory/users-groups-roles/roles-groups-concept), de modo que, em vez de atribuir um usuário individual a uma função do Azure AD, um administrador global ou um administrador de funções privilegiadas pode criar um grupo do Microsoft 365 e atribuir o grupo a essa função, para que quando os usuários se unam ao _grupo_, eles recebam a função pretendida indiretamente.

### <a name="identity-and-access"></a>Identidade e acesso
- [Adquira um token de acesso](/graph/api/synchronization-synchronization-acquireAccessToken?view=graph-rest-beta&preserve-view=true) para autorizar o serviço de provisionamento do Azure AD para provisionar usuários em um aplicativo.
- [Obtenha](/graph/api/entitlementmanagementsettings-get?view=graph-rest-beta&preserve-view=true) ou [atualize](/graph/api/entitlementmanagementsettings-update?view=graph-rest-beta&preserve-view=true) as configurações de gerenciamento de qualificação que controlam o acesso a grupos, aplicativos e sites do SharePoint Online para usuários internos e externos à sua organização. 

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e entrada
- Inclua os níveis de risco do usuário (`low`, `medium`, `high`, `none`) como consideração para aplicar uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- [Use a alteração de senha como um controle Grant](/graph/api/resources/conditionalaccessgrantcontrols?view=graph-rest-beta&preserve-view=true#special-considerations-when-using-passwordchange-as-a-control) para passar uma política de acesso condicional.
- Use um [provedor de conexão de ID aberta](/graph/api/resources/openidconnectprovider?view=graph-rest-beta&preserve-view=true) (ODIC) como um provedor de identidade em um locatário do Azure AD e um locatário do Azure AD B2C. Sua propriedade **claimsMapping** permite que o Azure AD [mapeie as declarações](/graph/api/resources/claimsmapping?view=graph-rest-beta&preserve-view=true) de um provedor OIDC para as declarações que o Azure AD reconhece e usa.

### <a name="people-and-workplace-intelligence--insights"></a>Inteligência social e do ambiente de trabalho | Ideias
Use mais o [controle de privacidade granular](insights-customize-item-insights-privacy.md) sobre a disponibilidade e a exibição das [informações do item](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true) no Microsoft 365. Essas informações representam as relações entre um usuário e documentos no OneDrive for Business, calculadas usando uma análise avançada e técnicas de aprendizado de máquina. 

### <a name="people-and-workplace-intelligence--profile-card-customization"></a>Inteligência de pessoas e local de trabalho | Personalização de cartão de perfil
Os administradores podem [personalizar as propriedades expostas no cartão de perfil de suas organizações](add-properties-profilecard.md) usando a API para [propriedade de cartão de perfil](/graph/api/resources/profilecardproperty?view=graph-rest-beta&preserve-view=true).

### <a name="sites-and-lists"></a>Sites e listas
Acesse a taxonomia do [repositório de termos](/graph/api/resources/termstore-store?view=graph-rest-beta&preserve-view=true) a hierarquia que consite em recursos de [grupo](/graph/api/resources/termstore-group?view=graph-rest-beta&preserve-view=true), [definição](/graph/api/resources/termstore-set?view=graph-rest-beta&preserve-view=true), e [termo](/graph/api/resources/termstore-term?view=graph-rest-beta&preserve-view=true), e [relacione](/graph/api/resources/termstore-relation?view=graph-rest-beta&preserve-view=true) recursos entre os termos.

### <a name="workbooks-and-charts"></a>Pastas de trabalho e gráficos
[Obtenha o status e todos os resultados](/graph/api/workbookoperation-get?view=graph-rest-beta&preserve-view=true) de uma operação [de longa execução](/graph/api/resources/workbookoperation?view=graph-rest-beta&preserve-view=true) em uma [pasta de trabalho](/graph/api/resources/workbook?view=graph-rest-beta&preserve-view=true).



## <a name="june-2020-new-and-generally-available"></a>Junho de 2020: novos e disponíveis para o público em geral

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
- Use o cabeçalho HTTP `Accept-Language`ao [criar uma reunião online](/graph/api/application-post-onlinemeetings?view=graph-rest-1.0&preserve-view=true&preserve-view=true) para fornecer informações de participação baseadas no local.
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-1.0&preserve-view=true&preserve-view=true) para retornar uma reunião online que tenha um valor **externalId** específico ou, caso nenhum valor desse tipo exista, para simplificar a incorporação da reunião resultante a um calendário de terceiros.

### <a name="files"></a>Arquivos
- Suporte aprimorado à sincronização:
  - Use a propriedade **pendingOperations** para identificar quaisquer [operações](/graph/api/resources/pendingoperations) que possam atualizar o conteúdo binário de um arquivo [driveItem](/graph/api/resources/driveitem) e que estejam pendentes.
  - [Restaure](/graph/api/driveitem-restore) um **driveItem** que tenha sido excluído e esteja na lixeira do OneDrive pessoal.
- Obtenha ou defina a orientação de uma [foto](/graph/api/resources/photo). A configuração é compatível com o OneDrive Personal.
- Use o Algoritmo de Hash Seguro (SHA-256) para aprimorar a segurança e a integridade dos dados do [arquivo](/graph/api/resources/file).
- Use o parâmetro `deferCommit` para adiar a criação final ao [carregar geralmente um arquivo grande](/graph/api/driveitem-createuploadsession) no OneDrive for Business, até que um aplicativo faça uma solicitação para concluir o carregamento.
- Use a propriedade **fileSize** para fornecer uma estimativa como parte do parâmetro do **item**, de modo a fazer uma verificação de cota antes de [carregar um arquivo](/graph/api/driveitem-createuploadsession) no OneDrive pessoal.
- Localize [storagePlanInformation](/graph/api/resources/storageplaninformation) por meio da propriedade **cota** de um recurso de [unidade](/graph/api/resources/drive) para ver se existem planos de uma cota de armazenamento mais alta disponíveis.

### <a name="groups"></a>Grupos
Use as permissões de aplicativo `Group.Read.All` e `Group.ReadWrite.All` para obter recursos de uma [conversa](/graph/api/resources/conversation) do grupo e de uma [sequência de conversa](/graph/api/resources/conversationthread).

### <a name="identity-and-access"></a>Identidade e acesso 
- Disponibilidade generalizada de dois conjuntos de APIs de [proteção de identidade](/graph/api/resources/identityprotectionroot): APIs de [detecção de riscos](/graph/api/resources/riskdetection) e de [usuário arriscado](/graph/api/resources/riskyuser).

### <a name="security"></a>Segurança
- Rastreie o seguinte como propriedades de um [alerta](/graph/api/resources/alert?view=graph-rest-1.0&preserve-view=true&preserve-view=true):
  - IDs de incidentes relacionados ao alerta.
  - Identificar um [recurso](/graph/api/resources/securityResource?view=graph-rest-1.0&preserve-view=true#securityresourcetype-values) como atacado ou como um recurso relacionado no alerta.
  - Especificar os locais de origem e destino de uma [conexão de rede](/graph/api/resources/networkconnection?view=graph-rest-1.0&preserve-view=true) relacionada ao alerta.

### <a name="sites-and-lists"></a>Sites e listas
Especifique dados de localização geográfica em uma [definição de coluna](/graph/api/resources/columndefinition) para um recurso de uma [lista](/graph/api/resources/list) do SharePoint.

### <a name="teamwork"></a>Trabalho em equipe
- Use a permissão delegada [AppCatalog.Read.All](./permissions-reference.md#appcatalog-resource-permissions) para listar [aplicativos](/graph/api/resources/teamsapp?view=graph-rest-1.0&preserve-view=true) do catálogo de aplicativos do Microsoft Teams.
- [Obtenha informações sobre a pasta](/graph/api/channel-get-filesfolder) que mapeia para a guia **Arquivos** de um [canal](/graph/api/resources/channel) do Teams.
- [Obtenha o do canal padrão](/graph/api/team-get-primarychannel) — rotulado como **Geral** — de uma [equipe](/graph/api/resources/team).


## <a name="june-2020-new-in-preview-only"></a>Junho de 2020: novos apenas na visualização

### <a name="calendar"></a>Calendário
Além de monitorar as alterações incrementais de eventos em um **calendarView** (um conjunto ou eventos delimitados por datas de início _e_ fim), use a função [delta](/graph/api/event-delta?view=graph-rest-beta&preserve-view=true) nos eventos de uma caixa de correio do usuário ou eventos em um calendário específico do usuário.

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
[Obtenha o status de presença](/graph/api/presence-get?view=graph-rest-beta&preserve-view=true) de todos os usuários em uma organização ou de um usuário específico na organização.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Especificar as [margens de impressão](/graph/api/resources/printmargin?view=graph-rest-beta&preserve-view=true) ao configurar um [documento para impressão](/graph/api/resources/printdocument?view=graph-rest-beta&preserve-view=true).
- Compatível com os seguintes [recursos da impressora](/graph/api/resources/printercapabilities?view=graph-rest-beta&preserve-view=true):
  - instruções de alimentação
  - impressão de intervalos de páginas
  - resolução da impressão em DPIs
  - tamanho máximo da fila de tarefas de impressão em bytes
  - compartimentos de entrada
  - margens
  - ordenação
  - escala do documento
- Compatível com a resolução da impressão (DPI) e com a escala do documento como parte das [configurações padrão da impressora](/graph/api/resources/printerdefaults?view=graph-rest-beta&preserve-view=true).
- Compatível com as seguintes [configurações do documento](/graph/api/resources/printerdocumentconfiguration?view=graph-rest-beta&preserve-view=true):
  - compartimentos de entrada
  - compartimentos de saída
  - tamanhos de papel
  - margens
  - tipos de papel
  - acabamentos como grampeamento ou encadernação
  - páginas por folha
  - layout multipáginas especificando a direção do layout das páginas na folha
  - ordenação
  - escala
- Expandir os documentos ao [listar as tarefas de impressão](/graph/api/printer-list-jobs?view=graph-rest-beta&preserve-view=true).
- [Registre uma impressora ]() e use o recurso [printerCreateOperation](/graph/api/resources/printercreateoperation?view=graph-rest-beta&preserve-view=true) para monitorar e verificar o registro da impressora.
- [Obtenha a operação de registro](/graph/api/printoperation-get?view=graph-rest-beta&preserve-view=true) da impressora de longa duração no usuário atual ou no locatário do aplicativo.
- Algumas propriedades e tipos de enumeração renomeados; confira os detalhes nas atualizações do log de alterações da impressão em nuvem do mês de [junho](changelog.md#june-2020).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações do Intune em [junho](changelog.md#june-2020) — em beta.

### <a name="education"></a>Educação
- Possibilidade de usar permissões delegadas `EduRoster.ReadBasic` para [obter](/graph/api/educationuser-get?view=graph-rest-beta&preserve-view=true) a ID de um(a) [professor(a)](/graph/api/resources/educationteacher?view=graph-rest-beta&preserve-view=true) ou [aluno(a)](/graph/api/resources/educationstudent?view=graph-rest-beta&preserve-view=true) em um programa de uma fonte externa, na forma de uma propriedade **externalId**.
- Use a propriedade **externalSource** para monitorar o valor `lms` se uma [organização](/graph/api/resources/educationorganization?view=graph-rest-beta&preserve-view=true) de ensino ou [aula](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) forem criados a partir de um sistema de gerenciamento de aprendizagem (LMS).

### <a name="identity-and-access"></a>Identidade e acesso
- Os profissionais de TI podem usar os recursos do [conector](/graph/api/resources/connector?view=graph-rest-beta&preserve-view=true) que sejam agentes leves para se conectar ao [Proxy de Aplicativos do Azure AD](/azure/active-directory/manage-apps/what-is-application-proxy) e [publicar aplicativos web locais externamente](/graph/api/resources/onpremisespublishing?view=graph-rest-beta&preserve-view=true)para que os usuários remotos de suas organizações possam acessá-los de forma segura.
- Gerenciar uma [política de autenticação](/graph/api/resources/authenticationflowspolicy?view=graph-rest-beta&preserve-view=true) no nível de locatário para ativar ou desativar um [serviço autoatendimento de cadastramento](/graph/api/resources/selfservicesignupauthenticationflowconfiguration?view=graph-rest-beta&preserve-view=true) para usuários externos.
- [Provisionar uma conta de usuário sob demanda](/graph/api/synchronization-synchronizationjob-provision-on-demand?view=graph-rest-beta&preserve-view=true) e ser capaz de especificar quais objetos provisionar e quais regras de sincronização executar.

### <a name="search"></a>Busca
- Utilizar os aperfeiçoamentos de uma [propriedade](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true) em um [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true): **isRefinable** para habilitar a filtragem dos resultados de busca e obter um controle mais refinado da experiência de busca, além de **aliases** e **rótulos** para maior relevância.
- Capacidade de especificar até 128 recursos de **propriedades** em um **esquema**.
- Use [get externalItem](/graph/api/externalitem-get?view=graph-rest-beta&preserve-view=true) para fins de diagnóstico.

### <a name="users"></a>Usuários
- Use a propriedade **userPurpose** em [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) para identificar e diferenciar uma caixa de correio para um único usuário de uma caixa de correio compartilhada e do equipamento de caixa de correio no Exchange Online. 
- Use as [configurações de usuário](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) para [obter](/graph/api/regionalandlanguagesettings-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/regionalandlanguagesettings-update?view=graph-rest-beta&preserve-view=true) [idiomas preferenciais e configurações regionais](/graph/api/resources/regionalandlanguagesettings?view=graph-rest-beta&preserve-view=true).
- As configurações de usuário são uma relação acessível por meio do [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) que permite uma experiência de usuário consistente em todos os aplicativos, bastando tocar no perfil de usuário do Azure AD para refletir as mesmas preferências do usuário. Veja [como as configurações de usuário diferem das configurações da caixa de correio](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true#user-preferences-for-languages-and-regional-formats). 


## <a name="may-2020-new-and-generally-available"></a>Maio de 2020: novos e disponíveis para o público em geral

### <a name="calendar--place"></a>Calendário | Local
GA da [API de locais](/graph/api/resources/place) na v1.0: use essa API em aplicativos de produção para obter, atualizar ou excluir uma [sala](/graph/api/resources/room) ou [lista de salas](/graph/api/resources/roomlist) em um locatário. [Saiba mais](outlook-calendar-concept-overview.md#build-apps-with-location-awareness-and-provide-intelligent-context) sobre a API de locais.

### <a name="change-notifications"></a>Notificações de alteração
- Inscreva-se para alterar as notificações no Microsoft Cloud for US Government.

### <a name="cloud-communications--call-records"></a>Comunicações na nuvem | Registros de chamadas
- GA da [API de registros de chamadas](/graph/api/resources/callrecords-api-overview?view=graph-rest-1.0&preserve-view=true): use o recurso [callRecord](/graph/api/resources/callrecord?view=graph-rest-1.0&preserve-view=true) para obter os metadados de chamadas e reuniões online no Microsoft Teams e no Skype.
- Inscreva-se para [alterar notificações](./webhooks.md) de alterações para todos os recursos de **callRecord** em uma organização.
- [Liste as sessões](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true) em um **callRecord** e, opcionalmente, [expanda cada sessão para listar os segmentos](/graph/api/callrecords-session-list?view=graph-rest-1.0&preserve-view=true#example-2-get-session-list-with-segments) no registro de chamadas.
- Suporte para 60 GHz (`frequency60GHz`) e valores de banda de WiFi de `unknownFutureValue` para um ponto de extremidade de mídia em um segmento.
- Suporte à caixa postal como um possível tipo de ponto de extremidade do lado do serviço em um [segmento](/graph/api/resources/callrecords-segment) de comunicação.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [maio](changelog.md#may-2020) do Intune v1.0.

### <a name="graph-explorer"></a>Explorador do Graph
Use os vários novos recursos do [Explorador do Graph](https://developer.microsoft.com/pt-BR/graph/graph-explorer) que aprimoram o aprendizado e a prototipagem na área restrita. Por exemplo:
- Exiba trechos de código que correspondam à consulta da API REST inserida em C#, Java, JavaScript e Objective C.
- Conecte-se com um locatário, exiba e copie um token de acesso para seu aplicativo cliente REST favorito.

Para mais detalhes, confira [O novo Explorador do Graph já está disponível](https://developer.microsoft.com/graph/blogs/new-graph-explorer-is-now-ga/).

### <a name="groups"></a>Grupos
- Agora, a sincronização do diretório local com o Azure Active Directory via Azure AD Connect retorna as propriedades **onPremisesDomainName**, **onPremisesNetBiosName** e **onPremisesSamAccountName** como parte do recurso de [grupo](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true).
- Inscreva-se para alterar as notificações de recursos de [grupo](/graph/api/resources/group) no Microsoft Cloud China operado pela 21Vianet.

### <a name="identity-and-access"></a>Identidade e acesso
- GA da API de entidades de serviço na v1.0: use o recurso [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true) em aplicativos de produção para gerenciar programaticamente instâncias de aplicativos e controlar o que um aplicativo pode fazer em seu locatário. Você pode controlar quem pode usar um aplicativo, quais recursos o aplicativo tem acesso, como a adição de credenciais de senha, a expiração de certificados, e o gerenciamento de permissões delegadas e atribuições de funções de aplicativos.
- GA da API [appRoleAssignment](/graph/api/resources/appRoleAssignment?view=graph-rest-1.0&preserve-view=true) que registra a atribuição de um [appRole](/graph/api/resources/approle?view=graph-rest-1.0&preserve-view=true) (representando a declaração de `roles` em tokens de ID e tokens de acesso) a um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), [grupo](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) ou [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0&preserve-view=true).
- Use o Facebook como provedor de identidade no Azure Active Directory.
- Use a permissão delegada ou de aplicativo do`AppRoleAssignment.ReadWrite.All` para permitir que um aplicativo gerencie concessões de permissões de aplicativo para qualquer API (incluindo o Microsoft Graph) e atribuições de aplicativo para qualquer aplicativo, respectivamente com ou sem o usuário conectado.


### <a name="microsoft-graph-sdks"></a>SDKs do Microsoft Graph
Confira as novas diretrizes de SDK em:
- [Paginação](./sdks/paging.md)
- [Envio em lote](./sdks/batch-requests.md)
- [Carregando arquivos grandes no OneDrive](./sdks/large-file-upload.md)
- [Personalizando o cliente do serviço SDK por meio dos componentes middleware HTTP](./sdks/customize-client.md).

### <a name="teamwork"></a>Trabalho em equipe
- Se o seu cenário envolver reuniões online no Teams, confira as novas diretrizes sobre [como escolher](choose-online-meeting-api.md) entre a [API de calendário](outlook-calendar-online-meetings.md) e a [API de comunicações na nuvem](cloud-communications-online-meetings.md) para criar e ingressar em reuniões online.
- [Enviar](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) e [responder](/graph/api/channel-post-messagereply?view=graph-rest-1.0&preserve-view=true) mensagens em um [canal](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true).
- Obtenha a localização dos arquivos do OneDrive for Business de um [canal](/graph/api/resources/channel?view=graph-rest-1.0&preserve-view=true), usando a propriedade de navegação **fileFolder**.

### <a name="teamwork--shifts"></a>Trabalho em equipe | Turnos
GA da [API de turnos](/graph/api/resources/shift?view=graph-rest-1.0&preserve-view=true) na v1.0: use esta API em aplicativos de produção para criar, atualizar e gerenciar cronogramas de funcionários da linha de frente, permitindo que eles estejam em contato e colaborem efetivamente.

### <a name="users"></a>Usuários
- Inscreva-se para alterar notificações de recursos de [usuário](/graph/api/resources/user) no Microsoft Cloud China operado pela 21Vianet.
- Acompanhe o status e a data/hora da última alteração de status de um usuário externo, que foi [convidado](/graph/api/invitation-post?view=graph-rest-1.0&preserve-view=true) a ingressar na organização, usando as propriedades **externalUserState** e **externalUserStateChangeDateTime** do recurso de **usuário**.

## <a name="may-2020-new-in-preview-only"></a>Maio de 2020: novo somente para visualização

### <a name="change-notifications"></a>Notificações de alteração
- Use os tipos esquematizados formalmente [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta&preserve-view=true) e [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta&preserve-view=true) para processar notificações de alteração de recursos. 
- Acompanhe se as notificações estão em sequência ou se uma notificação está ausente, usando a propriedade **sequenceNumber** no recurso **changeNotification**.

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem
- Os recursos da [impressora](/graph/api/resources/printer?view=graph-rest-beta&preserve-view=true) e do [printerShare](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) agora estão em paridade e têm as mesmas propriedades.
- Algumas limpezas de nomes de tipos e de propriedades sobre compartilhamentos da impressora:
  - Use a propriedade de navegação **compartilhada** de [impressão](/graph/api/resources/print?view=graph-rest-beta&preserve-view=true) para obter a lista de compartilhamentos de impressora registrados no locatário. 
  - Veja os detalhes no changelog de [maio](changelog.md#may-2020).

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [maio](changelog.md#may-2020) do Intune beta.

### <a name="groups"></a>Grupos
- [Avalie](/graph/api/group-evaluatedynamicmembership?view=graph-rest-beta&preserve-view=true) se um usuário ou dispositivo é ou seria membro de um grupo dinâmico, usando a regra existente do [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) ou uma regra especificada. As [associações dinâmicas baseadas em regras](/azure/active-directory/users-groups-roles/groups-dynamic-membership) reduz a sobrecarga administrativa na adição e remoção de membros.
- Ao criar um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) do Microsoft 365, configure os comportamentos do grupo especificando-os na propriedade **resourceBehaviorOptions**. Por exemplo, permita que os membros postem, inscrevam novos membros na conversa, desabilitem o email de boas-vindas e ocultem o grupo nas experiências do Outlook.
- Especifique os recursos a serem fornecidos na propriedade **resourceProvisioningOptions** que normalmente não fazem parte da criação do [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) padrão. Atualmente há suporte para provisionamento de um grupo como uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) com os recursos do Microsoft Teams.

### <a name="identity-and-access"></a>Identidade e acesso
- Aplica opções de consulta do sistema OData (`$count`, `$filter`, `$search`) ao obter coleções de entidades derivadas do [directoryObject](). Você pode [pesquisar tokens específicos](./query-parameters.md#using-search-on-directory-object-collections) nas propriedades **displayName** e **description** dessas entidades, e usar a conversão OData para aparar os resultados do **directoryObject** para determinados tipos derivados. Veja mais detalhes em [Criar consultas avançadas no Microsoft Graph com $count, $filter, $search e $orderby](https://developer.microsoft.com/pt-BR/graph/blogs/build-advanced-queries-with-count-filter-search-and-orderby/).
- Como parte da [API de proteção de identidade](/graph/api/resources/identityprotection-root?view=graph-rest-beta&preserve-view=true), use a propriedade **riskEventType** para [obter o tipo de risco detectado](/graph/api/riskdetection-get?view=graph-rest-beta&preserve-view=true) ou [obter o tipo de risco no histórico de um usuário](/graph/api/riskyuser-list-history?view=graph-rest-beta&preserve-view=true). Não use a propriedade **risktype** como foi preterida.
- Especifique os tipos de aplicativo cliente na propriedade **clientAppTypes** do [conjunto de condições](/graph/api/resources/conditionalaccessconditionset?view=graph-rest-beta&preserve-view=true) de uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true).
- Use a permissão delegada de `EntitlementManagement.Read.All` para permitir ao aplicativo solicitar acesso para ler pacotes de acesso e recursos de gerenciamento de direitos relacionados em nome do usuário conectado.
- Use as permissões delegadas ou de aplicativo do `Application.Read.All` e do `Application.ReadWrite.All` para [listar aplicativos](/graph/api/application-list?view=graph-rest-beta&preserve-view=true) em uma organização.
- Controle as configurações de autorização no Azure AD usando o tipo de recurso [authorizationPolicy](/graph/api/resources/authorizationpolicy?view=graph-rest-beta&preserve-view=true).

### <a name="teamwork"></a>Trabalho em equipe
- Os aplicativos do Teams que oferecem [suporte a SSO (logon único)](/microsoftteams/platform/tabs/how-to/authentication/auth-aad-sso) podem especificar o `WebApplicationInfo.id` a partir do manifesto do aplicativo Teams, na propriedade **azureADAppId** do [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta&preserve-view=true).
- Use as [permissões mais refinadas](./permissions-reference.md#teams-resource-specific-consent-permissions) para acessar os recursos da [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) e do [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true).


## <a name="april-2020-new-and-generally-available"></a>Abril de 2020: novo e geralmente disponível.

### <a name="calendar"></a>Calendário
- [Compartilhar ou delegar calendários](outlook-share-or-delegate-calendar.md) de forma programática, com uma maior paridade com a experiência do usuário do Outlook. Além de controlar as permissões do usuário atual e o status de compartilhamento de um calendário:
  - Para cada [calendário](/graph/api/resources/calendar?view=graph-rest-1.0&preserve-view=true), você pode gerenciar as [permissões](/graph/api/resources/calendarpermission?view=graph-rest-1.0&preserve-view=true) de cada usuário com o qual o calendário é compartilhado. 
  - Para cada [caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true), você pode especificar se um representante, proprietário de caixa de correio ou ambos receberão mensagens da reunião e respostas da reunião. 
- [Criar ou atualizar um evento como uma reunião online](outlook-calendar-online-meetings.md):
  - Para cada **calendário**, especifique os provedores de reuniões online permitidos e padrão.
  - Crie ou atualize um [evento](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true) que esteja disponível online e forneça detalhes para que os participantes possam ingressar na reunião online. 
  - Em particular, use as novas propriedades **onlineMeetingProvider** e **onlineMeeting** do **evento** para definir ou identificar o Microsoft Teams como um provedor de reuniões online, uma solução alternativa para um [problema conhecido](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) com a propriedade **onlineMeetingUrl**.
- Adicione [anexos de arquivo de até 150 MB](outlook-large-attachments.md) a um [evento](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Arquivos
- [Check-out](/graph/api/driveitem-checkout?view=graph-rest-1.0&preserve-view=true) ou [check-in](/graph/api/driveitem-checkin?view=graph-rest-1.0&preserve-view=true) de um arquivo para o OneDrive para gerenciar a atualização do arquivo e disponibilizar atualizações para outras pessoas quando as atualizações estiverem prontas.
- Aplique senha opcional e data/hora de vencimento como parâmetros do [convite](/graph/api/driveitem-invite?view=graph-rest-1.0&preserve-view=true) e das ações de [criar link de compartilhamento](/graph/api/driveitem-createlink?view=graph-rest-1.0&preserve-view=true) para compartilhar um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).
- Obtenha ou defina a senha e a data/hora de vencimento de uma [permissão](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true) e rastreie o [identitySet](/graph/api/resources/identityset?view=graph-rest-1.0&preserve-view=true) de usuários que receberam permissão para compartilhar um **driveItem**.
- Obtenha a [permissão](/graph/api/resources/permission?view=graph-rest-1.0&preserve-view=true) de um [item de drive compartilhado](/graph/api/resources/shareddriveitem?view=graph-rest-1.0&preserve-view=true) usando a propriedade de navegação de **permissão**.
- Limite os usuários com um [link de compartilhamento](/graph/api/resources/sharinglink?view=graph-rest-1.0&preserve-view=true) para somente visualização e não poder baixar o conteúdo de um **driveItem** compartilhado no OneDrive for Business ou no SharePoint.

### <a name="identity-and-access"></a>Identidade e acesso
- Para gerenciar funções e atribuir acesso a recursos nos provedores de controle de acesso baseado em função (RBAC), como o Microsoft Intune, use [unifiedRoleAssignmentMultiple](/graph/api/resources/unifiedroleassignmentmultiple?view=graph-rest-1.0&preserve-view=true). O recurso **unifiedRoleAssignmentMultiple** permite definir uma única função em uma matriz de escopos e atribuir a função a várias entidades (como usuários).
- Acessar tipos específicos de [políticas de uma organização](/graph/api/resources/policy-overview?view=graph-rest-1.0&preserve-view=true) usando o `/policies`segmento URL e especificando o tipo de política. Por exemplo, uma organização pode forçar uma política a entrar automaticamente no usuário de uma sessão da Web após um período de inatividade, confira as operações CRUD para instâncias de [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-1.0&preserve-view=true). Essa é um [alteração significativa](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-1.0/) para que seja mais fácil descobrir todas as políticas, agrupando todas as políticas digitadas sob o `/policies`segmento. Acesse outras políticas digitadas de uma abordagem semelhante: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-1.0&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-1.0&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-1.0&preserve-view=true)e [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-1.0&preserve-view=true). 

### <a name="mail"></a>Correio
Adicione [anexos de arquivo de até 150 MB](outlook-large-attachments.md) a uma [mensagem](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true).

### <a name="sites-and-lists"></a>Sites e listas
- [Faça uma lista de sites](/graph/api/sites-list-followed?view=graph-rest-1.0&preserve-view=true) que o usuário conectado seguiu.
- Identifique a região geográfica de um [conjunto de sites](/graph/api/resources/sitecollection?view=graph-rest-1.0&preserve-view=true) usando a propriedade **dataLocationCode**.
- Identifique o locatário de um arquivo, pasta ou outro item no SharePoint, acessando a propriedade **tenantId** que faça parte do **sharepointIds** de um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true).

## <a name="april-2020-new-in-preview-only"></a>Abril de 2020: novo somente para visualização

### <a name="devices-and-apps--cloud-printing"></a>Dispositivos e aplicativos | Impressão na nuvem

Designar usuários e grupos permitidos para usar compartilhamentos de impressoras [específicos](/graph/api/resources/printershare?view=graph-rest-beta&preserve-view=true) em impressão universal, a infraestrutura de impressão baseada na nuvem do Microsoft 365. Para experimentar recursos de gerenciamento de impressão eficientes e centralizados, assim como oferecer uma experiência de impressão simples, porém rica e segura para os usuários de impressão, consulte o [Anúncio de impressão universal](https://techcommunity.microsoft.com/t5/windows-it-pro-blog/announcing-universal-print-a-cloud-based-print-solution/ba-p/1204775) e participe do programa de visualização.

### <a name="devices-and-apps--corporate-management"></a>Dispositivos e aplicativos | Gerenciamento corporativo
Atualizações de [abril](changelog.md#april-2020) do Intune.

### <a name="groups"></a>Grupos
Identifique o aplicativo que criou um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) pela sua ID do aplicativo.

### <a name="identity-and-access"></a>Identidade e acesso
- [Controlar alterações](/graph/api/administrativeunit-delta?view=graph-rest-beta&preserve-view=true) para [unidades administrativas](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true).
- [Controlar alterações](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta&preserve-view=true) para [oAuth2PermissionGrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta&preserve-view=true).
- [Gerenciar](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta&preserve-view=true) os [métodos de autenticação](/graph/api/resources/authenticationmethod?view=graph-rest-beta&preserve-view=true) de um usuário que incluem a [senha](/graph/api/resources/passwordauthenticationmethod?view=graph-rest-beta&preserve-view=true) ou [telefone](/graph/api/resources/phoneauthenticationmethod?view=graph-rest-beta&preserve-view=true). Por exemplo, [redefinir uma senha de usuário](/graph/api/passwordauthenticationmethod-resetpassword?view=graph-rest-beta&preserve-view=true), [obter o status da redefinição](/graph/api/authenticationoperation-get?view=graph-rest-beta&preserve-view=true) ou [adicionar um número de telefone](/graph/api/authentication-post-phonemethods?view=graph-rest-beta&preserve-view=true) para um usuário para autenticação de SMS ou chamada de voz, se a política estiver habilitada para o usuário.

### <a name="reports--identity-and-access-reports"></a>Relatórios | Relatórios de identidade e acesso
[Listar](/graph/api/relyingpartydetailedsummary-list?view=graph-rest-beta&preserve-view=true) [participantes confiáveis](/windows-server/identity/ad-fs/technical-reference/understanding-key-ad-fs-concepts) configurados nos Serviços de Federação do Active Directory.

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
Exibir dados de **Reunião Criada** e de **Reunião Interagida** nos relatórios CSV para [contagens de atividades de email](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta&preserve-view=true), [contagens de atividades de email do usuário](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta&preserve-view=true) e [detalhes de atividades de email do usuário](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta&preserve-view=true).


## <a name="march-2020-new-and-generally-available"></a>Março de 2020: Novo e disponível para o público geral

### <a name="cloud-communications"></a>Comunicações na nuvem
- Obtenha o roteamento de chamadas e o contexto de entrada de um [chamada](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true).
- Um aplicativo pode [Atualizar o status da gravação](/graph/api/call-updaterecordingstatus?view=graph-rest-1.0&preserve-view=true) de uma chamada.
- Gravar as informações especificamente para um [participante](/graph/api/resources/participant?view=graph-rest-1.0&preserve-view=true), incluindo o iniciador e o status da gravação.
- Identifique de forma exclusiva os participantes de uma conferência ou [chamada](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) de participante a participante usando a propriedade **callChainId**.
- Identifique como parte do [participantInfo](/graph/api/resources/participantinfo?view=graph-rest-1.0&preserve-view=true) o código do país e o tipo de ponto de extremidade (como o Skype for Business ou o Skype for Business VOIP) do participante.
- Os parceiros de dispositivos de VTC (teleconferência por vídeo de terceiros) podem registrar e fornecer dados de qualidade de mídia para dispositivos de teleconferência por vídeo através de um bot de CVI (Interoperabilidade de vídeo em nuvem) e usando a função [logTeleconferenceDeviceQuality](/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0&preserve-view=true). A qualidade da mídia inclui dados do tipo aberto para [áudio](/graph/api/resources/teleconferencedeviceaudioquality?view=graph-rest-1.0&preserve-view=true), [vídeo](/graph/api/resources/teleconferencedevicevideoquality?view=graph-rest-1.0&preserve-view=true) e [compartilhamento de tela](/graph/api/resources/teleconferencedevicescreensharingquality?view=graph-rest-1.0&preserve-view=true).

### <a name="files"></a>Arquivos
- [Os itens remotos](/graph/api/resources/remoteitem?view=graph-rest-1.0&preserve-view=true) compartilhados com um usuário, adicionados ao OneDrive do usuário, ou retornados como resultado de pesquisa podem conter metadados para uma imagem ou um vídeo.
- [Siga](/graph/api/driveitem-follow?view=graph-rest-1.0&preserve-view=true) um [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0&preserve-view=true) para obter um acesso conveniente ou para facilitar ações como mover, copiar e salvar como. Use [deixar de serguir](/graph/api/driveitem-unfollow?view=graph-rest-1.0&preserve-view=true) para deixar de seguir o item da unidade.
- [Conceda](/graph/api/permission-grant?view=graph-rest-1.0&preserve-view=true) permissões aos usuários para acessarem um link de compartilhamento para compartilhar o item da unidade correspondente.

### <a name="identity-and-access"></a>Identidade e acesso
- [Controle de alterações](/graph/api/orgcontact-delta?view=graph-rest-1.0&preserve-view=true) para [contatos organizacionais](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true).
- Use a propriedade **riskEventTypes_v2** para obter os tipos de eventos de risco associados a [entrada](/graph/api/resources/signin?view=graph-rest-1.0&preserve-view=true).
- Use a permissão delegada `User.ManageIdentities.All` para permitir que um aplicativo leia, atualize ou exclua identidades associadas à conta de um usuário, às quais o usuário conectado tem acesso. Use essa permissão no nível do aplicativo sem um usuário conectado. Isso permite ao aplicativo [gerenciar](/graph/api/user-update?view=graph-rest-1.0&preserve-view=true) com quais identidades um usuário pode se inscrever.

### <a name="reports"></a>Relatórios
O administrador de serviços do Teams e o administrador de comunicações do Teams devem ser usados como funções de usuário aceitas para permitir que os aplicativos leiam os relatórios de uso do serviço do Microsoft 365 em nome de um usuário, como [formas de autorização delegada pelo usuário](reportroot-authorization.md). 

### <a name="sites"></a>Sites
- Permitir que os usuários [sigam](/graph/api/site-follow?view=graph-rest-1.0&preserve-view=true) ou [parem de seguir](/graph/api/site-unfollow?view=graph-rest-1.0&preserve-view=true) os sites do SharePoint.
- [Inscreva-se para alterar as notificações](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) para uma lista  [do SharePoint](/graph/api/resources/list?view=graph-rest-1.0&preserve-view=true).

## <a name="march-2020-new-in-preview-only"></a>Março de 2020: novo somente para visualização

### <a name="calendar"></a>Calendário
- Use a propriedade **calendarGroupId** para obter o [grupo de calendário](/graph/api/resources/calendargroup?view=graph-rest-beta&preserve-view=true) em que um [calendário](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true) foi criado.
- Use a propriedade **isDraft** para identificar um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) como uma reunião que o usuário atualizou no Outlook, mas não enviou para atualizar os participantes.

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use [createOrGet](/graph/api/onlinemeeting-createorget?view=graph-rest-beta&preserve-view=true) para obter uma instância de [reunião online](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true) por um ID externo personalizado e criar uma quando não houver nenhuma.
- Você tem a opção de usar a propriedade **externalId** para identificar uma reunião online com a ID externa personalizada.
- Use o `Accept-Language` cabeçalho opcional da solicitação HTTP para [criar](/graph/api/application-post-onlinemeetings?view=graph-rest-beta&preserve-view=true) ou [obter](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true) uma instância da reunião online, para que a operação bem-sucedida exiba o conteúdo da propriedade **joinInformation** no idioma especificado e variante de localidade.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [março](changelog.md#march-2020) do Intune

### <a name="identity-and-access"></a>Identidade e acesso
- Use a permissão `Auditlogs.Read.All` para listar a [atividade de entrada](/graph/api/resources/signinactivity?view=graph-rest-beta&preserve-view=true) de um [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true).
- Use a `PrivilegedAccess.Read.AzureResources` permissão no nível do aplicativo para [PIM (gerenciamento de identidades privilegiadas) dos recursos do Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta&preserve-view=true), para configurar o fluxo de trabalho de acesso just-in-time para funções de infraestrutura do Azure em um grupo de gerenciamento, assinatura, grupo de recursos ou nível de recurso.
- Use a entidade [identitySecurityDefaultsEnforcementPolicy](/graph/api/resources/identitysecuritydefaultsenforcementpolicy?view=graph-rest-beta&preserve-view=true) para [obter](/graph/api/identitysecuritydefaultsenforcementpolicy-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/identitysecuritydefaultsenforcementpolicy-update?view=graph-rest-beta&preserve-view=true) as configurações de segurança padrão pré-definidas que protegem as organizações contra ataques comuns.
- Use um segmento `identity` ao chamar APIs de acesso condicional. Por exemplo, para [obter](/graph/api/conditionalaccesspolicy-get?view=graph-rest-beta&preserve-view=true) ou uma [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true): `GET https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}`.
- Use a propriedade **authenticationRequirement** para obter o nível mais alto de autenticação necessária por meio de todas as etapas de entrada para que a [entrada](/graph/api/resources/signin?view=graph-rest-beta&preserve-view=true) seja bem-sucedida.
- Use a paginação quando [listar eventos de provisionamento](/graph/api/provisioningobjectsummary-list?view=graph-rest-beta&preserve-view=true) ocorridos no locatário.

### <a name="search"></a>Pesquisa
- Para adicionar dados em um arquivo para pesquisar resultados, indexe os dados como um [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true). O tipo **externalFile** foi substituído.
- Agora é possível [atualizar](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) um [item no índice](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true), atualizando especificamente a representação de texto simples do item (representado pela propriedade **conteúdo**), ou o conjunto de propriedades do item (representado pela propriedade **propriedades**). A atualização de qualquer propriedade no conjunto de propriedades substitui todo conjunto de propriedades, por isso certifique-se de incluir explicitamente todas as propriedades do item na atualização.
- Verifique o `HTTP 429` e o cabeçalho de resposta `Retry-After` depois de chamar a operação para [criar](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true), [atualizar](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) ou [excluir](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) de **externalItem**. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da [limitação](throttling.md#best-practices-to-handle-throttling).

### <a name="teamwork"></a>Trabalho em equipe
Use a `ChannelMessage.Read.All` permissão no nível do aplicativo para ler [instâncias de](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true)chatMessage em canais sem um usuário conectado.

### <a name="universal-print"></a>Impressão universal
Estréia da [API de impressão universal](universal-print-concept-overview.md), que permite que os usuários imprimam na Web ou de um aplicativo. A API permite que os administradores de TI gerenciem o acesso de usuários e grupos a impressoras na nuvem do Microsoft 365, compartilhamento remoto da impressora para manter a disponibilidade, monitorar o status da impressora e emitir relatórios sobre trabalho de impressão arquivado e uso. 

Observe que a partir de março de 2020, o serviço de _impressão universal_ está na visualização particular. Confira [anunciando a impressão universal: uma solução de impressão baseada na nuvem](https://aka.ms/announcinguniversalprint) para obter informações sobre a participação.


## <a name="february-2020-new-and-generally-available"></a>Fevereiro de 2020: novo e disponível para o público geral

### <a name="calendar"></a>Calendário
Vamos examinar um exemplo de [criação de um evento em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md), além das ações e propriedades disponíveis para o representante, os convidados e o proprietário do calendário durante esse processo.

### <a name="identity-and-access"></a>Identidade e acesso
- Para aumentar a segurança ao assinar as [notificações de alteração dos dados do usuário](webhooks.md), [impor o Protocolo TLS 1.2](/configmgr/core/plan-design/security/enable-tls-1-2) ou mais recente em clientes e servidores de sites usados no processo de notificação. O novo requisito será lançado em estágios a partir de 15 de fevereiro de 2020. A partir de 15 de maio de 2020, todos os pontos de extremidade de notificação devem atendem ao novo requisito de TLS. [Descubra os estágios do lançamento](https://developer.microsoft.com/graph/blogs/microsoft-graph-subscriptions-deprecating-tls-1-0-and-1-1/) e, se necessário, use a nova propriedade **latestSupportedTlsVersion** como uma solução alternativa temporária para evitar falhas de assinatura antes de concluir a atualização de TLS.
- Use os respectivos tipos de [solicitação de avaliação de ameaças](/graph/api/resources/threatAssessmentRequest?view=graph-rest-1.0&preserve-view=true) para controlar as ameaças de [email](/graph/api/resources/mailassessmentrequest?view=graph-rest-1.0&preserve-view=true), um [arquivo de mensagem de email](/graph/api/resources/emailfileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (arquivo .EML), [arquivo de anexo de email](/graph/api/resources/fileassessmentrequest?view=graph-rest-1.0&preserve-view=true) (texto, Word ou arquivo binário) ou [URL](/graph/api/resources/urlassessmentrequest?view=graph-rest-1.0&preserve-view=true).

### <a name="users"></a>Usuários
[Reprocessar](/graph/api/user-reprocesslicenseassignment?view=graph-rest-1.0&preserve-view=true) todas as atribuições de licença baseadas em grupo para um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).


## <a name="february-2020-new-in-preview-only"></a>Fevereiro de 2020: nova somente para visualização

### <a name="calendar"></a>Calendário
Confira [tarefas com suporte por APIs de visualização que gerenciam o compartilhamento de calendários e a delegação](outlook-share-or-delegate-calendar.md).

### <a name="cloud-communications"></a>Comunicações na nuvem

- Use o novo recurso [registros de chamadas](/graph/api/resources/callrecord?view=graph-rest-beta&preserve-view=true) para obter metadados de chamadas e reuniões online do Microsoft Teams e do Skype for Business para uma organização.
- Para um participante de uma reunião, use a propriedade **Iniciador** para obter as informações de identidade do iniciador de uma [gravação](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true), se houver uma.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [fevereiro](changelog.md#february-2020) do Intune.

### <a name="groups"></a>Grupos
Use o método [assignLicense](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) para atribuir licenças de produtos, como o Microsoft 365 ou o Enterprise Mobility + Security, a um grupo. Como o Azure AD garante que as licenças sejam designadas para os membros do grupo, os membros que ingressarem ou saírem de um grupo não precisarão mais de gerenciamento de licenças no nível individual.

### <a name="identity-and-access"></a>Identidade e acesso
- Defina as configurações de solicitação, aprovação e revisar ao criar uma [política de atribuição de pacote](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta&preserve-view=true).
- Acessar tipos específicos de [políticas de uma organização](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) usando o `/policies`segmento URL e especificando o tipo de política. Por exemplo, uma organização pode forçar uma política a entrar automaticamente no usuário de uma sessão da Web após um período de inatividade, confira as operações CRUD para instâncias de [activityBasedTimeoutPolicy](/graph/api/resources/activitybasedtimeoutpolicy?view=graph-rest-beta&preserve-view=true). Essa é um [alteração significativa](https://developer.microsoft.com/identity/blogs/breaking-changes-policy-api-microsoft-graph-beta/) para que seja mais fácil descobrir todas as políticas, agrupando todas as políticas digitadas sob o `/policies`segmento. Acesse outras políticas digitadas de uma abordagem semelhante: [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta&preserve-view=true), [homeRealmDiscoveryPolicy](/graph/api/resources/homerealmdiscoverypolicy?view=graph-rest-beta&preserve-view=true), [tokenLifetimePolicy](/graph/api/resources/tokenlifetimepolicy?view=graph-rest-beta&preserve-view=true)e [tokenIssuancePolicy](/graph/api/resources/tokenissuancetimepolicy?view=graph-rest-beta&preserve-view=true). 
- Use a permissão de nível de aplicativo e `Policy.ReadWrite.ApplicationConfiguration` delegada para operações de leitura e gravação na configuração do aplicativo [políticas](/graph/api/resources/policy-overview?view=graph-rest-beta&preserve-view=true) mencionadas no item anterior.

### <a name="teamwork"></a>Trabalho em equipe
- Use [alterar as notificações](/graph/api/resources/webhooks?view=graph-rest-beta&preserve-view=true) em todas as mensagens do canal ou em todas as mensagens de chat em uma organização.
- [Recuse](/graph/api/swapshiftschangerequest-decline?view=graph-rest-beta&preserve-view=true) uma [solicitação de troca de turnos](/graph/api/resources/swapshiftschangerequest?view=graph-rest-beta&preserve-view=true) com outro usuário em uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true).

## <a name="january-2020-new-and-generally-available"></a>Janeiro de 2020: Novo e disponível para o público geral

### <a name="security"></a>Segurança
Como parte do gerenciamento de alerta de cliente, use o método de [alerta de atualização](/graph/api/alert-update?view=graph-rest-1.0&preserve-view=true) e atualize o campo **comentários** como `Closed in IPC` ou `Closed in MCAS`.

### <a name="teamwork"></a>Trabalho em equipe
Use a propriedade de navegação **primaryChannel** de uma [equipe](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) para acessar o canal padrão, **Geral**.

### <a name="users"></a>Usuários
Use a propriedade **identities** para acessar uma ou mais identidades que um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true) pode usar para entrar em uma conta de usuário do Azure AD. As identidades podem ser fornecidas pela Microsoft, por organizações ou por provedores de identidade social, como Facebook, Google ou Microsoft. Essa propriedade permite que o usuário entre na conta de usuário com uma dessas identidades.

## <a name="january-2020-new-in-preview"></a>Janeiro de 2020: novidades na versão prévia

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [janeiro](changelog.md#january-2020) do Intune.


## <a name="december-2019-new-and-generally-available"></a>Dezembro de 2019: Novo e disponível para o público geral

### <a name="cloud-communications"></a>Comunicações na nuvem
A API de comunicações na nuvem tem o GA'd e as APIs para [chamada](/graph/api/resources/call?view=graph-rest-1.0&preserve-view=true) e [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-1.0&preserve-view=true) estão [disponíveis na v1.0](/graph/api/resources/communications-api-overview?view=graph-rest-1.0&preserve-view=true).

### <a name="education"></a>Educação
Use a propriedade **classSettings** para gerenciar configurações específicas de classe, como habilitar o envio de resumos de atribuições semanais. Esta propriedade está disponível no recurso [equipe](/graph/api/resources/team?view=graph-rest-1.0&preserve-view=true) quando a equipe representa uma [classe educacional](/graph/api/resources/educationclass?view=graph-rest-1.0&preserve-view=true).

### <a name="identity-and-access"></a>Identidade e acesso 
[Tentar obter objetos de contêiner com permissões limitadas retorna dados parciais](permissions-reference.md#limited-information-returned-for-inaccessible-member-objects). Um exemplo é uma instância de [grupo](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) associada a um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true), outro **grupo** e um [dispositivo](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true). Um aplicativo que tem somente as permissões User.Read.All e Group.Read.All e tentar acessar essa instância de **grupo** obteria os objetos de **usuário** e **grupo**, mas dados limitados para o objeto de **dispositivo** (apenas o tipo de dados e a ID do objeto e não os valores da propriedade).

### <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e local de trabalho
A API do insights tem GA'd. Use a API em aplicativos de produção para identificar os documentos mais relevantes, que são:

- [Tendências de](/graph/api/insights-list-trending?view=graph-rest-1.0&preserve-view=true) um usuário
- [Usado por](/graph/api/insights-list-used?view=graph-rest-1.0&preserve-view=true) um usuário
- [Compartilhados com ou por](/graph/api/insights-list-shared?view=graph-rest-1.0&preserve-view=true) um usuário

### <a name="reports"></a>Relatórios
Para obter relatórios de uso do Microsoft 365 usando permissões delegadas por um usuário, os administradores devem ter atribuído ao usuário uma função de administrador limitado do Azure AD. Podendo ser uma das seguintes funções: administrador da empresa, administrador do Exchange, administrador do SharePoint, administrador do Lync, leitor global ou leitor de relatórios. Para mais detalhes, confira [Autorização para APIs lerem os relatórios de uso do Microsoft 365](reportroot-authorization.md).

### <a name="toolkit"></a>Kit de ferramentas
O Microsoft Graph Toolkit v1.1 foi lançado. Para obter uma lista de aperfeiçoamentos e correções de bugs, confira a [seção de dezembro de 2019](changelog.md#december-2019) do log de alterações.

## <a name="december-2019-new-in-preview"></a>Dezembro de 2019: novidades na versão prévia

### <a name="cloud-communications"></a>Comunicações na nuvem
- Use o novo recurso [presença](/graph/api/resources/presence?view=graph-rest-beta&preserve-view=true) para obter informações sobre a disponibilidade e a atividade atual de um ou mais usuários.
- [Exclua](/graph/api/onlinemeeting-delete?view=graph-rest-beta&preserve-view=true) uma instância de um [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true).
- Confira a [seção de dezembro de 2019](changelog.md#december-2019) do log de alterações para a renomeação e a remoção de alguns membros dos recursos da [chamada](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) e do [onlineMeeting](/graph/api/resources/onlinemeeting?view=graph-rest-beta&preserve-view=true), para estar na paridade com a versão v1 desses recursos.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [Dezembro](changelog.md#december-2019) do Intune

### <a name="identity-and-access"></a>Identidade e acesso 
- Correção de comportamento nos relacionamentos **appRoleAssignments** e **appRoleAssignedTo** em [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Use [accessPackageResourceRequest](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta&preserve-view=true) em [gerenciamento de direitos do Azure AD](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) para solicitar a adição de um recurso a um [catálogo](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta&preserve-view=true), para que as funções desse recurso possam ser usadas em um [pacote de acesso](/graph/api/resources/accesspackage?view=graph-rest-beta&preserve-view=true).
- Use a [API de avaliação de ameaças](/graph/api/resources/threatassessment-api-overview?view=graph-rest-beta&preserve-view=true) para capacitar os administradores a relatar emails suspeitos, URLs de phishing, anexos de email ou outros arquivos. O veredicto de varredura de thread pode então informá-los a ajustar a política organizacional adequadamente.

### <a name="teamwork"></a>Trabalho em equipe
- [Configure as notificações que incluem dados de recursos](webhooks-with-resource-data.md) para recursos do [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) nos canais e bate-papos do Microsoft Teams.
- [Assine as notificações](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) de [mensagens de canal ou de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) novas ou modificadas.
- Use o recurso [shiftPreferences](/graph/api/resources/shiftpreferences?view=graph-rest-beta&preserve-view=true) para permitir que a especificação da disponibilidade de um usuário seja atribuída a turnos em um [cronograma](/graph/api/resources/schedule?view=graph-rest-beta&preserve-view=true). Obtenha ou defina isso como parte das [configurações](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true) do usuário.


## <a name="november-2019-new-and-generally-available"></a>Novembro de 2019: novo e disponível para o público geral

### <a name="groups"></a>Grupos
- Use permissões delegadas ou de aplicativo, GroupMember.Read.All e GroupMember.ReadWrite.All, para listar grupos, leia as propriedades básicas do grupo, leia (e atualize a permissão de leitura/gravação) a associação dos grupos aos quais o aplicativo tem acesso.
- Use a permissão do aplicativo, Group.Create, para criar grupos sem um usuário conectado.
- Para um [grupo](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true) especificado, [verifique a associação](/graph/api/group-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) em outros grupos ou funções de diretório.

### <a name="identity-and-access"></a>Identidade e acesso
- Registre [aplicativos](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true) que se autenticam com o Azure Active Directory (Azure AD). Use as [permissões](./permissions-reference.md#application-resource-permissions) delegadas, Application.Read.All e Application.ReadWrite.All ou as permissões de aplicativos, Application.Read.All, conforme apropriado.
- Para um [dispositivo](/graph/api/resources/device?view=graph-rest-1.0&preserve-view=true) especificado, [verifique a associação](/graph/api/device-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) em outros grupos ou funções de diretório.

### <a name="mail"></a>Email
- Use a propriedade **conversationIndex** para obter a posição de uma mensagem em uma conversa de email do Outlook.
- Use a permissão delegada, Mail.ReadBasic e a permissão de aplicativo, Mail.ReadBasic.All, para obter os recursos de [mensagem](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) ou de [pasta de email](/graph/api/resources/mailfolder?view=graph-rest-1.0&preserve-view=true), acompanhar suas alterações e gerenciar [assinaturas](/graph/api/resources/subscription?view=graph-rest-1.0&preserve-view=true) para notificações de alteração nas mensagens.

### <a name="users"></a>Usuários
- [Verifique se há associações de grupo](/graph/api/user-checkmemberobjects?view=graph-rest-1.0&preserve-view=true) de um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true) específico.
- Use a propriedade **creationType** para descobrir como uma conta de usuário foi criada, por exemplo, se a conta foi criada como uma conta corporativa ou de estudante ou como uma conta externa, etc.

## <a name="november-2019-new-in-preview"></a>Novembro de 2019: Novidades na versão prévia

### <a name="calendar"></a>Calendário
- [Use o Outlook para organizar e participar de reuniões online](outlook-calendar-online-meetings.md).
- [Defina as propriedades](/graph/api/place-update?view=graph-rest-beta&preserve-view=true) para os tipos de local avançado de [sala](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) e [lista de sala](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true).

### <a name="cloud-communication"></a>Comunicação na nuvem
O tipo de recurso de [chamada](/graph/api/resources/call?view=graph-rest-beta&preserve-view=true) dá suporte aos seguintes recursos adicionais:

- O [contexto de uma chamada de entrada](/graph/api/resources/incomingcontext?view=graph-rest-beta&preserve-view=true)
- O tipo de ponto de extremidade de um participante, como correio de voz ou Skype for Business
- A capacidade de [atualizar](/graph/api/call-updaterecordingstatus?view=graph-rest-beta&preserve-view=true) as [informações de registro](/graph/api/resources/recordinginfo?view=graph-rest-beta&preserve-view=true) de um [participante](/graph/api/resources/participant?view=graph-rest-beta&preserve-view=true)

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [novembro](changelog.md#november-2019) do Intune

### <a name="education"></a>Educação
Os administradores podem habilitar as configurações de toda a classe por meio da propriedade **classSettings** da [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) associada à [classe](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true). Atualmente, há uma configuração para notificar os guardiões sobre tarefas semanais.

### <a name="identity-and-access"></a>Identidade e acesso
- Use a permissão do aplicativo, Policy.Read.All, para ler todas as políticas de acesso condicional da sua localização e locais nomeados, sem um usuário conectado.
- Permita que a [política de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) esteja em um estado somente de relatório, `enabledForReportingButNotEnforced`.
- Use a permissão delegada, ThreatAssessment.ReadWrite.All, ou a permissão de aplicativo, ThreatAssessment.Read.All, leia (ou crie uma permissão de leitura/gravação) solicitações para avaliar ameaças em uma organização.

### <a name="mail"></a>Email
Use a permissão delegada, Mail.ReadBasic e a permissão de aplicativo, Mail.ReadBasic.All, para gerenciar as [assinaturas](/graph/api/resources/subscription?view=graph-rest-beta&preserve-view=true) para notificações de alteração no recurso de [mensagem](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true).

### <a name="notifications"></a>Notificações
Use as novas notificações simples [SDK Web](https://aka.ms/GNSDK) em vez do [SDK do Project Rome](https://github.com/Microsoft/project-rome), para aproveitar um modelo de autenticação aperfeiçoado e suporte a aplicativos da Web usando o push da Web. 

### <a name="people-and-workplace-intelligence"></a>Inteligência de pessoas e local de trabalho
Estreia do recurso do [perfil](/graph/api/resources/profile?view=graph-rest-beta&preserve-view=true) que é uma representação avançada da próxima geração de entidades de pessoas nos serviços da Microsoft. Esse recurso se relaciona aos atributos comuns e práticos de pessoas, incluindo informações sobre datas significativas, como [aniversários](/graph/api/resources/personanniversary?view=graph-rest-beta&preserve-view=true), [escolaridade](/graph/api/resources/educationalactivity?view=graph-rest-beta&preserve-view=true), [cargos](/graph/api/resources/workposition?view=graph-rest-beta&preserve-view=true), [interesses](/graph/api/resources/personinterest?view=graph-rest-beta&preserve-view=true), [idioma](/graph/api/resources/languageproficiency?view=graph-rest-beta&preserve-view=true) e [habilidades](/graph/api/resources/skillproficiency?view=graph-rest-beta&preserve-view=true) e competências, [participação em projetos](/graph/api/resources/projectparticipation?view=graph-rest-beta&preserve-view=true), [associação em sites](/graph/api/resources/personwebsite?view=graph-rest-beta&preserve-view=true) e outras informações de contato e [conta](/graph/api/resources/useraccountinformation?view=graph-rest-beta&preserve-view=true).

### <a name="search"></a>Pesquisar
Estreia da [API de Pesquisa da Microsoft](search-concept-overview.md) que permite aos usuários do aplicativo obter os resultados de pesquisa mais atualizados, personalizados e relevantes com a plataforma Microsoft Graph. Use o recurso de [consulta](/graph/api/search-query?view=graph-rest-beta&preserve-view=true)por padrão, pesquisas mensagens e eventos do Outlook e arquivos do OneDrive e do SharePoint na nuvem da Microsoft. Use os conectores [disponíveis](/microsoftsearch/connectors-overview) na [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery), para incluir dados de pesquisa fora do Microsoft Cloud. Como alternativa, [construa seus próprios conectores](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), indexe arquivos e itens personalizados externos e consulte fontes de dados externas específicas.

### <a name="teamwork"></a>Trabalho em equipe
Obtenha os recursos de [arquivo](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) associados a uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) e [canal](/graph/api/resources/channel?view=graph-rest-beta&preserve-view=true) usando a seguinte sintaxe de solicitação de HTTP:

```http
GET /teams/{teamId}/channels/{channelId}/filesFolder
```

### <a name="users"></a>Usuários
Use a propriedade **creationType** para descobrir como uma conta de usuário foi criada, por exemplo, se a conta foi criada como uma conta corporativa ou de estudante ou como uma conta externa, etc.


## <a name="october-2019-new-and-generally-available"></a>Outubro de 2019: Novo e geralmente disponível

### <a name="identity-and-access"></a>Identidade e acesso
- Use [contatos da organização](/graph/api/resources/orgcontact?view=graph-rest-1.0&preserve-view=true) em aplicativos de produção. Os contatos da organização são gerenciados por administradores da organização, sincronizados de um Active Directory local ou do Exchange Online.
- Configure a [autenticação baseada em certificado](/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started) em uma [organização](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true).
- Adicionar e remover [credenciais de senha](/graph/api/resources/passwordcredential?view=graph-rest-1.0&preserve-view=true) para [aplicativos](/graph/api/resources/application?view=graph-rest-1.0&preserve-view=true).

### <a name="mail"></a>Email
Use o novo parâmetro de **mensagem** para atualizar quaisquer propriedades de [mensagem](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) graváveis ao [responder](/graph/api/message-reply?view=graph-rest-1.0&preserve-view=true) a uma mensagem, por exemplo, [adicionar um destinatário à resposta](/graph/api/message-reply#example?view=graph-rest-1.0&preserve-view=true).

### <a name="microsoft-graph-data-connect"></a>Conexão de dados do Microsoft Graph
Os desenvolvedores e os cientistas de dados agora podem usar [ferramentas para traduzir dados do Office 365 para o formato Modelo de Dados Comum](https://github.com/OfficeDev/MS-Graph-Data-Connect/blob/master/Common-Data-Model/README.md), tornando-o esquematicamente consistente com outros conjuntos de dados prontos da Open Data Initiative (ODI). 


### <a name="microsoft-graph-sdks"></a>SDKs do Microsoft Graph
- Use os manipuladores de caos no SDK do JavaScript para verificar se um aplicativo é resistente a falhas de servidor que são difíceis de iniciar.
- Ler sobre [fazer chamadas API usando os SDKs](./sdks/create-requests.md).

### <a name="users"></a>Usuários
- [Obtenha](/graph/api/user-get-mailboxsettings?view=graph-rest-1.0&preserve-view=true) ou [defina](/graph/api/user-update-mailboxsettings?view=graph-rest-1.0&preserve-view=true) as configurações preferenciais de formato de data e hora do usuário [para a caixa de correio do usuário](/graph/api/resources/mailboxsettings?view=graph-rest-1.0&preserve-view=true). 
- Rastreie a data/hora da última alteração de senha de um [usuário](/graph/api/resources/user?view=graph-rest-1.0&preserve-view=true).

## <a name="october-2019-new-in-preview"></a>Outubro de 2019: Novo em visualização

### <a name="calendar"></a>Calendário
- Os organizadores de reuniões podem [permitir que os convidados proponham horários de reunião alternativos ](outlook-calendar-meeting-proposals.md). Ao receber uma resposta de reunião que inclua um horário alternativo proposto, o organizador pode decidir aceitar a proposta e [atualizar](/graph/api/event-update?view=graph-rest-beta&preserve-view=true) o horário da reunião.
- O compartilhamento de calendário programático está mais parecido com a experiência do usuário do Outlook. Além de controlar as permissões do usuário atual e o status de compartilhamento de um calendário:
  - Para cada [calendário](/graph/api/resources/calendar?view=graph-rest-beta&preserve-view=true), você pode gerenciar as [permissões](/graph/api/resources/calendarpermission?view=graph-rest-beta&preserve-view=true) de cada usuário com o qual o calendário é compartilhado. 
  - Para cada [caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true), você pode especificar se um representante, proprietário de caixa de correio ou ambos receberão mensagens da reunião e respostas da reunião. 
- Suporte adicional para reuniões online:
  - Para cada **calendário**, especifique os provedores de reuniões online permitidos e padrão.
  - Crie ou atualize um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) que esteja disponível online e forneça detalhes para que os participantes possam ingressar na reunião online. 
  - Em particular, use as novas propriedades **onlineMeetingProvider** e **onlineMeeting** do **evento** para definir ou identificar o Microsoft Teams como um provedor de reuniões online, uma solução alternativa para um [problema conhecido](known-issues.md#onlinemeetingurl-property-support-for-microsoft-teams) com a propriedade **onlineMeetingUrl**.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [outubro](changelog.md#october-2019) do Intune

### <a name="graph-explorer"></a>Graph Explorer
Experimente a [próxima versão do Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/preview) e confira informações contextuais úteis, como permissões, tokens de acesso e trechos de código do SDK nas novas guias **Permissões**, **Autenticação** e **Trechos de código**. Use o controle deslizante **Visualizar** para alternar entre a [produção](https://developer.microsoft.com/graph/graph-explorer) e a nova versão de visualização do Graph Explorer.

### <a name="groups"></a>Grupos
- Use as propriedades **hideFromAddressLists** e **hideFromOutlookClients** para controlar a visibilidade de um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) em determinadas partes da interface do usuário do Outlook ou em um cliente do Outlook.
- [Atribuir](/graph/api/group-assignlicense?view=graph-rest-beta&preserve-view=true) ou remover licenças de usuários em um [grupo](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Identidade e acesso
- Use as [políticas de acesso condicional](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta&preserve-view=true) para personalizar regras de acesso para uma organização. Essas regras consideram sinais sobre uma identidade de um usuário ou dispositivo, como associação a um usuário ou grupo, localização do IP e comportamentos, como tentativas de acesso a aplicativos específicos e comportamentos arriscados de logon.
- Use o [gerenciamento de direitos](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta&preserve-view=true) para gerenciar o acesso a grupos, aplicativos e sites do SharePoint Online para usuários dentro e fora de uma organização.
- Adicione e remova [credenciais de senha](/graph/api/resources/passwordcredential?view=graph-rest-beta&preserve-view=true) para [aplicativos](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) e [entidades de serviço](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true).
- Gerenciar a [política de estrutura confiável](/graph/api/resources/trustframeworkkeyset?view=graph-rest-beta&preserve-view=true) do Azure AD B2C.
- Defina as políticas de [fluxo de usuário](/graph/api/resources/identityuserflow?view=graph-rest-beta&preserve-view=true) do Azure AD B2C para entrar, inscrever-se, entrar e Inscrever-se combinados, redefinir senha e atualizar perfil.
- Configure [rótulos de proteção de informações](/graph/api/resources/informationprotectionlabel?view=graph-rest-beta&preserve-view=true) para classificar a confidencialidade de um usuário ou locatário.
- Aplicativos existentes usando as APIs para [eventos de risco de identidade](/graph/api/resources/identityriskevent?view=graph-rest-beta&preserve-view=true) devem fazer ar transição para [ detecção de risco](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) no Azure AD Identity Protection. Confira a postagem de blog [ postagem de blog](https://developer.microsoft.com/graph/blogs/deprecatation-of-the-identityriskevents-api/) relacionada para obter mais detalhes e cronograma de descontinuação.


### <a name="mail"></a>Email
[Anexe arquivos grandes de até 150MB](outlook-large-attachments.md) a uma instância de [mensagem](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true), criando uma [sessão de upload](/graph/api/resources/uploadsession?view=graph-rest-beta&preserve-view=true) e carregando iterativamente os intervalos do arquivo até que todos os bytes do arquivo tenham sido carregados. 

### <a name="microsoft-graph-security-api"></a>API de Segurança do Microsoft Graph
- Visualize a integração com a RSA NetWitness, ServiceNow e Splunk, para correlacionar e sincronizar [alertas](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#alerts)e melhorar a proteção contra ameaças e respostas.
- Novos disparadores adicionados ao [Conector de Segurança do Microsoft Graph](/connectors/microsoftgraphsecurity/) e [guias estratégicos](/azure/security-center/security-center-playbooks) para Aplicativos de Lógica e Fluxo. Confira [exemplos de guias estratégicos](https://github.com/microsoftgraph/security-api-solutions/tree/master/Playbooks).
- Suporte no envio de [indicadores ameaças](/graph/api/resources/security-api-overview?view=graph-rest-beta&preserve-view=true#threat-indicators-preview) para o Microsoft Defender ATP para bloquear ou alertar ameaças usando suas próprias fontes de inteligência. Integrações com parceiros como o ThreatConnect permitem que os clientes enviem indicadores diretamente das soluções de inteligência e automação contra ameaças. 

### <a name="notifications"></a>Notificações
- [Crie e envie notificações](/graph/api/user-post-notifications?view=graph-rest-beta&preserve-view=true) a todos os clientes de aplicativos em todos os pontos de extremidade do dispositivo que um usuário está conectado, sem ter que gerenciar as permissões de usuário delegadas.
- Use [os pontos de extremidade da política de destino](/graph/api/resources/targetpolicyendpoints?view=graph-rest-beta&preserve-view=true) em [notificações](/graph/api/resources/notification?view=graph-rest-beta&preserve-view=true) do usuário para direcionar especificamente notificações para as plataformas Windows, iOS, Android ou WebPush.
- Especificar uma [política de retirada](/graph/api/resources/fallbackpolicy?view=graph-rest-beta&preserve-view=true) nas notificações para pontos de extremidade iOS, enviar notificações brutas de alta prioridade que podem não ser entregues aos dispositivos, caso contrário, devido a restrições específicas da plataforma, como o modo de economia de bateria.

 
### <a name="powershell-sdk"></a>SDK do PowerShell 
Os desenvolvedores e profissionais de TI podem observar o lançamento da [SDK do Microsoft Graph PowerShell](https://github.com/microsoftgraph/msgraph-sdk-powershell), que criará módulos que contêm cmdlets para criar solicitações da API REST do Microsoft Graph.

## <a name="september-2019-new-and-generally-available"></a>Setembro de 2019: novo e disponível para o público geral

### <a name="calendar-mail-and-group"></a>Calendário, email e grupo
[Obter o conteúdo bruto de um arquivo, ou o conteúdo MIME de um item](/graph/api/attachment-get?view=graph-rest-1.0&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment) que foi adicionado como um [anexo](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true) a um[evento](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true), [ mensagem](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)ou[ postagem](/graph/api/resources/post?view=graph-rest-1.0&preserve-view=true) de grupo.

### <a name="calendar-mail-outlook-task-personal-contact"></a>Calendário, email, tarefa do Outlook, contato pessoal
Use a função [translateExchange](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true) para converter uma ID de item do Outlook [entre](/graph/api/user-translateexchangeids?view=graph-rest-1.0&preserve-view=true#exchangeidformat-values)formatos suportados, incluindo o formato de ID padrão do Microsoft Graph e o formato de ID imutável. 

Os recursos a seguir são compatíveis com a conversão de formato de ID:

- [attachment](/graph/api/resources/attachment?view=graph-rest-1.0&preserve-view=true)
- [contato](/graph/api/resources/contact?view=graph-rest-1.0&preserve-view=true)
- [event](/graph/api/resources/event?view=graph-rest-1.0&preserve-view=true)
- [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-1.0&preserve-view=true)
- [message](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true)
- [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-1.0&preserve-view=true)

### <a name="mail"></a>Email
[Obter conteúdo MIME de uma mensagem](outlook-get-mime-message.md).

### <a name="microsoft-graph-toolkit"></a>Microsoft Graph Toolkit
Use o [Microsoft Graph Toolkit](toolkit/overview.md) para desenvolver aplicativos de produção que ofereçam uma aparência consistente do Microsoft 365 e economize tempo na autenticação e acesso a dados do Microsoft Graph.

## <a name="september-2019-new-in-preview"></a>Setembro de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [Setembro](changelog.md#september-2019) do Intune

### <a name="files"></a>Arquivos
- Suporte aprimorado à sincronização:

  - Use a nova propriedade **pendingOperations** para identificar operações que podem afetar o conteúdo binário de um [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true).
  - [Restaure](/graph/api/driveitem-restore?view=graph-rest-beta&preserve-view=true) um **driveItem** excluído. 
- Use o Algoritmo de Hash Seguro (SHA-256) para aprimorar a segurança e a integridade dos [dados](/graph/api/resources/file?view=graph-rest-beta&preserve-view=true) do arquivo.
- Obtenha ou defina a orientação de uma [foto](/graph/api/resources/photo?view=graph-rest-beta&preserve-view=true). A configuração é compatível com o OneDrive Personal.

### <a name="identity-and-access"></a>Identidade e acesso
- Use a propriedade new **identities** e obtenha as identidades que um [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) pode usar para entrar em uma conta. As identidades podem ser fornecidas por organizações ou provedores de identidade social, como Facebook, Google e Microsoft.
- Aperfeiçoamentos incrementais para [sincronizar identidades](/graph/api/resources/synchronization-overview?view=graph-rest-beta&preserve-view=true) em um aplicativo de nuvem para um locatário:

  - Armazenar configurações para um [trabalho de sincronização](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta&preserve-view=true)
  - Especifique um motivo para impor a [quarentena](/graph/api/resources/synchronization-quarantine?view=graph-rest-beta&preserve-view=true) a um trabalho de sincronização

### <a name="teamwork"></a>Trabalho em equipe
Use o canal **Geral** de uma [equipe](/graph/api/resources/team?view=graph-rest-beta&preserve-view=true) ou personalize as [configurações de membros](/graph/api/resources/teammembersettings?view=graph-rest-beta&preserve-view=true) para permitir que eles criem canais privados na **equipe**.

### <a name="users"></a>Usuários
- Obtenha ou atualize as identidades com as quais um [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true) pode entrar em uma conta. Essas identidades podem ser fornecidas por organizações de negócios ou por provedores de identidade social, como o Facebook, o Google e a Microsoft.
- Obtenha ou atualize as [configurações da caixa de correio](/graph/api/resources/mailboxsettings?view=graph-rest-beta&preserve-view=true) do formato de data e hora escolhidas pelo usuário.


## <a name="august-2019-new-and-generally-available"></a>Agosto de 2019: novo e disponível para o público geral 

### <a name="reports"></a>Relatórios
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0&preserve-view=true) sobre o tamanho e a contagem de itens excluídos.
- Acompanhe as IDs do grupo do Microsoft 365 ao [obter detalhes da atividade do grupo](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0&preserve-view=true).
- Rastreie o nome principal do proprietário ao obter [detalhes da conta de uso do OneDrive](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0&preserve-view=true) e [ detalhes de uso do site do SharePoint](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0&preserve-view=true).
- Obtenha o número de usuários ativos e inativos no Microsoft 365, ao [receber um relatório sobre contagens de usuários por serviço do Microsoft 365](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0&preserve-view=true).

### <a name="security"></a>Segurança
- Use o novo [complemento Microsoft Graph Security API para Splunk](https://aka.ms/graphsecuritysplunkaddon) para transmitir alertas de segurança e insights de muitos produtos de parceiros para o Splunk, permitindo uma correlação mais simples de seus dados de segurança. Para saber mais, confira o [comunicado](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Introducing-the-new-Microsoft-Graph-Security-API-add-on-for/ba-p/815972). 
- [Confira uma lista de outras soluções e conectores](security-integration.md) criados pela Microsoft ou por parceiros da Microsoft que se conectam à API de segurança e permitem que você trabalhe com dados em um formato unificado.


## <a name="august-2019-new-in-preview"></a>Agosto de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [agosto](changelog.md#august-2019) do Intune

### <a name="education"></a>Educação
- Associe um [professor](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true) ou uma [atribuição](/graph/api/resources/educationassignment?view=graph-rest-beta&preserve-view=true) com uma [lista de critérios de avaliação classificada](/graph/api/resources/educationrubric?view=graph-rest-beta&preserve-view=true) para considerar qualidades e níveis específicos em atribuições. Um exemplo de qualidade é a ortografia e a gramática, e exemplos de níveis são "bons" e "ruins". Você pode ainda associar pontos e pesos a lista de critérios de avaliação. Para saber mais, confira [visão geral da lista de critérios de avaliação educacional](education-rubric-overview.md).
- Avaliar uma atribuição e apresentar os resultados em termos de [feedback](/graph/api/resources/educationfeedbackoutcome?view=graph-rest-beta&preserve-view=true), de um [grau numérico](/graph/api/resources/educationpointsoutcome?view=graph-rest-beta&preserve-view=true), ou de [lista de critérios de avaliação](/graph/api/resources/educationrubricoutcome?view=graph-rest-beta&preserve-view=true).

### <a name="files"></a>Arquivos
Até esse ponto, você pode [seguir](/graph/api/driveitem-follow?view=graph-rest-beta&preserve-view=true) um [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true) para obter um acesso conveniente ou para facilitar ações como, mover, copiar e salvar como. Agora você pode usar a ação [deixar de seguir](/graph/api/driveitem-unfollow?view=graph-rest-beta&preserve-view=true) para parar de seguir esses itens da unidade.

### <a name="identity-and-access"></a>Identidade e acesso
- Os provedores de controle de acesso baseado em função (RBAC) podem [gerenciar funções](/graph/api/resources/rolemanagement?view=graph-rest-beta&preserve-view=true) do Azure Active Directory, [definindo ações de funções](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta&preserve-view=true)que podem ser realizadas em recursos específicos e [atribuindo funções](/graph/api/resources/unifiedroleassignment?view=graph-rest-beta&preserve-view=true) aos usuários com base em tais definições de função, fornecendo o acesso correspondente a esses recursos.
- Os administradores podem [listar as revisões de acesso](/graph/api/accessreview-list?view=graph-rest-beta&preserve-view=true) para facilitar de maneira eficiente a análise de associações de grupos, o acesso a aplicativos corporativos e as atribuições de funções. As revisões de acesso regular garantem que apenas as pessoas adequadas tenham acesso contínuo aos recursos de maneiras específicas.

### <a name="social-and-workplace-intelligence"></a>Inteligência social e do local de trabalho
Os usuários finais podem usar o aplicativo [MyAnalytics](social-intel-concept-overview.md#why-integrate-with-document-based-insights) do Microsoft 365 para obter insights sobre gerenciamento de tempo, colaboração no trabalho e equilíbrio profissional. Agora você pode usar a [API de análise](/graph/api/resources/social-overview?view=graph-rest-beta&preserve-view=true#help-users-gain-insights-into-their-work-patterns) para integrar dados sobre tempo gasto em atividades de trabalho, como chamadas, chats e email, para ajudar a melhorar a produtividade e o bem-estar do usuário. 


## <a name="july-2019-new-and-generally-available"></a>Julho de 2019: novo e disponível para o público geral 

### <a name="example-code-snippets"></a>Exemplo de trechos de código
Agora há trechos do código Objective-C em todos os tópicos da API nas referências v 1.0 e beta. Veja o exemplo do Objective-C de como [obter um evento](/graph/api/event-get?view=graph-rest-1.0&preserve-view=true&tabs=objective-c#example).

### <a name="group"></a>Grupo
- Use a função[validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0&preserve-view=true) para verificar se o nome de exibição ou apelido de email de um grupo existente do Microsoft 365 está em conformidade com as políticas de nomenclatura.
- Como alternativa, antes de criar o grupo, você pode usar a função[ ValidateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0&preserve-view=true)para um[directoryobject](/graph/api/resources/directoryobject?view=graph-rest-1.0&preserve-view=true) para validar primeiro os nomes.

### <a name="identity-and-access"></a>Identidade e acesso
- Use as [novas permissões delegadas e de aplicativo](permissions-reference.md#organization-permissions), _Organization.Read.All_ e _Organization.ReadWrite.All_ para acessar uma [organização](/graph/api/resources/organization?view=graph-rest-1.0&preserve-view=true) e recursos relacionados, como [SKUs inscritos](/graph/api/resources/subscribedsku?view=graph-rest-1.0&preserve-view=true).
- Use [novas permissões delegadas e de aplicativo](permissions-reference.md#role-management-permissions), _RoleManagement. Read.Directory_ e _RoleManagement. ReadWrite.Directory_, para controle de acesso baseado em função ( RBAC) para o diretório da empresa:

  - Use a permissão de leitura/gravação para [ativar](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0&preserve-view=true) primeiro uma função de diretório. 
  - Com a função ativada, você pode usar a permissão de leitura para[ler funções de diretório](/graph/api/directoryrole-list?view=graph-rest-1.0&preserve-view=true), [listar os membros da função](/graph/api/directoryrole-list-members?view=graph-rest-1.0&preserve-view=true) e [listar modelos de função de diretório](/graph/api/directoryroletemplate-list?view=graph-rest-1.0&preserve-view=true). 
  - Você também pode usar a permissão de leitura/gravação para[adicionar](/graph/api/directoryrole-post-members?view=graph-rest-1.0&preserve-view=true)e [remover](/graph/api/directoryrole-delete-member?view=graph-rest-1.0&preserve-view=true) membros da função.


## <a name="july-2019-new-in-preview"></a>Julho de 2019: Novo na visualização

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="calendar"></a>Calendário 
Use a nova [API de locais](/graph/api/resources/place?view=graph-rest-beta&preserve-view=true) para usar vários tipos de locais, como [salas](/graph/api/resources/room?view=graph-rest-beta&preserve-view=true) e [lista de salas](/graph/api/resources/roomlist?view=graph-rest-beta&preserve-view=true), conforme configurado pelos administradores do Exchange Online.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
Atualizações de [julho](changelog.md#july-2019) do Intune

### <a name="files"></a>Arquivos 
Aplique a data/hora de vencimento ou a senha ao [criar um link de compartilhamento](/graph/api/driveitem-createlink?view=graph-rest-beta&preserve-view=true) para um arquivo, pasta, ou outros [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access"></a>Identidade e acesso
- Use [nova permissão de aplicativo](./permissions-reference.md#access-reviews-permissions) _AccessReview.ReadWrite.Membership_ para operações CRUD nas [análises de acesso](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true). 
- Use [novas permissões delegadas e de aplicativo](permissions-reference.md#administrative-units-permissions),_AdministrativeUnit.Read.All_ e _AdministrativeUnit. ReadWrite.All_, para ler ou gravar respectivamente (incluindo criar, atualizar, excluir ou gerenciar a associação) recursos da [unidade de administração](/graph/api/resources/administrativeunit?view=graph-rest-beta&preserve-view=true).
- Use as [novas permissões delegadas e de aplicativo](permissions-reference.md#organization-permissions), _Organization.Read.All_ e _Organization.ReadWrite.All_ para acessar uma [organização](/graph/api/resources/organization?view=graph-rest-beta&preserve-view=true) e recursos relacionados, como [SKU inscritos](/graph/api/resources/subscribedsku?view=graph-rest-beta&preserve-view=true).
- Use a nova função[descobrir](/graph/api/directorydefinition-discover?view=graph-rest-beta&preserve-view=true) para encontrar o [esquema de sincronização](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta&preserve-view=true)de diretório mais recente, para sincronizar objetos de diretório, atributos e seus tipos de aplicativo.
- Use a [política de distribuição de recursos](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta&preserve-view=true) para ajudar os administradores de locatários a testar recursos em grupos específicos antes de habilitá-los para toda a organização.

### <a name="mail"></a>Email
Use permissões de aplicativo mais granulares _Mail.ReadBasic.All_ para ler a caixa de correio de um usuário, com exceção de qualquer corpo de mensagem, corpo de visualização, anexos e propriedades estendidas e com exceção da pesquisa na caixa de correio. Agora aplicável a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) e [controle de alterações](delta-query-overview.md) para [mensagem](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) e **mailFolder.**

### <a name="reports"></a>Relatórios
- Obtenha dados [adicionais de uso da caixa de correio](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta&preserve-view=true) sobre o tamanho e a contagem de itens excluídos.

### <a name="teamwork"></a>Trabalho em equipe
- [Instalar](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [desinstalar](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta&preserve-view=true), [atualizar ](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta&preserve-view=true) e [listar aplicativos do Microsoft Teams instalados ](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta&preserve-view=true) para um usuário. 
- Use o acesso somente para aplicativos para ler mensagens de canal, respostas a mensagens de canal e mensagens em um chat. [Solicite a aprovação](teams-protected-apis.md) para tal acesso.

## <a name="may---june-2019-new-and-generally-available"></a>Maio e julho de 2019: novo e disponível para o público geral

### <a name="calendar-mail-and-personal-contacts"></a>Calendário, email e contatos pessoais
Os administradores do Exchange podem conceder permissões de aplicativo a um aplicativo e [restringir o seu acesso apenas a um subconjunto de caixas de correio em um ](auth-limit-mailbox-access.md), ao invés do padrão, que é o acesso a todas as caixas de correio na organização. Este acesso restrito se aplicaria a quaisquer permissões de aplicativos concedidas ao aplicativo para [calendários](permissions-reference.md#calendars-permissions), [contatos](permissions-reference.md#contacts-permissions) e [configurações de email e de caixa de correio](permissions-reference.md#mail-permissions). Confira o [anúncio do blog](https://developer.microsoft.com/graph/blogs/scoping-microsoft-graph-application-permissions-to-specific-exchange-online-mailboxes/) relacionado.

### <a name="mail"></a>Email
Use a API de [pastas de pesquisa de email](/graph/api/resources/mailsearchfolder?view=graph-rest-1.0&preserve-view=true) para pesquisar mensagens e acessar os resultados de pesquisa de email do Outlook. Confira o [anúncio do blog](https://developer.microsoft.com/graph/blogs/mail-search-folder-support-for-microsoft-graph-apis/) relacionado.

### <a name="postman"></a>Postman
Como uma alternativa ao Explorador do Graph, experimente a API do Microsoft Graph na [coleção do Microsoft Graph Postman](use-postman.md) para aprender o comportamento da API e acelerar o desenvolvimento de aplicativos.

### <a name="tutorials"></a>Tutoriais
Experimente o novo [tutorial para criar um aplicativo de console do Java](/graph/tutorials/java) para obter informações sobre um calendário de usuário.

### <a name="user"></a>Usuário
Administradores ou usuários podem [revogar](/graph/api/user-revokesigninsessions?view=graph-rest-1.0&preserve-view=true) todos os tokens de atualização emitidos para um usuário. Isso geralmente é usado para impedir que aplicativos em um dispositivo perdido ou roubado acessem os dados de uma organização.


## <a name="may---june-2019-new-in-preview"></a>Maio e junho de 2019: novidades na versão prévia

> [!IMPORTANT]
> Os recursos, incluindo APIs e ferramentas, no status de _visualização_, podem ser alterados sem aviso prévio e alguns talvez nunca sejam promovidos ao status GA. Não use-os em aplicativos de produção.

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
- Atualizações de [maio](changelog.md#may-2019) do Intune 
- Atualizações de [junho](changelog.md#june-2019) do Intune

### <a name="education"></a>Educação
- Consulta Delta para um objeto [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta&preserve-view=true).
- Consulta Delta e adições de propriedade para objetos [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta&preserve-view=true) e [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta&preserve-view=true).

### <a name="group"></a>Grupo
Obtenha [rótulos de confidencialidade](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true) para ajudar a proteger dados confidenciais de grupos do Microsoft 365 e atender às políticas de conformidade. Esses rótulos são objetos [assignedLabel](/graph/api/resources/assignedlabel?view=graph-rest-beta&preserve-view=true), publicados por administradores no Centro de Conformidade e Segurança do Microsoft 365, como parte dos recursos de Proteção de Informações da Microsoft. 

### <a name="identity-and-access"></a>Identidade e acesso
- Obtenha uma instância de um [aplicativo](/graph/api/resources/applicationtemplate?view=graph-rest-beta&preserve-view=true) ou adicione uma instância da galeria de aplicativos do Azure AD ao seu diretório como modelo.
- Obtenha um log de todos os diretórios de[eventos de provisionamento](/graph/api/resources/provisioningobjectsummary?view=graph-rest-beta&preserve-view=true) em um locatário.
- Obtenha informações sobre [usuário detectado ou riscos de login](/graph/api/resources/riskdetection?view=graph-rest-beta&preserve-view=true) em um ambiente do Azure AD. Esta funcionalidade de detecção de riscos faz parte do Azure AD Identity Protection.

### <a name="mail"></a>Email
Use permissões de aplicativo mais detalhadas _Mail.ReadBasic.All_ para ler a caixa de correio de um usuário, com exceção de qualquer corpo de mensagem, corpo de visualização, anexos e propriedades estendidas e com exceção da pesquisa na caixa de correio. Disponível para métodos de leitura [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta&preserve-view=true) e [controle de alterações](delta-query-overview.md) para [mensagem](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) e **mailFolder.**

### <a name="microsoft-graph-toolkit"></a>Kit de ferramentas do Microsoft Graph
O [kit de ferramentas do Microsoft Graph](./toolkit/overview.md) é um conjunto de colaboradores e de componentes da Web de estrutura independente que oferece conveniência para autenticar e acessar dados no Microsoft Graph. Como o kit de ferramentas do Microsoft Graph está no status de visualização, use provedores e componentes do kit de ferramentas somente em aplicativos que não são de produção.

### <a name="reports"></a>Relatórios
- Obtenha [relatórios sobre os métodos de autenticação](/graph/api/resources/authenticationmethods-usage-insights-overview?view=graph-rest-beta&preserve-view=true) adotados pelos usuários em uma organização, como rest de senha de autoatendimento e autenticação multifator (MFA).

### <a name="sites"></a>Sites
Permitir que os usuários [sigam](/graph/api/site-follow?view=graph-rest-beta&preserve-view=true) ou [parem de seguir](/graph/api/site-unfollow?view=graph-rest-beta&preserve-view=true) os sites do SharePoint.

### <a name="teamwork"></a>Trabalho em equipe
- Hospede [imagens](/graph/api/resources/chatmessagehostedimage?view=graph-rest-beta&preserve-view=true) em [mensagens de bate-papo](/graph/api/resources/chatmessage?view=graph-rest-beta&preserve-view=true) do Microsoft Teams.
- Suporte para [configurar](/graph/api/resources/teamdiscoverysettings?view=graph-rest-beta&preserve-view=true) como uma equipe privada pode ser descoberta.


## <a name="january---april-2019-new-and-generally-available"></a>Janeiro a abril de 2019: novo e disponível para o público geral

[Microsoft Graph data connect](data-connect-concept-overview.md)

### <a name="calendar"></a>Calendário
[Obter agenda de disponibilidade](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>Identidade e acesso
[Fornecedores de identidade](/graph/api/resources/identityprovider?view=graph-rest-1.0&preserve-view=true)
[melhores guias de autenticação](./auth/index.yml)
[migrando aplicativos do Azure AD Graph para o Microsoft Graph](migrate-azure-ad-graph-planning-checklist.md)

### <a name="sdks"></a>SDKs
[Guias SDK](/sdks/sdks-overview.md)Trechos de API ([exemplo](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true&tabs=cs#sdk-sample-code))

### <a name="security"></a>Segurança
[Classificação de segurança do locatário](/graph/api/resources/securescore?view=graph-rest-1.0&preserve-view=true)

## <a name="january---april-2019-new-in-preview"></a>Janeiro a abril de 2019: novo na versão prévia

### <a name="calendar-group-mail-to-do-tasks"></a>Calendário, grupo, email, tarefas pendentes
[Obter o conteúdo bruto/MIME de anexos de arquivo ou item](/graph/api/attachment-get?view=graph-rest-beta&preserve-view=true#get-the-raw-contents-of-a-file-or-item-attachment) para um evento, mensagem, tarefa do Outlook ou postagem do grupo

### <a name="change-notifications"></a>Notificações de alteração
[Reduzir notificações ausentes de alteração](webhooks-lifecycle.md)

### <a name="devices-and-apps"></a>Dispositivos e aplicativos
- Atualizações [de](changelog.md#january-2019) janeiro do Intune 
- Atualizações [de](changelog.md#february-2019) fevereiro do Intune
- Atualizações [de](changelog.md#march-2019) março do Intune
- Atualizações [de](changelog.md#april-2019) abril do Intune

### <a name="files"></a>Arquivos
[Compartilhamento de convite](/graph/api/driveitem-invite?view=graph-rest-beta&preserve-view=true) inclui data de vencimento e senha

### <a name="financials"></a>Finanças
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>Identidade e acesso
[O Access revisa](/graph/api/resources/accessreviews-root?view=graph-rest-beta&preserve-view=true) as permissões de aplicativo suporte [auditoria e registros](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta&preserve-view=true)
[de entrada personalizado, entre e inscreva-se no Azure AD B2C](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta&preserve-view=true)
[usuário arriscado](/graph/api/resources/riskyuser?view=graph-rest-beta&preserve-view=true) e [histórico](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta&preserve-view=true)

### <a name="mail"></a>Correio
[Obter conteúdo MIME de mensagens](outlook-get-mime-message.md)

### <a name="reports"></a>Relatórios
[Relatórios de entrada do aplicativo](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta&preserve-view=true)

### <a name="security"></a>Segurança
[Indicadores de ameaça ](/graph/api/resources/securityaction?view=graph-rest-beta&preserve-view=true)
[de Ações de segurança](/graph/api/resources/tiindicator?view=graph-rest-beta&preserve-view=true)

### <a name="teamwork"></a>Trabalho em equipe
[O gerenciamento](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)
[de conversas em 1:1](/graph/api/resources/shift?view=graph-rest-beta&preserve-view=true)

## <a name="see-also"></a>Confira também
- Confira [O que há de novo](whats-new-overview.md) no Microsoft Graph.
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](changelog.md).