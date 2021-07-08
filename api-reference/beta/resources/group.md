---
title: tipo de recurso de grupo
description: Representa um grupo do Diretório Ativo do Azure (Azure AD), que pode ser um grupo do Microsoft 365, uma equipe do Microsoft Teams ou um grupo de segurança.
localization_priority: Priority
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 36204bb6421ef294bf300f6d72f79bef133d9ec6
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317060"
---
# <a name="group-resource-type"></a>tipo de recurso de grupo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo do Diretório Ativo do Azure (Azure AD), que pode ser um grupo do Microsoft 365, uma equipe do Microsoft Teams ou um grupo de segurança. Herda do [directoryObject](directoryobject.md).

Por motivos de desempenho, as operações [create](../api/group-post-groups.md), [get](../api/group-get.md) e [list](../api/group-list.md) retornam por padrão apenas um subconjunto das propriedades usadas com mais frequência. Essas propriedades _padrão_ estão listadas na seção [Propriedades](#properties). Para obter as propriedades não retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).

> O **Microsoft Teams e os grupos do Microsoft 365 oferecem suporte à colaboração em grupo**. Você pode usar a maioria das APIs de grupos do Microsoft 365 com o Microsoft Teams. Para criar uma [equipe](team.md), primeiro [crie o grupo](../api/group-post-groups.md) e, em seguida, [adicionar uma equipe para ele](../api/team-put-teams.md). Para obter detalhes, confira a [visão geral do Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:------ |:----------- |:----------- |
| **Gerenciamento de grupos** |||
| [Criar grupo](../api/group-post-groups.md) | [group](group.md) | Crie um novo grupo conforme especificado. Pode ser um grupo, grupo dinâmico, grupo de segurança ou equipe do Microsoft 365. |
| [Obter grupo](../api/group-get.md) | [grupo](group.md) | Ler as propriedades e as relações do objeto do grupo. |
| [Atualizar grupo](../api/group-update.md) | Nenhum | Atualizar as propriedades de um objeto group. |
| [Excluir grupo](../api/group-delete.md) | Nenhum | Excluir um objeto group. |
| [Listar grupos](../api/group-list.md) | [group](group.md) | Ler as propriedades e as relações de todos os objetos do grupo. |
| [delta](../api/group-delta.md) | Coleção group | Obter alterações incrementais para grupos. |
| [Adicionar membro](../api/group-post-members.md) | [directoryObject](directoryobject.md) | Adicionar um usuário ou grupo a esse grupo postando na propriedade de navegação **members** (com suporte somente para grupos de segurança e grupos de segurança habilitados para email). |
| [Adicionar proprietário](../api/group-post-owners.md) | [directoryObject](directoryobject.md) | Adicionar um novo proprietário para o grupo postando na propriedade de navegação **owners** (com suporte somente para grupos de segurança e grupos de segurança habilitados para email). |
| [Criar configuração](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) | Criar um objeto de configuração com base em um directorySettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo. Somente modelos específicos de grupos podem ser usados para essa operação. |
| [Excluir configuração](../api/directorysetting-delete.md) | Nenhum | Excluir um objeto de configuração. |
| [Obter o ponto de extremidade](../api/endpoint-get.md) | [ponto de extremidade](endpoint.md) | Leia as propriedades e os relacionamentos do objeto ponto de extremidade. |
| [Obter configuração](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) | Ler propriedades de um objeto de configuração específico. |
| [Listar pontos de extremidade](../api/group-list-endpoints.md) | conjunto [ponto de extremidade](endpoint.md)  | Obtenha uma coleção de o objeto ponto de extremidade. |
| [Listar membros](../api/group-list-members.md) | Coleção [directoryObject](directoryobject.md) | Obter os usuários e grupos que são membros diretos desse grupo da propriedade de navegação **members**. |
| [Listar memberOf](../api/group-list-memberof.md) | Coleção [directoryObject](directoryobject.md) | Obter os grupos e as unidades administrativas dos quais esse grupo é membro direto, da propriedade de navegação memberOf. |
| [Listar groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) | Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md) | Listar políticas de ciclo de vida de grupo. |
| [Listar proprietários](../api/group-list-owners.md) | Coleção [directoryObject](directoryobject.md) | Obter os proprietários do grupo da propriedade de navegação **owners**. |
| [Listar configurações](../api/directorysetting-list.md) | conjunto [directorySetting](directorysetting.md) | Lista propriedades de todos os objetos de configuração. |
| [Listar membros transitivos](../api/group-list-transitivemembers.md) | Coleção [directoryObject](directoryobject.md) | Obtenha os usuários, grupos, dispositivos e entidades de serviço que são membros, incluindo membros aninhados desse grupo. |
| [Listar memberOf transitivos](../api/group-list-transitivememberof.md) | Coleção [directoryObject](directoryobject.md) | Listar as unidades administrativas e grupos dos quais esse grupo é membro. Essa operação é transitiva e inclui os grupos que são membros aninhados desse grupo. |
| [Remover proprietário](../api/group-delete-owners.md) | Nenhum | Remover um proprietário de um grupo do Microsoft 365, de um grupo de segurança ou de um grupo de segurança habilitado para email por meio da propriedade de navegação **owners**. |
| [Remover membro](../api/group-delete-members.md) | Nenhum | Remover um membro de um grupo do Microsoft 365, de um grupo de segurança ou de um grupo de segurança habilitado para email por meio da propriedade de navegação **members**. É possível remover usuários ou outros grupos. |
| [Atualizar configuração](../api/directorysetting-update.md) | [directorySetting](directorysetting.md) | Atualizar um objeto setting. |
| [assignLicense](../api/group-assignlicense.md) | [group](group.md) | Adicione ou remova inscrições para o grupo. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura. |
| [checkMemberGroups](../api/group-checkmembergroups.md) | Coleção de cadeias de caracteres | Verificar associação em uma lista de grupos. Essa função é transitiva. |
| [checkMemberObjects](../api/group-checkmemberobjects.md) | Coleção de cadeias de caracteres | Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa. A função é transitiva. |
| [evaluateDynamicMembership](../api/group-evaluatedynamicmembership.md) | [evaluateDynamicMembershipResult](evaluatedynamicmembershipresult.md) | Avaliar se um usuário ou dispositivo é ou seria membro de um grupo dinâmico. |
| [getMemberGroups](../api/group-getmembergroups.md) | Coleção de cadeias de caracteres | Retornar todos os grupos dos quais o grupo é membro. Essa função é transitiva. |
| [getMemberObjects](../api/group-getmemberobjects.md) | Coleção de cadeias de caracteres | Retornar todas as unidades administrativas e grupos dos quais o grupo é membro. Essa função é transitiva. |
| [validateProperties](../api/group-validateproperties.md) | JSON | Validar se o nome de exibição de um grupo do Microsoft 365 ou apelido de email está em conformidade com as políticas de nomenclatura. |
| **Atribuição de funções do aplicativo** |||
| [List appRoleAssignments](../api/group-list-approleassignments.md) | [appRoleAssignment](approleassignment.md) collection | Obter os aplicativos e funções do aplicativo atribuídos a esse grupo. |
| [Adicionar uma atribuição de função do aplicativo](../api/group-post-approleassignments.md) | [appRoleAssignment](approleassignment.md) | Atribuir uma função do aplicativo a esse grupo. |
| [Remover uma atribuição de função do aplicativo](../api/group-delete-approleassignments.md) | Nenhum. | Remover uma atribuição de função do aplicativo desse grupo. |
| **Calendar** |||
| [Criar evento](../api/group-post-events.md) | [event](event.md) | Criar um novo Event postando na coleção de eventos. |
| [Obter evento](../api/group-get-event.md) | [event](event.md) | Ler as propriedades de um objeto event. |
| [Listar eventos](../api/group-list-events.md) | Coleção [event](event.md) | Obter uma coleção de objetos de evento. |
| [Atualizar evento](../api/group-update-event.md) | Nenhum | Atualizar as propriedades de um objeto event. |
| [Excluir evento](../api/group-delete-event.md) | Nenhum | Excluir o objeto event. |
| [Listar calendarView](../api/group-list-calendarview.md) | Coleção [event](event.md) | Obter um conjunto de eventos em uma janela de tempo especificada. |
| **Conversas** |||
| [Criar conversa](../api/group-post-conversations.md) | [conversa](conversation.md) | Crie uma nova conversa postando na coleção de conversas. |
| [Obter conversa](../api/group-get-conversation.md) | [conversation](conversation.md) | Ler as propriedades de um objeto conversation. |
| [Listar conversas](../api/group-list-conversations.md) | Coleção [conversation](conversation.md) | Obter uma coleção de objetos Conversation. |
| [Excluir conversa](../api/group-delete-conversation.md) | Nenhum | Excluir objeto conversation. |
| [Criar thread](../api/group-post-threads.md) | [conversationThread](conversationthread.md) | Criar um novo thread de conversa. |
| [Acessar thread](../api/group-get-thread.md) | [conversationThread](conversationthread.md) | Ler as propriedades de um objeto thread. |
| [Listar threads](../api/group-list-threads.md) | Coleção [conversationThread](conversationthread.md) | Obter todos os threads de um grupo. |
| [Atualizar thread](../api/group-update-thread.md) | Nenhum | Atualizar as propriedades de um objeto thread. |
| [Excluir thread](../api/group-delete-thread.md) | Nenhum | Excluir objeto thread |
| [Listar acceptedSenders](../api/group-list-acceptedsenders.md) | Coleção [directoryObject](directoryobject.md) | Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo. |
| [Adicionar acceptedSender](../api/group-post-acceptedsenders.md) | [directoryObject](directoryobject.md) | Adicionar um Usuário ou Grupo à coleção acceptSenders. |
| [Remover acceptedSender](../api/group-delete-acceptedsenders.md) | [directoryObject](directoryobject.md) | Remover um Usuário ou Grupo da coleção acceptedSenders. |
| [Listar rejectedSenders](../api/group-list-rejectedsenders.md) | Coleção [directoryObject](directoryobject.md) | Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo. |
| [Adicionar rejectedSender](../api/group-post-rejectedsenders.md) | [directoryObject](directoryobject.md) | Adicionar um novo Usuário ou Grupo à coleção rejectedSenders. |
| [Remover rejectedSender](../api/group-delete-rejectedsenders.md) | [directoryObject](directoryobject.md) | Remover um novo Usuário ou Grupo da coleção Remetentesrejeitados. |
| **Extensões abertas** |||
| [Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso. |
| [Obter extensão aberta](../api/opentypeextension-get.md) | Coleção [openTypeExtension](opentypeextension.md) | Obtenha uma extensão aberta identificada pelo nome da extensão. |
| **Extensões de esquema** |||
| [Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) | Nenhum | Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso. |
| **Outros recursos de grupo** |||
| [Listar fotos](../api/group-list-photos.md) | Coleção [profilePhoto](photo.md) | Obter um conjunto de fotos de perfil para o grupo. |
| [Listar plannerPlans](../api/plannergroup-list-plans.md) | Coleção [plannerPlan](plannerplan.md) | Obter os planos de planejador pertencentes ao grupo. |
| [Listar as permissionGrants](../api/group-list-permissiongrants.md) | Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Liste as permissões que foram concedidas aos aplicativos para acessar o grupo. |
| **Configurações do usuário** |||
| [addFavorite](../api/group-addfavorite.md) | Nenhum | Adicionar o grupo à lista de grupos favoritos do usuário conectado. Suportado apenas para grupos do Microsoft 365. |
| [removeFavorite](../api/group-removefavorite.md) | Nenhum | Remova o grupo da lista de grupos favoritos do usuário que se inscreveu. Somente grupos do Microsoft 365 com suporte. |
| [Listar memberOf](../api/group-list-memberof.md) | Coleção [directoryObject](directoryobject.md) | Obter os grupos e unidades administrativas dos quais esse usuário é um membro direto a partir da propriedade de navegação **memberOf**. |
| [Listar joinedTeams](../api/user-list-joinedteams.md) | Coleção [group](group.md) | Obtenha as equipes do Microsoft Teams das quais o usuário é um membro direto. |
| [subscribeByMail](../api/group-subscribebymail.md) | Nenhum | Defina a propriedade isSubscribedByMail como `true`. Permitir que o usuário conectado receba conversas por email. Apenas grupos do Microsoft 365 são suportados. |
| [unsubscribeByMail](../api/group-unsubscribebymail.md) | Nenhum | Defina a propriedade isSubscribedByMail como `false`. Desabilitar o recebimento de conversas por email do usuário conectado. Apenas grupos do Microsoft 365 são suportados. |
| [resetUnseenCount](../api/group-resetunseencount.md) | Nenhum | Redefinir a Contagem Não Vista para 0 de todas as postagens que o usuário que se inscreveu não viu desde sua última visita. Somente grupos do Microsoft 365 com suporte. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean| Indica se as pessoas externas à empresa podem enviar mensagens para o grupo. O valor padrão é `false`. <br><br>Retornado apenas em `$select`. Com suporte apenas para Obter API de grupo (`GET /groups/{ID}`) |
|assignedLabels|coleção [assignedLabel](assignedlabel.md)|Lista de pares de rótulos de confidencialidade (ID do rótulo, nome do rótulo) associados a um grupo do Microsoft 365. <br><br>Retornado apenas em `$select`.|
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao grupo. <br><br>Retornado apenas em `$select`. Somente leitura.|
|autoSubscribeNewMembers|Boolean|Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email. Você pode definir essa propriedade em uma solicitação PATCH para o grupo. Não a defina na solicitação POST inicial que cria esse grupo. O valor padrão é `false`. <br><br>Retornado apenas em `$select`. Com suporte apenas para Obter API de grupo (`GET /groups/{ID}`)|
|classificação|String|Descreve uma classificação para o grupo (como impacto comercial baixo, médio ou alto). Os valores válidos para esta propriedade são definidos criando um valor de [configuração](directorysetting.md) ClassificationList com base na [definição de modelo](directorysettingtemplate.md).<br><br>Retornado por padrão.|
|createdByAppId|Cadeia de caracteres|ID do aplicativo usado para criar o grupo. Pode ser nulo para alguns grupos. <br><br>Retornado por padrão. Somente leitura. Oferece suporte para `$filter`.|
|createdDateTime|DateTimeOffset| Carimbo de data/hora da ocasião em que o grupo foi criado. Não é possível modificar o valor e ele é preenchido automaticamente quando o grupo é criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado por padrão. Somente leitura. |
|deletedDateTime|DateTimeOffset| Para alguns objetos do Azure Active Directory (usuário, grupo, aplicativo), se o objeto for excluído, ele será excluído primeiro logicamente e essa propriedade será atualizada com a data e a hora em que o objeto foi excluído. Caso contrário, essa propriedade é nula. Se o objeto for restaurado, essa propriedade será atualizada para nula. |
|description|String|Uma descrição opcional para o grupo. <br><br>Retornado por padrão.|
|displayName|String|O nome de exibição do grupo. Esta propriedade é necessária quando um grupo é criado e não pode ser limpa durante as atualizações.<br><br>Retornado por padrão. Oferece suporte para `$filter` e `$orderby`. |
|expirationDateTime|DateTimeOffset| Data e hora de quando o grupo está configurado para expirar. Não é possível modificar o valor e ele é preenchido automaticamente quando o grupo é criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado por padrão. Somente leitura. |
|groupTypes|Coleção de cadeias de caracteres| Especifica o tipo de grupo e sua associação.  <br><br>Se a coleção contiver `Unified`, o grupo será um grupo do Microsoft 365; caso contrário, será um grupo de segurança ou um grupo de distribuição. Para obter detalhes, confira [visão geral sobre grupos](groups-overview.md).<br><br>Se a coleção inclui `DynamicMembership`, o grupo tem associação dinâmica; caso contrário, a associação é estática.  <br><br>Retornado por padrão. Oferece suporte para `$filter`.|
|hasMembersWithLicenseErrors|Boolean| Indica se existem membros neste grupo com erros de licença da sua atribuição de licença baseada em grupo. <br><br>Esta propriedade nunca é retornada em uma operação GET. Você pode usá-lo como um argumento $filter para acessar os grupos que têm membros com erros de licença (ou seja, o filtro para essa propriedade é `true`).|
|hideFromAddressLists |Booliano |`true` se o grupo não for exibido em certas partes da interface do usuário do Outlook: no **Catálogo de Endereços**, nas listas de endereços para selecionar os destinatários da mensagem e na caixa de diálogo **Procurar Grupos** para pesquisar grupos; caso contrário, false. O valor padrão é `false`. <br><br>Retornado apenas em `$select`. Com suporte apenas para Obter API de grupo (`GET /groups/{ID}`)|
|hideFromOutlookClients |Booliano |`true` se o grupo não for exibido em clientes Outlook, como Outlook para Windows e Outlook na Web, caso contrário, false. O valor padrão é `false`. <br><br>Retornado apenas em `$select`. Com suporte apenas para Obter API de grupo (`GET /groups/{ID}`)|
|id|String|O identificador exclusivo do grupo. <br><br>Retornado por padrão. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|isAssignableToRole|Booliano|Indica se este grupo pode ser atribuído a uma função do Azure Active Directory.<br><br>Esta propriedade só pode ser definida durante a criação do grupo e é imutável. Se definida como `true`, a propriedade **securityEnabled** também deverá ser definida como `true` e o grupo não poderá ser um grupo dinâmico (ou seja, **groupTypes** não pode conter `DynamicMembership`). Somente chamadores em funções de Administrador global e de Administrador de funções com privilégios podem definir essa propriedade. O chamador também deve receber a permissão *Directory.AccessAsUser.All* para definir essa propriedade. Para obter mais informações, confira [Usando um grupo para gerenciar atribuições de função do Azure Active Directory](https://go.microsoft.com/fwlink/?linkid=2103037)<br><br>Retornado por padrão.|
|infoCatalogs|Conjunto de cadeias de caracteres|Identifica os segmentos de informações atribuídos ao grupo. Retornado por padrão.|
|isSubscribedByMail|Boolean|Indica se o usuário conectado está inscrito para receber conversas de email. O valor padrão é `true`. <br><br>Retornado apenas em `$select`. Com suporte apenas para Obter API de grupo (`GET /groups/{ID}`) |
|licenseProcessingState|String|Indica o status da atribuição de licença de grupo para todos os membros do grupo. Valores possíveis: `QueuedForProcessing`, `ProcessingInProgress` e `ProcessingComplete`. <br><br>Retornado apenas em `$select`. Somente leitura. |
|email|String|O endereço SMTP do grupo, por exemplo, "serviceadmins@contoso.onmicrosoft.com". <br><br>Retornado por padrão. Somente leitura. Oferece suporte para `$filter`.|
|mailEnabled|Boolean|Especifica se o grupo está habilitado para email. <br><br>Retornado por padrão.|
|mailNickname|String|O alias de email do grupo, exclusivo na organização. Essa propriedade deve ser especificada quando um grupo é criado. Esses caracteres não podem ser usados no mailNickName: `@()\[]";:.<>,SPACE`. <br><br>Retornado por padrão. Oferece suporte para `$filter`.|
|membershipRule|String|A regra que determina membros para esse grupo se o grupo for um grupo dinâmico (groupTypes contém `DynamicMembership`). Para saber mais sobre a sintaxe da regra de associação, confira [sintaxe regras de associação](https://azure.microsoft.com/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/). <br><br>Retornado por padrão. |
|membershipRuleProcessingState|String|Indica se o processamento de associação dinâmica está ativado ou em pausa. Os valores possíveis são: `On` ou `Paused`. <br><br>Retornado por padrão. |
|membershipRuleProcessingStatus|[membershipRuleProcessingStatus](membershipruleprocessingstatus.md) |Descreve o status de processamento para grupos dinâmicos baseados em regras. A propriedade é `null` para grupos dinâmicos não baseados em regras ou se o processamento do grupo dinâmico foi pausado. <br><br>Retornado apenas em `$select`. Oferece suporte para `$filter`. Somente leitura. |
|onPremisesDomainName|Cadeia de Caracteres|Contém o **nome de domínio totalmente qualificado (FQDN)** local, também chamado de **dnsDomainName** sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect.<br><br>Retornado por padrão. Somente leitura. |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o grupo foi sincronizado com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado por padrão. Somente leitura. Oferece suporte para `$filter`.|
|onPremisesNetBiosName|Cadeia de Caracteres|Contém o **netBios name** local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect.<br><br>Retornado por padrão. Somente leitura. |
|onPremisesProvisioningErrors|coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante a configuração. <br><br>Retornado por padrão.|
|onPremisesSamAccountName|Cadeia de Caracteres|Contém o **nome da conta SAM** local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect.<br><br>Retornado por padrão. Somente leitura. |
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do grupo que foi sincronizado do local com a nuvem. <br><br>Retornado por padrão. Somente leitura. |
|onPremisesSyncEnabled|Booliano|`true` se esse grupo está sincronizado de um diretório local; `false` se esse grupo foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). <br><br>Retornado por padrão. Somente leitura. Oferece suporte para `$filter`.|
|preferredDataLocation|String|O local de data preferido para o grupo. Saiba mais em [OneDrive Online com Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction). <br><br>Retornado por padrão.|
|preferredLanguage|String|O idioma preferido para um grupo Microsoft 365. Deve seguir o Código ISO 639-1; por exemplo "en-US". <br><br>Retornado por padrão. |
|proxyAddresses|String collection| Endereços de email para o grupo que direcionam para a mesma caixa de correio do grupo. Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. <br><br>Retornado por padrão. Somente leitura. Não anulável. Oferece suporte para `$filter`. |
|renewedDateTime|DateTimeOffset| Carimbo de data/hora da ocasião em que o grupo foi renovado pela última vez. Não é possível modificar isso diretamente e a atualização ocorre apenas por meio da [ação de renovação de serviço](../api/grouplifecyclepolicy-renewgroup.md). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado por padrão. Somente leitura.|
|resourceBehaviorOptions|Conjunto de cadeias de caracteres|Especifica os comportamentos de grupo que podem ser configurados para um grupo do Microsoft 365 durante sua criação. Isso só pode ser definido como parte da criação (POST). Os valores possíveis são `AllowOnlyMembersToPost`, `HideGroupInOutlook`, `SubscribeNewGroupMembers`, `WelcomeEmailDisabled`. Para obter mais informações, confira o artigo [Definir as opções de provisionamento e comportamentos de grupo do Microsoft 365 ](/graph/group-set-options).|
|resourceProvisioningOptions|Conjunto de cadeias de caracteres|Especifica os recursos de grupo provisionados como parte da criação de grupos do Microsoft 365 que não costumam fazer parte do processo padrão de criação de grupos. Um valor possível é `Team`. Para obter mais informações, confira o artigo [Definir as opções de provisionamento e comportamentos de grupo do Microsoft 365 ](/graph/group-set-options).|
|securityEnabled|Boolean|Especifica se o grupo é um grupo de segurança. <br><br>Retornado por padrão. Oferece suporte para `$filter`.|
|securityIdentifier|Cadeia de Caracteres|Identificador de segurança do grupo, usado em cenários do Windows. <br><br>Retornado por padrão.|
|tema|Cadeia de caracteres|Especifica o tema de cor de um grupo do Microsoft 365. Os valores possíveis são: `Teal`, `Purple`, `Green`, `Blue`,`Pink`, `Orange` ou `Red`. <br><br>Retornado por padrão. |
|unseenConversationsCount|Int32|Contagem de conversas que receberam uma ou mais novas postagens desde a última visita do usuário conectado ao grupo. Essa propriedade é igual a **unseenCount**. <br><br>Retornado apenas em `$select`.|
|unseenCount|Int32|Contagem das conversas que receberam novas postagens desde que o usuário conectado visitou o grupo pela última vez. Essa propriedade é igual a **unseenConversationsCount**.<br><br>Retornado apenas em `$select`. Suportado apenas para Obter API de grupo (`GET /groups/{ID}`). |
|unseenMessagesCount|Int32|Contagem de novas postagens que foram entregues às conversas do grupo desde a última visita do usuário conectado ao grupo. <br><br>Retornado apenas em `$select`.|
|visibility|Cadeia de caracteres| Especifica a política de associação ao grupo e a visibilidade do conteúdo do grupo para grupos. Os valores possíveis são: `Private`, `Public` ou `Hiddenmembership`. `Hiddenmembership` pode ser definido apenas para grupos do Microsoft 365, quando os grupos são criados. Não pode ser atualizado posteriormente. Outros valores de visibilidade podem ser atualizados após a criação do grupo.<br> Se o valor de visibilidade não for especificado durante a criação do grupo no Microsoft Graph, um grupo de segurança é criado como `Private` por padrão e o grupo Microsoft 365 é `Public`. Saiba mais em [Opções de visibilidade do grupo](#group-visibility-options). <br><br>Retornado por padrão.|

### <a name="group-visibility-options"></a>Opções de visibilidade do grupo

|Valor|Descrição|
|:----|-----------|
| Público | Qualquer pessoa pode ingressar no grupo sem precisar de permissão de proprietário.<br>Qualquer pessoa pode exibir o conteúdo do grupo.|
| Privado | A permissão de proprietário é necessária para ingressar no grupo.<br>Não membros não podem exibir o conteúdo do grupo.|
| Hiddenmembership | A permissão de proprietário é necessária para ingressar no grupo.<br>Não membros não podem exibir o conteúdo do grupo.<br>Não membros não podem ver os membros do grupo.<br>Administradores (global, empresa, usuário e helpdesk) podem visualizar a associação do grupo.<br>O grupo aparece no catálogo de endereços global (GAL).|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|acceptedSenders|Coleção [directoryObject](directoryobject.md)|A lista de usuários ou grupos que têm permissão para criar eventos de calendário ou postagens nesse grupo. Se essa lista não estiver vazia, somente os usuários ou grupos listados aqui poderão fazer postagens.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Representa as funções de aplicativo que um grupo recebeu para um aplicativo. |
|calendar|[calendar](calendar.md)|O calendário do grupo. Somente leitura.|
|calendarView|Coleção [event](event.md)|O modo de exibição do calendário. Somente leitura.|
|conversations|Coleção [conversation](conversation.md)|As conversas do grupo.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| O usuário (ou aplicativo) que criou o grupo. **Observação:** isso não será definido se o usuário for um administrador. Somente leitura.|
|drive|[unidade](drive.md)|A unidade padrão do grupo. Somente leitura.|
|unidades|Coleção [drive](drive.md)|As unidades do grupo. Somente leitura.|
|pontos de extremidade|conjunto [Ponto de extremidade](endpoint.md)| Pontos de extremidade do grupo. Somente leitura. Anulável.|
|eventos|Coleção [event](event.md)|Eventos do grupo.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o grupo. Somente leitura. Anulável.|
|groupLifecyclePolicies|Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)|A coleção de políticas de ciclo de vida para este grupo. Somente leitura. Anulável.|
|memberOf|Coleção [directoryObject](directoryobject.md)|Grupos e unidades administrativas das que esse grupo faz parte. Métodos HTTP: GET (com suporte para todos os grupos). Somente leitura. Nullable.|
|membros|Coleção [directoryObject](directoryobject.md)| Usuários, contatos e grupos que são membros desse grupo. Métodos HTTP: GET (com suporte para todos os grupos), POST (com suporte para grupos de segurança e grupos de segurança habilitados para email), DELETE (com suporte apenas para grupos de segurança) Somente leitura. Nullable.|
|membersWithLicenseErrors|Coleção [usuário](user.md)|Uma lista de membros do grupo com erros de licença desta atribuição de licença baseada em grupo. Somente leitura.|
|onenote|[onenote](onenote.md)| Somente leitura.|
|owners|Coleção [directoryObject](directoryobject.md)|Os proprietários do grupo. Os proprietários são um conjunto de usuários não administradores que têm permissão para modificar esse objeto. Métodos HTTP: GET (com suporte para todos os grupos), POST (com suporte para grupos de segurança e grupos de segurança habilitados para email), DELETE (com suporte apenas para grupos de segurança) Somente leitura. Nullable.|
|permissionGrants|[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)|As permissões que foram concedidas a um grupo para um aplicativo específico.|
|photo|[profilePhoto](profilephoto.md)| A foto de perfil do grupo. |
|fotos|Coleção [profilePhoto](profilephoto.md)| As fotos de perfil pertencentes ao grupo. Somente leitura. Anulável.|
|planejador|[plannerGroup](plannergroup.md)| Serviços do Planejador Seletivo disponíveis para o grupo. Somente leitura. Nullable. |
|rejectedSenders|Coleção [directoryObject](directoryobject.md)|A lista de usuários ou grupos que não têm permissão para criar eventos de calendário ou postagens nesse grupo. Anulável|
|configurações|conjunto [directorySetting](directorysetting.md)| Configurações que podem reger o comportamento desse grupo, como se os membros podem convidar usuários convidados para o grupo. Nullable.|
|sites|conjunto de [sites](site.md)|A lista de sites do SharePoint nesse grupo. Acesse o site padrão com /sites/root.|
|threads|Coleção [conversationThread](conversationthread.md)| Os threads de conversas do grupo. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "drives",
    "endpoints",
    "events",
    "extensions",
    "groupLifecyclePolicies",
    "memberOf",
    "members",
    "membersWithLicenseErrors",
    "onenote",
    "owners",
    "photo",
    "photos",
    "planner",
    "rejectedSenders",
    "settings",
    "sites",
    "threads",
    "allowExternalSenders",
    "assignedLicenses",
    "autoSubscribeNewMembers",
    "hasMembersWithLicenseErrors",
    "isAssignableToRole",
    "isSubscribedByMail",
    "licenseProcessingState",
    "unseenConversationsCount",
    "unseenCount",
    "unseenMessagesCount"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "accessType": "string",
  "assignedLabels": [{"@odata.type": "microsoft.graph.assignedLabel"}],
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdByAppId": "String",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "expirationDateTime": "String (timestamp)",
  "groupTypes": ["string"],
  "hideFromAddressLists": false,
  "hideFromOutlookClients": false,
  "id": "string (identifier)",
  "isFavorite": true,
  "isAssignableRole": false,
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesDomainName": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesNetBiosName": "string",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "string",
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "resourceBehaviorOptions": ["String"],
  "resourceProvisioningOptions": ["String"],
  "securityEnabled": true,
  "securityIdentifier": "string",
  "unseenConversationsCount": 1024,
  "unseenCount": 1024,
  "unseenMessagesCount": 1024,
  "visibility": "string",
  "acceptedSenders": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "calendar": {"@odata.type": "microsoft.graph.calendar"},
  "calendarView": [{"@odata.type": "microsoft.graph.event"}],
  "conversations": [{"@odata.type": "microsoft.graph.conversation"}],
  "createdOnBehalfOf": {"@odata.type": "microsoft.graph.directoryObject"},
  "drive": {"@odata.type": "microsoft.graph.drive"},
  "events": [{"@odata.type": "microsoft.graph.event"}],
  "memberOf": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "members": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "photo": {"@odata.type": "microsoft.graph.profilePhoto"},
  "rejectedSenders": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "sites": [{"@odata.type": "microsoft.graph.site"}],
  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}],
  "classification": "string",
  "hasMembersWithLicenseErrors": true,
  "membershipRule": "string",
  "membershipRuleProcessingState": "string",
  "membershipRuleProcessingStatus":{"@odata.type": "microsoft.graph.membershipRuleProcessingStatus"},
  "preferredLanguage": "string",
  "theme": "string"
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

