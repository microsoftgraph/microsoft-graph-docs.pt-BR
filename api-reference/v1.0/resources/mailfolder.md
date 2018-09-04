# <a name="mailfolder-resource-type"></a>tipo de recurso mailFolder

Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de e-mail podem conter mensagens, outros itens do Outlook e pastas filho e-mails.

Esse recurso tem suporte para o uso da [consulta delta](../../../concepts/delta_query_overview.md) para acompanhar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/mailfolder_delta.md).

**Nomes conhecidos de pasta**

O Outlook cria determinadas pastas para usuários por padrão. Em vez de usar o valor correspondente de **id** da pasta, para facilitar, você pode usar os nomes conhecidos listados na tabela abaixo para acessar as pastas. Por exemplo, você pode obter a pasta Rascunhos usando seu nome conhecido com a seguinte consulta.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Os nomes conhecidos funcionam de forma independente da localidade da caixa de correio do usuário, portanto, a consulta acima sempre retorna a pasta Rascunhos, não importando como ela é chamada.

| Nome conhecido de pasta | Descrição |
|:-----------------------|:------------|
| archive | As mensagens são enviadas para a pasta arquivo morto através do recurso de arquivamento com um clique nos clientes do Outlook com suporte. **Observação:** isso não é o mesmo que o recurso de caixa de correio de arquivo morto do Exchange online. |
| clutter | As mensagens de baixa prioridade são movidas para a pasta de e-mail secundário ao usar o recurso de Email secundário. |
| conflicts | A pasta que contém itens conflitantes na caixa de correio. |
| conversationhistory | A pasta onde o Skype salva conversas de mensagens Instantâneas (se o Skype estiver configurado para isso). |
| deleteditems | A pasta para onde os itens são movidos para quando são excluídos. |
| drafts | A pasta que contém as mensagens não enviadas. |
| inbox | A pasta Caixa de Entrada. |
| junkemail | A pasta de lixo eletrônico. |
| localfailures | A pasta que contém itens que existem no cliente local, mas não puderam ser carregados no servidor. |
| msgfolderroot | A pasta da "Parte superior do armazenamento de informações". Essa pasta é a pasta pai das pastas exibidas em clientes normais de e-mail, como a caixa de entrada. |
| outbox | A pasta Caixa de Saída. |
| recoverableitemsdeletions | A pasta que contém itens excluídos permanentemente: excluídos da pasta Itens excluídos ou pressionando shift + delete no Outlook. Essa pasta não é visível em nenhum cliente de e-mail do Outlook, mas os usuários finais podem interagir com ela por meio do recurso **Recuperar itens excluídos do servidor** do Outlook ou do Outlook na web. |
| scheduled | A pasta que contém mensagens agendadas para reaparecer na caixa de entrada usando o recurso de Agendamento do Outlook para iOS. |
| searchfolders | A pasta pai de todas as pastas de pesquisa definidas na caixa de correio do usuário. |
| sentitems | A pasta itens enviados. |
| serverfailures | A pasta que contém itens que existem no servidor, mas que não puderam ser sincronizados no cliente local. |
| syncissues | A pasta que contém os logs de sincronização criados pelo Outlook. |

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
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
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[mailFolder](mailFolder.md)  |Criar uma ou mais propriedades estendidas de valor único em uma mailFolder nova ou existente.   |
|[Obter mailFolder com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Obtenha mailFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [mailFolder](mailFolder.md) | Criar uma ou mais propriedades estendidas de vários valores em uma mailFolder nova ou existente.  |
|[Obter mailFolder com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [mailFolder](mailFolder.md) | Obtenha uma mailFolder que contém uma propriedade estendida com vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|childFolderCount|Int32|O número de mailFolders filho imediatas na mailFolder atual.|
|displayName|Cadeia de caracteres|O nome de exibição da mailFolder.|
|id|Sequência de caracteres|O Identificador exclusivo de mailFolder.|
|parentFolderId|Sequência de caracteres|O identificador exclusivo de mailFolder do mailFolder pai.|
|totalItemCount|Int32|O número de itens na mailFolder.|
|unreadItemCount|Int32|O número de itens na mailFolder marcados como não lidos.|

**Acessar contagens de itens de forma eficiente**

As propriedades `TotalItemCount` e `UnreadItemCount` de uma pasta permitem que você calcule convenientemente o número de itens lidos na pasta.
Eles permitem que você evite consultas como as seguintes, que podem incorrer em latência significativa:

```http
https://outlook.office.com/api/v1.0/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Pastas de e-mail no Outlook podem conter mais de um tipo de item, por exemplo, a Caixa de entrada pode conter itens de solicitação de reunião que são distintos dos itens de e-mail. `TotalItemCount` e `UnreadItemCount` incluem itens em uma pasta de e-mail, independentemente de seus tipos de item.

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:-------------|:-----|:------------|
|childFolders|Coleção [MailFolder](mailfolder.md)|A coleção de pastas filho na mailFolder.|
|messageRules | Coleção [messageRule](messagerule.md) | A coleção de regras que se aplicam à pasta da Caixa de Entrada do usuário. |
|mensagens|Coleção [Message](message.md)|A coleção de mensagens na mailFolder.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mailFolder",
  "@odata.annotations": [
    {
      "property": "childFolders",
      "capabilities": {
        "changeTracking": false,
        "navigability": "single",
        "searchable": false
      }
    },
    {
      "property": "messageRules",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": true,
        "navigability": "single"
      }
    }
  ]
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
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
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
