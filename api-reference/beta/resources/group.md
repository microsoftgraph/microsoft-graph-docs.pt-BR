---
title: tipo de recurso de grupo
description: Representa um grupo do Diretório Ativo do Azure (Azure AD), que pode ser um grupo do Microsoft 365, uma equipe do Microsoft Teams ou um grupo de segurança.
ms.localizationpriority: high
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 51ccf93866153b088d9c2b9170ee38dd0217e35d
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201453"
---
# <a name="group-resource-type"></a>tipo de recurso de grupo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo do Diretório Ativo do Azure (Azure AD), que pode ser um grupo do Microsoft 365, uma equipe do Microsoft Teams ou um grupo de segurança. Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas.

Herda de [directoryObject](directoryobject.md).

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
| [Adicionar membros](../api/group-post-members.md) | [directoryObject](directoryobject.md) | Adicione um usuário ou grupo a este grupo postando na propriedade de navegação **membros** (com suporte para grupos de segurança e grupos do Microsoft 365 apenas). |
| [Adicionar proprietários](../api/group-post-owners.md) | [directoryObject](directoryobject.md) | Adicione um novo proprietário para o grupo postando na propriedade de navegação dos **proprietários** (com suporte para grupos de segurança e grupos do Microsoft 365 apenas). |
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
| [Remover proprietário](../api/group-delete-owners.md) | Nenhum | Remova um proprietário de um grupo do Microsoft 365 ou de um grupo de segurança por meio da propriedade de navegação **proprietários**. |
| [Remover membro](../api/group-delete-members.md) | Nenhum | Remova um membro de um grupo do Microsoft 365 ou de um grupo de segurança por meio da propriedade de navegação **membros**. |
| [Atualizar configuração](../api/directorysetting-update.md) | [directorySetting](directorysetting.md) | Atualizar um objeto setting. |
| [assignLicense](../api/group-assignlicense.md) | [group](group.md) | Adicione ou remova inscrições para o grupo. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura. |
| [evaluateDynamicMembership](../api/group-evaluatedynamicmembership.md) | [evaluateDynamicMembershipResult](evaluatedynamicmembershipresult.md) | Avaliar se um usuário ou dispositivo é ou seria membro de um grupo dinâmico. |
| [renovar](../api/group-renew.md) | Booleano | Renova a expiração de um grupo. Quando um grupo é renovado, a expiração do grupo é estendida pelo número de dias definido na política. |
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
| **Objetos de diretório** |||
| [Listar grupos excluídos](../api/directory-deleteditems-list.md) | Coleção [directoryObject](directoryobject.md) | Recupere os grupos excluídos no locatário nos últimos 30 dias. |
| [Listar grupos excluídos pertencentes ao usuário](../api/directory-deleteditems-user-owned.md) | Coleção [directoryObject](directoryobject.md) | Recupere os grupos excluídos no locatário nos últimos 30 dias e que pertencem a um usuário. |
| [Obter grupo excluído](../api/directory-deleteditems-get.md) | Coleção [directoryObject](directoryobject.md) | Recupere um grupo excluído por ID. |
| [Restaurar grupo excluído](../api/directory-deleteditems-delete.md) | Coleção [directoryObject](directoryobject.md) | Restaure um grupo excluído no locatário nos últimos 30 dias. |
| [Excluir permanentemente um grupo](../api/directory-deleteditems-restore.md) | Coleção [directoryObject](directoryobject.md) | Exclua permanentemente um grupo excluído do locatário. |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | Coleção de cadeias de caracteres | Verificar associação em uma lista de grupos. Essa função é transitiva. |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | Coleção de cadeias de caracteres | Retornar todos os grupos dos quais o grupo é membro. Essa função é transitiva. |
| [checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | Coleção de cadeias de caracteres | Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa. A função é transitiva. |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md) | Coleção de cadeias de caracteres | Retornar todas as unidades administrativas e grupos dos quais o grupo é membro. Essa função é transitiva. |
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
| [subscribeByMail](../api/group-subscribebymail.md) | Nenhum | Defina a propriedade isSubscribedByMail como `true`. Permitindo que o usuário conectado receba conversas por email. Compatível apenas para grupos do Microsoft 365. |
| [unsubscribeByMail](../api/group-unsubscribebymail.md) | Nenhum | Defina a propriedade isSubscribedByMail como `false`. Desabilitando o usuário conectado de receber conversas de email. Compatível apenas para grupos do Microsoft 365. |
| [resetUnseenCount](../api/group-resetunseencount.md) | Nenhum | Redefinir a Contagem Não Vista para 0 de todas as postagens que o usuário que se inscreveu não viu desde sua última visita. Somente grupos do Microsoft 365 com suporte. |

## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries#group-properties).

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean| Indica se as pessoas externas à organização podem enviar mensagens para o grupo. O valor padrão é `false`. <br><br>Retornado somente em `$select`. Compatível apenas com a API Obter grupo (`GET /groups/{ID}`). |
|assignedLabels|coleção [assignedLabel](assignedlabel.md)|Lista de pares de rótulos de confidencialidade (ID do rótulo, nome do rótulo) associados a um grupo do Microsoft 365. <br><br>Retornado apenas em `$select`.|
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao grupo. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`). Somente leitura.|
|autoSubscribeNewMembers|Boolean|Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email. Você pode definir essa propriedade em uma solicitação PATCH para o grupo. Não a defina na solicitação POST inicial que cria esse grupo. O valor padrão é `false`. <br><br>Retornado somente em `$select`. Com suporte apenas para a API Get group (`GET /groups/{ID}`).|
|classificação|String|Descreve uma classificação para o grupo (como impacto comercial baixo, médio ou alto). Os valores válidos para esta propriedade são definidos criando um valor de [configuração](directorysetting.md) ClassificationList com base na [definição de modelo](directorysettingtemplate.md).<br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`).|
|createdByAppId|Cadeia de caracteres|ID do aplicativo usado para criar o grupo. Pode ser nulo para alguns grupos. <br><br>Retornado por padrão. Somente leitura. Suporta `$filter` (`eq`, `ne`, `not`, `in`, `startsWith`).|
|createdDateTime|DateTimeOffset| Carimbo de data/hora da ocasião em que o grupo foi criado. Não é possível modificar o valor e ele é preenchido automaticamente quando o grupo é criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). Somente leitura. |
|deletedDateTime|DateTimeOffset| Para alguns objetos do Azure Active Directory (usuário, grupo, aplicativo), se o objeto for excluído, ele será primeiro excluído logicamente e essa propriedade será atualizada com a data e hora em que o objeto foi excluído. Caso contrário, esta propriedade é nula. Se o objeto for restaurado, essa propriedade será atualizada para nula. |
|description|String|Uma descrição opcional para o grupo. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`) e `$search`.|
|displayName|Cadeia de caracteres|O nome de exibição do grupo. Obrigatório.<br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores), `$search`, e `$orderBy`.|
|expirationDateTime|DateTimeOffset| Data e hora de quando o grupo está configurado para expirar. Não é possível modificar o valor e ele é preenchido automaticamente quando o grupo é criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). Somente leitura. |
|groupTypes|Coleção de cadeias de caracteres| Especifica o tipo de grupo e sua associação.  <br><br>Se a coleção contiver `Unified`, o grupo será Microsoft 365 grupo; caso contrário, é um grupo de segurança ou grupo de distribuição. Para obter detalhes, consulte [visão geral dos grupos](groups-overview.md).<br><br>Se a coleção inclui `DynamicMembership`, o grupo tem associação dinâmica; caso contrário, a associação é estática.  <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `not`).|
|hasMembersWithLicenseErrors|Boolean| Indica se existem membros neste grupo com erros de licença da sua atribuição de licença baseada em grupo. <br><br>Essa propriedade nunca é retornada em uma operação GET. Você pode usá-lo como um $filter para obter grupos que têm membros com erros de licença (ou seja, filtrar essa propriedade sendo `true`).  <br><br>Suporta `$filter` (`eq`).|
|hideFromAddressLists |Booliano |`true` se o grupo não for exibido em determinadas partes da interface do usuário do Outlook: no **Catálogo de Endereços**, em listas de endereços para selecionar destinatários de mensagens e na caixa de diálogo **Procurar grupos** para pesquisar grupos; caso contrário, false. O valor padrão é `false`. <br><br>Retornado somente em `$select`. Compatível apenas com a API Obter grupo (`GET /groups/{ID}`).|
|hideFromOutlookClients |Booliano |`true` se o grupo não for exibido em clientes do Outlook, como Outlook para Windows e Outlook na Web, caso contrário, false. O valor padrão é `false`. <br><br>Retornado somente em `$select`. Compatível apenas com a API Obter grupo (`GET /groups/{ID}`).|
|id|String|O identificador exclusivo do grupo. <br><br>Retornado por padrão. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. <br><br>Suporta `$filter` (`eq`, `ne`, `not`, `in`).|
|isAssignableToRole|Booliano|Indica se este grupo pode ser atribuído a uma função do Azure Active Directory. Opcional.<br><br>Esta propriedade só pode ser definida durante a criação do grupo e é imutável. Se definida como `true`, a propriedade **securityEnabled** também deverá ser definida como `true` e o grupo não poderá ser um grupo dinâmico (ou seja, **groupTypes** não pode conter `DynamicMembership`). Somente chamadores em funções de Administrador global e de Administrador de funções com privilégios podem definir essa propriedade. O chamador deve receber a permissão *RoleManagement.ReadWrite.Directory* para definir essa propriedade ou atualizar a associação desses grupos. Para obter mais informações, confira [Usando um grupo para gerenciar atribuições de função do Azure Active Directory](https://go.microsoft.com/fwlink/?linkid=2103037)<br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`).|
|infoCatalogs|Conjunto de cadeias de caracteres|Identifica os segmentos de informações atribuídos ao grupo. Retornado por padrão. Dá suporte `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|isSubscribedByMail|Boolean|Indica se o usuário conectado está inscrito para receber conversas por email. O valor padrão é `true`.<br><br>Retornado somente em `$select`. Com suporte apenas para a API Get group (`GET /groups/{ID}`). |
|licenseProcessingState|String|Indica o status da atribuição de licença de grupo a todos os membros do grupo. Valores possíveis: `QueuedForProcessing`, `ProcessingInProgress`e `ProcessingComplete`. <br><br>Retornado apenas em `$select`. Somente leitura. |
|email|String|O endereço SMTP do grupo, por exemplo, "serviceadmins@contoso.onmicrosoft.com". <br><br>Retornado por padrão. Somente leitura. Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores).|
|mailEnabled|Boolean|Especifica se o grupo está habilitado para email. Obrigatório.<br><br>Devolvido por padrão. Suporte `$filter` (`eq`, `ne`, `not`, e `eq` no `null` valores).|
|mailNickname|String|O alias de email do grupo, exclusivo para grupos do Microsoft 365 na organização. O comprimento máximo é de 64 caracteres. Essa propriedade pode conter apenas caracteres no [conjunto de caracteres ASCII de 0 a 127](/office/vba/language/reference/user-interface-help/character-set-0127), exceto o seguinte: ` @ () \ [] " ; : . <> , SPACE`. <br><br>Devolvido por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`).|
|membershipRule|String|A regra que determina membros para esse grupo se o grupo for um grupo dinâmico (groupTypes contém `DynamicMembership`). Para saber mais sobre a sintaxe da regra de associação, confira [sintaxe regras de associação](/azure/active-directory/enterprise-users/groups-dynamic-membership). <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `startsWith`). |
|membershipRuleProcessingState|String|Indica se o processamento de associação dinâmica está ativado ou em pausa. Os valores possíveis são `On` ou `Paused`. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `in`). |
|membershipRuleProcessingStatus|[membershipRuleProcessingStatus](membershipruleprocessingstatus.md) |Descreve o status de processamento para grupos dinâmicos baseados em regras. A propriedade é `null` para grupos dinâmicos não baseados em regras ou se o processamento do grupo dinâmico foi pausado. <br><br>Retornado somente no `$select`. Compatível apenas com a API obter grupo (`GET /groups/{ID}`). Somente leitura. |
|onPremisesDomainName|String|Contém o **FQDN de domínio** local, também chamado **dnsDomainName** sincronizado do diretório local. A propriedade só é populada para clientes que estão sincronizando seu diretório local para Azure Active Directory via Azure AD Connect.<br><br>Retornado por padrão. Somente leitura. |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o grupo foi sincronizado com o diretório local. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado por padrão. Somente leitura. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`).|
|onPremisesNetBiosName|Cadeia de Caracteres|Contém o nome **netBios** sincronizado do diretório local. A propriedade só é populada para clientes que estão sincronizando seu diretório local para Azure Active Directory via Azure AD Connect.<br><br>Retornado por padrão. Somente leitura. |
|onPremisesProvisioningErrors|coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante a configuração. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `not`). |
|onPremisesSamAccountName|String|Contém o nome **da conta SAM** sincronizado do diretório local. A propriedade só é populada para clientes que estão sincronizando seu diretório local para Azure Active Directory via Azure AD Connect.<br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`). Somente leitura. |
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do grupo que foi sincronizado do local com a nuvem. <br><br>Retornado por padrão. Suporta `$filter` em `null` valores. Somente leitura. |
|onPremisesSyncEnabled|Booliano|`true` se esse grupo está sincronizado de um diretório local; `false` se esse grupo foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). <br><br>Retornado por padrão. Somente leitura. Suporte `$filter` (`eq`, `ne`, `not`, `in`, e `eq` no `null` valores). |
|preferredDataLocation|String|O local de data preferido para o grupo do Microsoft 365. Por padrão, o grupo herda o local de dados preferencial do criador do grupo. Para definir essa propriedade, o usuário de chamada deve ter uma das seguintes [funções do Azure AD](/azure/active-directory/roles/permissions-reference): <br><ul><li> Administrador Global <li> Administrador de Conta de Usuário <li>Escritor de Diretórios <li> Administrador do Exchange <li> Administrador do SharePoint </ul><br/> Para obter mais informações sobre essa propriedade, consulte [OneDrive Online Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction). <br><br>Anulável. Retornado por padrão.|
|preferredLanguage|Cadeia de caracteres|O idioma preferencial para um Microsoft 365 grupo. Deve seguir o código ISO 639-1; por exemplo, `en-US`. <br><br>Retornado por padrão. Suporte `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` no `null` valores). |
|proxyAddresses|String collection| Endereços de email para o grupo que direcionam para a mesma caixa de correio do grupo. Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. <br><br>Retornado por padrão. Somente leitura. Não anulável. Suporta `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`). |
|renewedDateTime|DateTimeOffset| Carimbo de data/hora da ocasião em que o grupo foi renovado pela última vez. Não é possível modificar isso diretamente e a atualização ocorre apenas por meio da [ação de renovação de serviço](../api/grouplifecyclepolicy-renewgroup.md). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). Apenas leitura.|
|resourceBehaviorOptions|Conjunto de cadeias de caracteres|Especifica os comportamentos de grupo que podem ser configurados para um grupo do Microsoft 365 durante sua criação. Isso só pode ser definido como parte da criação (POST). Os valores possíveis são `AllowOnlyMembersToPost`, `HideGroupInOutlook`, `SubscribeNewGroupMembers`, `WelcomeEmailDisabled`. Para obter mais informações, confira o artigo [Definir as opções de provisionamento e comportamentos de grupo do Microsoft 365 ](/graph/group-set-options).|
|resourceProvisioningOptions|Conjunto de cadeias de caracteres|Especifica os recursos de grupo provisionados como parte da criação de grupos do Microsoft 365 que não costumam fazer parte do processo padrão de criação de grupos. Um valor possível é `Team`. Para obter mais informações, confira o artigo [Definir as opções de provisionamento e comportamentos de grupo do Microsoft 365 ](/graph/group-set-options). <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `not`, `startsWith`.|
|securityEnabled|Boolean|Especifica se o grupo é um grupo de segurança. Obrigatório.<br><br>Retornado por padrão. Dá suporte `$filter` (`eq`, `ne`, `not`, `in`).|
|securityIdentifier|Cadeia de Caracteres|Identificador de segurança do grupo, usado em cenários do Windows. <br><br>Retornado por padrão.|
|tema|Cadeia de caracteres|Especifica o tema de cor de um grupo do Microsoft 365. Os valores possíveis são: `Teal`, `Purple`, `Green`, `Blue`,`Pink`, `Orange` ou `Red`. <br><br>Retornado por padrão. |
|unseenConversationsCount|Int32|Contagem de conversas que foram entregues em uma ou mais postagens novas desde a última visita do usuário conectado ao grupo. Essa propriedade é a mesma que **unseenCount**. <br><br>Retornado apenas em `$select`.|
|unseenCount|Int32|Contagem de conversas que receberam novas postagens desde que o usuário conectado visitou o grupo pela última vez. Essa propriedade é a mesma que **unseenConversationsCount**.<br><br>Retornado somente em `$select`. Compatível apenas com a API Obter grupo (`GET /groups/{ID}`). |
|unseenMessagesCount|Int32|Contagem de novas postagens que foram entregues às conversas do grupo desde a última visita do usuário conectado ao grupo. <br><br>Retornado apenas em `$select`.|
|visibility|Cadeia de caracteres| Especifica a política de associação ao grupo e a visibilidade do conteúdo do grupo para grupos. Os valores possíveis são: `Private`, `Public` ou `Hiddenmembership`. `Hiddenmembership` pode ser definido apenas para grupos do Microsoft 365, quando os grupos são criados. Não pode ser atualizado posteriormente. Outros valores de visibilidade podem ser atualizados após a criação do grupo.<br> Se o valor de visibilidade não for especificado durante a criação do grupo no Microsoft Graph, um grupo de segurança é criado como `Private` por padrão e o grupo Microsoft 365 é `Public`.  Grupos atribuídos a funções são sempre `Private`. Saiba mais em [Opções de visibilidade do grupo](#group-visibility-options). <br><br>Retornado por padrão. Anulável.|

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
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Representa as funções de aplicativo que um grupo recebeu para um aplicativo. Dá suporte `$expand`. |
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
|memberOf|Coleção [directoryObject](directoryobject.md)|Grupos e unidades administrativas dos qual esse grupo é membro. Métodos HTTP: GET (com suporte para todos os grupos). Somente leitura. Anulável. Dá suporte `$expand`.|
|members|Coleção [directoryObject](directoryobject.md)| Membros desse grupo, que podem ser usuários, dispositivos, outros grupos ou entidades de serviço. Suporta as operações [Membros da lista](../api/group-list-members.md), [Adicionar membro](../api/group-post-members.md) e [Remover membro](../api/group-delete-members.md). Anulável. <br/>Suporta `$expand` incluindo `$select` aninhado. Por exemplo, `/groups?$filter=startsWith(displayName,'Role')&$select=id,displayName&$expand=members($select=id,userPrincipalName,displayName)`.|
|membersWithLicenseErrors|Coleção [usuário](user.md)|Uma lista de membros do grupo com erros de licença desta atribuição de licença baseada em grupo. Somente leitura.|
|onenote|[onenote](onenote.md)| Somente leitura.|
|owners|Coleção [directoryObject](directoryobject.md)|Os proprietários do grupo que podem ser usuários ou entidades de serviço.  Anulável. Se essa propriedade não for especificada ao criar um grupo Microsoft 365, o usuário chamador será atribuído automaticamente como o proprietário do grupo. <br/>Suporta `$expand` incluindo `$select` aninhado. Por exemplo, `/groups?$filter=startsWith(displayName,'Role')&$select=id,displayName&$expand=owners($select=id,userPrincipalName,displayName)`.|
|permissionGrants|[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)|As permissões que foram concedidas a um grupo para um aplicativo específico. Suporta `$expand`.|
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
  "accessType": "String",
  "assignedLabels": [{"@odata.type": "microsoft.graph.assignedLabel"}],
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdByAppId": "String",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "expirationDateTime": "String (timestamp)",
  "groupTypes": ["String"],
  "hideFromAddressLists": false,
  "hideFromOutlookClients": false,
  "id": "String (identifier)",
  "isFavorite": true,
  "isAssignableRole": false,
  "isSubscribedByMail": true,
  "licenseProcessingState": "String",
  "mail": "String",
  "mailEnabled": true,
  "mailNickname": "String",
  "onPremisesDomainName": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesNetBiosName": "String",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "String",
  "proxyAddresses": ["String"],
  "renewedDateTime": "String (timestamp)",
  "resourceBehaviorOptions": ["String"],
  "resourceProvisioningOptions": ["String"],
  "securityEnabled": true,
  "securityIdentifier": "String",
  "unseenConversationsCount": 1024,
  "unseenCount": 1024,
  "unseenMessagesCount": 1024,
  "visibility": "String",
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
  "classification": "String",
  "hasMembersWithLicenseErrors": true,
  "membershipRule": "String",
  "membershipRuleProcessingState": "String",
  "membershipRuleProcessingStatus":{"@odata.type": "microsoft.graph.membershipRuleProcessingStatus"},
  "preferredLanguage": "String",
  "theme": "String"
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