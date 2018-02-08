# <a name="mailfolder-resource-type"></a>tipo de recurso mailFolder

Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.

O Outlook cria determinadas pastas para usuários por padrão. Em vez de usar o valor **id** da pasta correspondente, para mais praticidade, é possível usar os seguintes nomes de pasta comuns ao acessar essas pastas em um conjunto de **mailFolder**: `ArchiveRoot`, `ConversationHistory`, `DeletedItems`, `Drafts`, `Inbox`, `JunkEmail`, `Outbox` e `SentItems`.

Esse recurso tem suporte para o uso da [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/mailfolder_delta.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter mailFolder](../api/mailfolder_get.md) | [mailFolder](mailfolder.md) |Leia as propriedades e os relacionamentos do objeto mailFolder.|
|[Criar MailFolder](../api/mailfolder_post_childfolders.md) |[MailFolder](mailfolder.md)| Crie uma nova mailFolder na atual postando na coleção childFolders.|
|[Listar childFolders](../api/mailfolder_list_childfolders.md) |Coleção [MailFolder](mailfolder.md)| Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.|
|[Criar Mensagem](../api/mailfolder_post_messages.md) |[Mensagem](message.md)| Crie uma nova mensagem na mailFolder atual postando na coleção de mensagens.|
|[Listar mensagens](../api/mailfolder_list_messages.md) |Coleção [Message](message.md)| Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.|
|[Update](../api/mailfolder_update.md) | [mailFolder](mailfolder.md)|Atualize o objeto mailFolder especificado. |
|[Delete](../api/mailfolder_delete.md) | Nenhuma |Exclua o objeto mailFolder especificado. |
|[copy](../api/mailfolder_copy.md)|[MailFolder](mailfolder.md)|Copie uma mailFolder e seu conteúdo para outra mailFolder.|
|[delta](../api/mailfolder_delta.md)|Coleção [mailFolder](mailfolder.md)|Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.|
|[move](../api/mailfolder_move.md)|[MailFolder](mailfolder.md)|Mova uma mailFolder e seu conteúdo para outra mailFolder.|
|[Criar propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |Criar uma ou mais propriedades estendidas de valor único em uma mailFolder nova ou existente.   |
|[Obter mailFolder com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Obtenha mailFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | Criar uma ou mais propriedades estendidas de vários valores em uma mailFolder nova ou existente.  |
|[Obter mailFolder com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Obtenha uma mailFolder que contém uma propriedade estendida com vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|childFolderCount|Int32|O número de mailFolders filho imediatas na mailFolder atual.|
|displayName|String|O nome de exibição da mailFolder.|
|id|String|Identificador exclusivo de mailFolder. Você pode usar os seguintes nomes conhecidos para acessar a pasta correspondente: Caixa de Entrada, Rascunhos, Itens Enviados, DeletedItems.|
|parentFolderId|String|O identificador exclusivo de mailFolder do mailFolder pai.|
|totalItemCount|Int32|O número de itens na mailFolder.|
|unreadItemCount|Int32|O número de itens na mailFolder marcados como não lidos.|

**Acessar contagens de itens de forma eficiente**

As propriedades TotalItemCount e UnreadItemCount de uma pasta permitem que você calcule convenientemente o número de itens lidos na pasta. Eles permitem que você evite consultas semelhante à seguinte, que podem causar latência significativa:
```
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```
MailFolders no Outlook podem conter mais de um tipo de itens. Por exemplo, a caixa de entrada pode conter itens de solicitação de reunião que são diferentes dos itens de email. TotalItemCount e UnreadItemCount incluem itens em uma mailFolder independentemente de seus tipos de item.


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|childFolders|Coleção [MailFolder](mailfolder.md)|A coleção de pastas filho na mailFolder.|
|mensagens|Coleção [Message](message.md)|A coleção de mensagens na mailFolder.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,

  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](../../../concepts/delta_query_overview.md)
- [Obter as alterações incrementais para as mensagens em uma pasta](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
