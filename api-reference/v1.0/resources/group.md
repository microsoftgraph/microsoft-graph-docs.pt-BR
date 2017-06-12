# <a name="group-resource-type"></a>tipo de recurso de grupo

Representa um grupo do Azure Active Directory, que pode ser um grupo do Office 365, um grupo dinâmico ou um grupo de segurança. Herda de [directoryObject](directoryobject.md).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).
- Usar a [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user_delta.md).

> **O Microsoft Teams tem como base grupos do Office 365**. Você pode usar a maior parte das APIs de grupos com o Microsoft Teams. Não é possível usar [Criar grupo](../api/group_post_groups.md) para criar uma equipe. Para obter detalhes, confira a [referência do Microsoft Teams](teams_api_overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar grupo](../api/group_post_groups.md) | [group](group.md) |Criar um novo grupo. Pode ser um grupo do Office 365, um grupo dinâmico ou um grupo de segurança.|
|[Obter grupo](../api/group_get.md) | [group](group.md) |Ler as propriedades de um objeto group.|
|[Listar grupos](../api/group_list.md) |Coleção [group](group.md) |Listar objetos group e suas propriedades.|
|[Atualizar grupo](../api/group_update.md) | [group](group.md) |Atualizar as propriedades de um objeto group. |
|[Excluir grupo](../api/group_delete.md) | Nenhum |Excluir um objeto group. |
|[Adicionar membro](../api/group_post_members.md) |Nenhum| Adicionar um usuário ou grupo a esse grupo postando na propriedade de navegação **members** (com suporte somente para grupos de segurança e grupos de segurança habilitados para email).|
|[Listar membros](../api/group_list_members.md) |Coleção [directoryObject](directoryobject.md)| Obter os usuários e grupos que são membros diretos desse grupo da propriedade de navegação **members**.|
|[Remover membro](../api/group_delete_members.md) | None |Remover um membro de um grupo do Office 365, grupo de segurança ou grupo de segurança habilitado para email por meio da propriedade de navegação **members**. É possível remover usuários ou outros grupos. |
|[Listar memberOf](../api/group_list_memberof.md) |Coleção [directoryObject](directoryobject.md)| Obter os grupos dos quais esse grupo é membro direto da propriedade de navegação **memberOf**.|
|[Adicionar proprietário](../api/group_post_owners.md) |[Nenhum| Adicionar um novo proprietário para o grupo postando na propriedade de navegação **owners** (com suporte somente para grupos de segurança e grupos de segurança habilitados para email).|
|[Listar proprietários](../api/group_list_owners.md) |Coleção [directoryObject](directoryobject.md)| Obter os proprietários do grupo da propriedade de navegação **owners**.|
|[Remover proprietário](../api/group_delete_owners.md) | Nenhum |Remover um proprietário de um grupo do Office 365, grupo de segurança ou grupo de segurança habilitado para email por meio da propriedade de navegação **owners**.|
|[checkMemberGroups](../api/group_checkmembergroups.md)|Coleção de cadeias de caracteres|Verificar esse grupo quanto a uma associação em uma lista de grupos. Essa função é transitiva.|
|[getMemberGroups](../api/group_getmembergroups.md)|Coleção de cadeias de caracteres|Retornar todos os grupos dos quais o grupo é membro. Essa função é transitiva.|
|[getMemberObjects](../api/group_getmemberobjects.md)|Coleção de cadeias de caracteres|Retornar todos os grupos dos quais o grupo é um membro. Essa função é transitiva. |
|[Criar evento](../api/group_post_events.md) |[Event](event.md)| Criar um novo Event postando na coleção events.|
|[Listar eventos](../api/group_list_events.md) |Coleção [Event](event.md)| Obter uma coleção de objetos Event.|
|[Listar calendarView](../api/group_list_calendarview.md) |Coleção [Event](event.md)| Obter um conjunto de eventos em uma janela de tempo especificada.|
|[Criar conversa](../api/group_post_conversations.md) |[Conversation](conversation.md)| Criar uma nova Conversation postando noa coleção conversations.|
|[Listar conversas](../api/group_list_conversations.md) |Coleção [Conversation](conversation.md)| Obter uma coleção de objetos Conversation.|
|[Lista threads](../api/group_list_threads.md) |Coleção [ConversationThread](conversationthread.md)| Obter todos os threads de um grupo.|
|[Listar acceptedSenders](../api/group_list_acceptedsenders.md) |Coleção [directoryObject](directoryobject.md)| Obter uma lista de usuários ou grupos que estão na lista acceptedSenders desse grupo.|
|[Adicionar acceptedSender](../api/group_post_acceptedsenders.md) |[directoryObject](directoryobject.md)| Adicionar um Usuário ou Grupo à coleção acceptSenders.|
|[Remover acceptedSender](../api/group_delete_acceptedsenders.md) |[directoryObject](directoryobject.md)| Remover um Usuário ou Grupo da coleção acceptedSenders.|
|[Adicionar rejectedSender](../api/group_post_rejectedsenders.md) |[directoryObject](directoryobject.md)| Adicionar um novo Usuário ou Grupo à coleção rejectedSenders.|
|[Listar rejectedSenders](../api/group_list_rejectedsenders.md) |Coleção [directoryObject](directoryobject.md)| Obter uma lista de usuários ou grupos que estão na lista rejectedSenders desse grupo.|
|[Remover rejectedSender](../api/group_delete_rejectedsenders.md) |[directoryObject](directoryobject.md)| Remover um novo Usuário ou Grupo da coleção rejectedSenders.|
|[addFavorite](../api/group_addfavorite.md)|None|Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.|
|[removeFavorite](../api/group_removefavorite.md)|Nenhum|Remover o grupo da lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.|
|[subscribeByMail](../api/group_subscribebymail.md)|None|Definir a propriedade isSubscribedByMail como **true**. Permitindo que o usuário atual receba conversas por email. Com suporte apenas para grupos do Office 365.|
|[unsubscribeByMail](../api/group_unsubscribebymail.md)|None|Definir a propriedade isSubscribedByMail como **false**. Não permitindo que o usuário atual receba conversas por email. Com suporte apenas para grupos do Office 365.|
|[resetUnseenCount](../api/group_resetunseencount.md)|None|Redefinir unseenCount como 0 para todas as postagens que o usuário atual não viu desde sua última visita. Com suporte apenas para grupos do Office 365.|
|[delta](../api/group_delta.md)|coleção de grupos| Obtenha as alterações incrementais para grupos. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](../../../concepts/extensibility_schema_groups.md) || Crie uma definição para a extensão de esquema e use-a para adicionar dados digitados personalizados a um recurso.|


## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|O padrão é **false**. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.|
|autoSubscribeNewMembers|Booliano|O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email. Você pode definir essa propriedade em uma solicitação PATCH para o grupo. Não a defina na solicitação POST inicial que cria esse grupo.|
|createdDateTime|DateTimeOffset| A data e a hora da criação do grupo. |
|description|String|Uma descrição opcional para o grupo. |
|displayName|String|O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|groupTypes|Coleção de cadeias de caracteres| Especifica o tipo de grupo a ser criado. Os valores possíveis são **Unified** para criar um grupo do Office 365 ou **DynamicMembership** para grupos dinâmicos.  Para todos os outro tipos de grupos, como grupos habilitados para segurança e grupos de segurança habilitados para email, não defina essa propriedade. Oferece suporte a $filter.|
|id|String|O identificador exclusivo do grupo. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|isSubscribedByMail|Booliano|O valor padrão é **true**. Indica se o usuário atual está inscrito para receber conversas de email.|
|Email|String|O endereço SMTP do grupo, por exemplo, "serviceadmins@contoso.onmicrosoft.com". Somente leitura. Oferece suporte a $filter.|
|mailEnabled|Booliano|Especifica se o grupo está habilitado para email. Se a propriedade **securityEnabled** também é **true**, o grupo é um grupo de segurança habilitado para email. Caso contrário, o grupo é um grupo de distribuição do Microsoft Exchange.|
|mailNickname|String|O alias de email do grupo. Essa propriedade deve ser especificada quando um grupo é criado. Oferece suporte a $filter.|
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o grupo foi sincronizado com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura. Oferece suporte a $filter.|
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do grupo que foi sincronizado do local com a nuvem. Somente leitura. |
|onPremisesSyncEnabled|Booliano|**True** se esse grupo está sincronizado de um diretório local; **false** se esse grupo foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). Somente leitura. Oferece suporte a $filter.|
|proxyAddresses|Coleção de cadeias de caracteres| O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Somente leitura. Não anulável. Oferece suporte a $filter. |
|securityEnabled|Booliano|Especifica se o grupo é um grupo de segurança. Se a propriedade **mailEnabled** também é true, o grupo é um grupo de segurança habilitado para email; caso contrário, é um grupo de segurança. Deve ser **false** para grupos do Office 365. Oferece suporte a $filter.|
|unseenCount|Int32|Contagem de postagens que o usuário atual não viu desde a última visita.|
|visibility|String| Especifica a visibilidade de um grupo do Office 365. Os valores possíveis são: **Private**, **Public** ou vazio (que é interpretado como **Public**).|

## <a name="relationships"></a>Relações
| Relação | Tipo    |Descrição|
|:---------------|:--------|:----------|
|acceptedSenders|Coleção [directoryObject](directoryobject.md)|A lista de usuários ou grupos que têm permissão para criar eventos de calendário ou postagens nesse grupo. Se essa lista não estiver vazia, somente os usuários ou grupos listados aqui poderão fazer postagens.|
|calendário|[calendar](calendar.md)|O calendário do grupo. Somente leitura.|
|calendarView|Coleção [event](event.md)|O modo de exibição do calendário. Somente leitura.|
|conversations|Coleção [conversation](conversation.md)|As conversas do grupo.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| O usuário (ou aplicativo) que criou o grupo. OBSERVAÇÃO: Não definido se o usuário for um administrador. Somente leitura.|
|Unidade|[drive](drive.md)|A unidade do grupo. Somente leitura.|
|events|Coleção [event](event.md)|Os eventos de calendário do grupo.|
|extensions|[extension](extension.md) collection|A coleção de extensões abertas definidas para o grupo. Somente leitura. Anulável.|
|memberOf|Coleção [directoryObject](directoryobject.md)|Grupos dos quais esse grupo é membro. Métodos HTTP: GET (com suporte para todos os grupos). Somente leitura. Anulável.|
|membros|Coleção [directoryObject](directoryobject.md)| Os usuários e grupos que são membros desse grupo. Métodos HTTP: GET (com suporte para todos os grupos), POST (com suporte para grupos do Office 365, grupos de segurança e grupos de segurança habilitados para email), DELETE (com suporte para grupos do Office 365 e grupos de segurança) Anulável.|
|onenote|[OneNote](onenote.md)| Somente leitura.|
|planner|[Planner](planner.md)| Ponto de entrada para o recurso Planejador que pode existir para um grupo unificado.|
|proprietários|Coleção [directoryObject](directoryobject.md)|Os proprietários do grupo. Os proprietários são um conjunto de usuários não administradores e que têm permissão para modificar esse objeto. Limitado a 10 proprietários. Métodos HTTP: GET (com suporte para todos os grupos), POST (com suporte para grupos do Office 365, grupos de segurança e grupos de segurança habilitados para email), DELETE (com suporte para grupos do Office 365 e grupos de segurança). Anulável.|
|Foto|[profilePhoto](profilephoto.md)| A foto de perfil do grupo |
|rejectedSenders|Coleção [directoryObject](directoryobject.md)|A lista de usuários ou grupos que não têm permissão para criar eventos de calendário ou postagens nesse grupo. Anulável|
|sites|conjunto de [sites](site.md)|A lista de sites do SharePoint nesse grupo. Acesse o site padrão com /sites/root.
|threads|Coleção [conversationThread](conversationthread.md)| Os threads de conversas do grupo. Anulável.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

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
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": ["string"],
  "securityEnabled": true,
  "unseenCount": 1024,
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
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

## <a name="see-also"></a>Ver também

- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
