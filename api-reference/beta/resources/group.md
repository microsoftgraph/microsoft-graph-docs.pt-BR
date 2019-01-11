---
title: tipo de recurso de grupo
description: Representa um grupo do Windows Azure Active Directory (AD Azure), que pode ser um grupo do Office 365, uma equipe no Microsoft Teams, um grupo dinâmico ou um grupo de segurança.
localization_priority: Priority
ms.openlocfilehash: 928eb9887665b117535bcf4fa13cf6a95b8ff283
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866889"
---
# <a name="group-resource-type"></a>tipo de recurso de grupo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um grupo do Windows Azure Active Directory (AD Azure), que pode ser um grupo do Office 365, uma equipe no Microsoft Teams, um grupo dinâmico ou um grupo de segurança.
Herda de [directoryObject](directoryobject.md).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensões](/graph/extensibility-overview).
- Assinatura de [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).

> **Grupos de Office 365 e as equipes da Microsoft oferecem suporte à colaboração de grupo**. Você pode usar a maioria dos grupos de Office 365 API com Microsoft Teams. Para criar uma [equipe](team.md), primeiro [criar o grupo](../api/group-post-groups.md) e, em seguida, [Adicionar uma equipe a ela](../api/team-put-teams.md). Para obter detalhes, consulte [Visão geral de equipes da Microsoft](teams-api-overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|**Gerenciamento de grupos**| | |
|[Criar grupo](../api/group-post-groups.md) | [group](group.md) |Crie um novo grupo, conforme especificado. Pode ser um grupo do Office 365, o grupo dinâmico, o grupo de segurança ou a equipe.|
|[Obter grupo](../api/group-get.md) | [group](group.md) |As propriedades de leitura e relações do objeto de grupo.|
|[Atualizar grupo](../api/group-update.md) | Nenhum |Atualizar as propriedades de um objeto group. |
|[Excluir grupo](../api/group-delete.md) | Nenhum |Excluir um objeto group. |
|[delta](../api/group-delta.md)|Coleção group| Obter alterações incrementais para grupos. |
|[Listar groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md) |Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)| Listar políticas de ciclo de vida de grupo. |
|[Listar proprietários](../api/group-list-owners.md) |Coleção [directoryObject](directoryobject.md)| Obter os proprietários do grupo da propriedade de navegação **owners**.|
|[Adicionar proprietário](../api/group-post-owners.md) |[directoryObject](directoryobject.md)| Adicionar um novo proprietário para o grupo postando na propriedade de navegação **owners** (com suporte somente para grupos de segurança e grupos de segurança habilitados para email).|
|[Remover proprietário](../api/group-delete-owners.md) | Nenhum |Remover um proprietário de um grupo do Office 365, grupo de segurança ou grupo de segurança habilitado para email por meio da propriedade de navegação **owners**.|
|[Listar membros](../api/group-list-members.md) |Coleção [directoryObject](directoryobject.md)| Obter os usuários e grupos que são membros diretos desse grupo da propriedade de navegação **members**.|
|[Membros da lista transitivos](../api/group-list-transitivemembers.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários, grupos, dispositivos e entidades de serviço que são membros, incluindo aninhados membros desse grupo.|
|[Adicionar membro](../api/group-post-members.md) |[directoryObject](directoryobject.md)| Adicionar um usuário ou grupo a esse grupo postando na propriedade de navegação **members** (com suporte somente para grupos de segurança e grupos de segurança habilitados para email).|
|[Remover membro](../api/group-delete-members.md) | None |Remover um membro de um grupo do Office 365, grupo de segurança ou grupo de segurança habilitado para email por meio da propriedade de navegação **members**. É possível remover usuários ou outros grupos. |
|[Listar memberOf](../api/group-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os grupos e unidades administrativas que esse grupo é um membro direto da propriedade membro navegação.|
|[Membro de lista transitivo](../api/group-list-transitivememberof.md) |Coleção [directoryObject](directoryobject.md)| Liste os grupos e unidades administrativas que esse usuário é um membro da. Essa operação é transitiva e inclui os grupos que este grupo é um membro aninhado do. |
|[checkMemberGroups](../api/group-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se a associação em uma lista de grupos. A função é transitiva.|
|[getMemberGroups](../api/group-getmembergroups.md)|Coleção de cadeias de caracteres|Retornar todos os grupos dos quais o grupo é membro. Essa função é transitiva.|
|[getMemberObjects](../api/group-getmemberobjects.md)|Coleção de cadeias de caracteres|Retorne todos os grupos e unidades administrativas que o grupo é um membro de. A função é transitiva. |
|[Criar configuração](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Crie um objeto de configuração com base em um directorySettingTemplate. A solicitação POST deve fornecer settingValues para todas as configurações definidas no modelo. Somente os modelos específicos de grupos podem ser usados para essa operação.|
|[Obter configuração](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Ler propriedades de um objeto de configuração específico.|
|[Listar configurações](../api/directorysetting-list.md) | coleção [directorySetting](directorysetting.md) |Lista propriedades de todos os objetos de configuração.|
|[Atualizar configuração](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Atualizar um objeto setting. |
|[Excluir configuração](../api/directorysetting-delete.md) | None |Excluir um objeto de configuração. |
|[Lista de pontos de extremidade](../api/group-list-endpoints.md) |coleção de [ponto de extremidade](endpoint.md)| Obtenha uma coleção de objetos de ponto de extremidade. |
|[Obtenha o ponto de extremidade](../api/endpoint-get.md) | [ponto de extremidade](endpoint.md) | Leia as propriedades e os relacionamentos de um objeto de ponto de extremidade. |
|[delta](../api/group-delta.md)|Coleção group| Obter alterações incrementais para grupos. |
|[validateProperties](../api/group-validateproperties.md)|JSON| Validar o nome de exibição de um grupo Office 365 ou apelido de email está em conformidade com as políticas de nomenclatura. | 
|**Calendário**| | |
|[Criar evento](../api/group-post-events.md) |[event](event.md)| Criar um novo Event postando na coleção de eventos.|
|[Obter evento](../api/group-get-event.md) |[event](event.md)|Ler as propriedades de um objeto event.|
|[Listar eventos](../api/group-list-events.md) |Coleção de [eventos](event.md)| Obter uma coleção de objetos de evento.|
|[Atualizar evento](../api/group-update-event.md) |Nenhum|Atualizar as propriedades de um objeto event.|
|[Excluir evento](../api/group-delete-event.md) |Nenhum|Excluir o objeto event.|
|[Listar calendarView](../api/group-list-calendarview.md) |Coleção [event](event.md)| Obter um conjunto de eventos em uma janela de tempo especificada.|
|**Conversas**| | |
|[Criar conversa](../api/group-post-conversations.md) |[conversa](conversation.md)| Crie uma nova conversa postando na coleção de conversas.|
|[Obter conversa](../api/group-get-conversation.md) |[conversation](conversation.md)| Ler as propriedades de um objeto conversation.|
|[Listar conversas](../api/group-list-conversations.md) |Coleção [conversation](conversation.md)| Obter uma coleção de objetos Conversation.|
|[Excluir conversa](../api/group-delete-conversation.md) |Nenhum|Excluir objeto conversation.|
|[Acessar thread](../api/group-get-thread.md) |[conversationThread](conversationthread.md)| Ler as propriedades de um objeto thread.|
|[Listar threads](../api/group-list-threads.md) |Coleção [conversationThread](conversationthread.md)| Obter todos os threads de um grupo.|
|[Atualizar thread](../api/group-update-thread.md) |Nenhum| Atualizar as propriedades de um objeto thread.|
|[Excluir thread](../api/group-delete-thread.md) |Nenhum| Excluir o objeto de thread
|[Listar acceptedSenders](../api/group-list-acceptedsenders.md) |Coleção [directoryObject](directoryobject.md)| Obter uma lista de usuários ou grupos que estão na lista acceptedSenders desse grupo.|
|[Adicionar acceptedSender](../api/group-post-acceptedsenders.md) |[directoryObject](directoryobject.md)| Adicionar um Usuário ou Grupo à coleção acceptSenders.|
|[Remover acceptedSender](../api/group-delete-acceptedsenders.md) |[directoryObject](directoryobject.md)| Remover um Usuário ou Grupo da coleção acceptedSenders.|
|[Listar rejectedSenders](../api/group-list-rejectedsenders.md) |Coleção [directoryObject](directoryobject.md)| Obter uma lista de usuários ou grupos que estão na lista rejectedSenders desse grupo.|
|[Adicionar rejectedSender](../api/group-post-rejectedsenders.md) |[directoryObject](directoryobject.md)| Adicionar um novo Usuário ou Grupo à coleção rejectedSenders.|
|[Remover rejectedSender](../api/group-delete-rejectedsenders.md) |[directoryObject](directoryobject.md)| Remover um novo Usuário ou Grupo da coleção rejectedSenders.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|
|**Outros recursos de grupo**| | |
|[Listar fotos](../api/group-list-photos.md) |Coleção [profilePhoto](photo.md)| Obter um conjunto de fotos de perfil para o grupo.|
|[Listar plannerPlans](../api/plannergroup-list-plans.md) |Coleção [plannerPlan](plannerplan.md)| Obter os planos de planejador pertencentes ao grupo.|
|**Configurações do usuário**| | |
|[addFavorite](../api/group-addfavorite.md)|Nenhum|Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.|
|[removeFavorite](../api/group-removefavorite.md)|Nenhum|Remova o grupo da lista de grupos favoritos do usuário atual. Suporte apenas para grupos do Office 365.|
|[Listar memberOf](../api/group-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Obter os grupos e as unidades administrativas dos quais esse usuário é membro direto, da propriedade de navegação **memberOf**.|
|[Listar joinedTeams](../api/user-list-joinedteams.md) |Coleção [group](group.md)| Obtenha o Microsoft Teams que o usuário é um membro direto.|
|[subscribeByMail](../api/group-subscribebymail.md)|Nenhum|Defina a propriedade isSubscribedByMail como **true**. Permitir que o usuário atual receber as conversas de email. Suporte para Office 365 apenas para grupos.|
|[unsubscribeByMail](../api/group-unsubscribebymail.md)|Nenhum|Defina a propriedade isSubscribedByMail como **false**. Desabilitando o usuário atual em conversas de email de recebimento. Suporte para Office 365 apenas para grupos.|
|[resetUnseenCount](../api/group-resetunseencount.md)|None|Redefina o unseenCount como 0 das postagens que o usuário atual não observou desde sua última visita. Suporte para Office 365 apenas para grupos.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|O padrão é **false**. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.|
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que estão atribuídas ao grupo. Somente leitura.|
|autoSubscribeNewMembers|Booliano|O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email. Você pode definir essa propriedade em uma solicitação PATCH para o grupo. Não a defina na solicitação POST inicial que cria esse grupo.|
|classificação|String|Descreve uma classificação para o grupo (como impacto comercial baixo, médio ou alto). Os valores válidos para esta propriedade são definidos criando um valor de [configuração](directorysetting.md) ClassificationList com base na [definição de modelo](directorysettingtemplate.md).|
|createdDateTime|DateTimeOffset| Carimbo de data/hora da ocasião em que o grupo foi criado. Não é possível modificar o valor e ele é preenchido automaticamente quando o grupo é criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. |
|description|String|Uma descrição opcional para o grupo.|
|displayName|String|O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|groupTypes|Coleção de cadeias de caracteres| Especifica o tipo de grupo para criar. Os valores possíveis são `Unified` para criar um grupo do Office 365, ou `DynamicMembership` para grupos dinâmicos.  Para todos os outro grupo tipos, como grupos de segurança e grupos de segurança habilitado para email, não defina essa propriedade.|
|id|String|O identificador exclusivo do grupo. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|isSubscribedByMail|Booliano|O valor padrão é **true**. Indica se o usuário atual está inscrito para receber conversas de email.|
|licenseProcessingState|Cadeia de caracteres|Indica o status da atribuição de licença de grupo para todos os membros do grupo. Somente leitura. Valores possíveis: `QueuedForProcessing`, `ProcessingInProgress`, e `ProcessingComplete`.|
|Email|String|O endereço SMTP do grupo, por exemplo, "serviceadmins@contoso.onmicrosoft.com". Somente leitura. Oferece suporte a $filter.|
|mailEnabled|Boolean|Especifica se o grupo está habilitado para email. Se a propriedade **securityEnabled** também é **true**, o grupo é um grupo de segurança habilitado para email. Caso contrário, o grupo é um grupo de distribuição do Microsoft Exchange.|
|mailNickname|Cadeia de caracteres|O alias de email do grupo que é exclusivo na organização. Essa propriedade deverá ser especificada quando um grupo for criado. Oferece suporte a $filter.|
|membershipRule|Cadeia de caracteres|A regra que determina os membros desse grupo se o grupo for um grupo dinâmico (groupTypes contém `DynamicMembership`). Para obter mais informações sobre a sintaxe da regra de associação, consulte [sintaxe de regras de participação](https://azure.microsoft.com/en-us/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)|
|membershipRuleProcessingState|Cadeia de caracteres|Indica se o processamento de associação dinâmica está no ou pausado. Os valores possíveis são "Ligado" ou "Pausado"|
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o objeto foi sincronizado com o diretório local. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. Oferece suporte a $filter.|
|onPremisesProvisioningErrors|coleção [onPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante o provisionamento. |
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do grupo que foi sincronizado do local com a nuvem. Somente leitura. |
|onPremisesSyncEnabled|Booliano|**True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). Somente leitura. Oferece suporte a $filter.|
|preferredDataLocation|Cadeia de caracteres|O local de dados preferida para o grupo. Para obter mais informações, consulte [Multi-Geo OneDrive Online](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|O idioma preferencial para um grupo do Office 365. Deve seguir o código ISO 639-1; Por exemplo, "en-US".|
|proxyAddresses|Coleção de cadeias de caracteres| Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` o operador **any** é necessário para expressões de filtro propriedades de valores múltiplos. Somente leitura. Não anulável. Oferece suporte a $filter. |
|renewedDateTime|DateTimeOffset| Carimbo de data/hora da ocasião em que o grupo foi renovado pela última vez. Não é possível modificar isso diretamente e a atualização ocorre apenas por meio da [ação de renovação de serviço](../api/grouplifecyclepolicy-renewgroup.md). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|securityEnabled|Booliano|Especifica se o grupo é um grupo de segurança. Se a propriedade **mailEnabled** também é true, o grupo é um grupo de segurança habilitado para email; caso contrário, é um grupo de segurança. Deve ser **false** para grupos do Office 365. Oferece suporte a $filter.|
|tema|Cadeia de caracteres|Especifica o tema de cor de um grupo Office 365. Os valores possíveis são `Teal`, `Purple`, `Green`, `Blue`, `Pink`, `Orange` ou `Red`.|
|unseenConversationsCount|Int32|Contagem de conversas que foram entregues uma ou mais novas postagens desde a última visita do usuário conectado ao grupo. Essa propriedade é o mesmo **unseenCount**.|
|unseenCount|Int32|Contagem de conversas que foram entregues uma ou mais novas postagens desde a última visita do usuário conectado ao grupo. Essa propriedade é o mesmo **unseenConversationsCount**.|
|unseenMessagesCount|Int32|Contagem de novas postagens que foram entregues a conversas do grupo desde a última visita do usuário conectado ao grupo.|
|visibility|String| Especifica a visibilidade de um grupo do Office 365. Os valores possíveis são: `private`, `public`, ou `hiddenmembership`; os valores em branco são tratados como público.  Consulte [as opções de visibilidade de grupo](#group-visibility-options) para saber mais.<br>Visibilidade pode ser definida somente quando um grupo é criado; não é editável.<br>Visibilidade somente há suporte para grupos unificados; Não há suporte para grupos de segurança.|

### <a name="group-visibility-options"></a>Opções de visibilidade de grupo

Aqui está o que significa que cada valor de propriedade de **visibilidade** :
 
|Valor|Descrição|
|:----|-----------|
| `public` | Qualquer pessoa pode ingressar no grupo sem a necessidade de permissão do proprietário.<br>Qualquer pessoa pode ver o conteúdo do grupo.|
| `private` | Permissão do proprietário é necessária para ingressar no grupo.<br>Não membros não é possível exibir o conteúdo do grupo.|
| `hiddenmembership` | Permissão do proprietário é necessária para ingressar no grupo.<br>Não membros não é possível exibir o conteúdo do grupo.<br>Não membros não podem ver os membros do grupo.<br>Administradores (global, empresa, usuário e assistência técnica) podem exibir a associação do grupo.<br>O grupo aparece no catálogo de endereços global (GAL).|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|acceptedSenders|Coleção [directoryObject](directoryobject.md)|A lista de usuários ou grupos que têm permissão para criar eventos de calendário ou postagens nesse grupo. Se essa lista não estiver vazia, somente os usuários ou grupos listados aqui poderão fazer postagens.|
|calendário|[calendar](calendar.md)|O calendário do grupo. Somente leitura.|
|calendarView|Coleção [event](event.md)|O modo de exibição do calendário. Somente leitura.|
|conversations|Coleção [conversation](conversation.md)|As conversas do grupo.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| O usuário (ou aplicativo) que criou o grupo. OBSERVAÇÃO: Não definido se o usuário for um administrador. Somente leitura.|
|Unidade|[drive](drive.md)|Unidade de padrão do grupo. Somente leitura.|
|drives|Coleção [drive](drive.md)|Unidades do grupo. Somente leitura.|
|pontos de extremidade|Coleção de [ponto de extremidade](endpoint.md)| Pontos de extremidade para o grupo. Somente leitura. Anulável.|
|events|Coleção [event](event.md)|Eventos do grupo.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o grupo. Somente leitura. Anulável.|
|groupLifecyclePolicies|Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)|A coleção de políticas de ciclo de vida para esse grupo. Somente leitura. Anulável.|
|memberOf|Coleção [directoryObject](directoryobject.md)|Grupos e unidades administrativas que este grupo é um membro de. Métodos HTTP: Obtenha (suportado para todos os grupos). Somente leitura. Anulável.|
|membros|Coleção [directoryObject](directoryobject.md)| Usuários, contatos e grupos que são membros desse grupo. Métodos HTTP: Obtenha (suporte para todos os grupos), POST (oferece suportada aos grupos de segurança e grupos de segurança habilitados para email), DELETE (suportada somente para grupos de segurança) somente leitura. Anulável.|
|membersWithLicenseErrors|Conjunto de [usuário](user.md)|Uma lista de membros de grupo com erros de licença dessa atribuição de licença baseadas em grupos. Somente leitura.|
|onenote|[OneNote](onenote.md)| Somente leitura.|
|owners|Coleção [directoryObject](directoryobject.md)|Os proprietários do grupo. Os proprietários são um conjunto de usuários não seja o administrador que têm permissão para modificar esse objeto. Métodos HTTP: Obtenha (suporte para todos os grupos), POST (oferece suportada aos grupos de segurança e grupos de segurança habilitados para email), DELETE (suportada somente para grupos de segurança) somente leitura. Anulável.|
|Foto|[profilePhoto](profilephoto.md)| Foto de perfil do grupo. |
|fotos|Coleção [profilePhoto](profilephoto.md)| As fotos de perfil pertencentes ao grupo. Somente leitura. Anulável.|
|planejador|[plannerGroup](plannergroup.md)| Serviços Planejador seletivos disponíveis para o grupo. Somente leitura. Anulável. |
|rejectedSenders|Coleção [directoryObject](directoryobject.md)|A lista de usuários ou grupos que não têm permissão para criar eventos de calendário ou postagens nesse grupo. Anulável|
|configurações|coleção [directorySetting](directorysetting.md)| Configurações que podem controlam o comportamento desse grupo, como se os membros podem convidar usuários convidados ao grupo. Anulável.|
|sites|conjunto de [sites](site.md)|A lista de sites do SharePoint nesse grupo. Acesse o site padrão com /sites/root.|
|threads|Coleção [conversationThread](conversationthread.md)| Os threads de conversas do grupo. Anulável.|

## <a name="json-representation"></a>Representação JSON
A seguir está uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "extensions",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",    
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "accessType": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isFavorite": true,  
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": ["string"],
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "unseenConversationsCount": 1024,
  "unseenCount": 1024,
  "unseenMessagesCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
