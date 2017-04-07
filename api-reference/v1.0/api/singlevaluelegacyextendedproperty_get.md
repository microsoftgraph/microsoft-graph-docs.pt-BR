# <a name="get-singlevaluelegacyextendedproperty"></a>Obter singleValueLegacyExtendedProperty

Obtenha instâncias de recursos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`.

Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada. Atualmente, esta é a única maneira de obter o objeto [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) que representa uma propriedade estendida.

Usar o parâmetro de consulta `$filter` permite obter todas as instâncias do recurso especificado que têm uma correspondência estendida correspondente a um filtro nas propriedades **id** e **value**. O filtro é aplicado a todas as instâncias do recurso na caixa de correio do usuário conectado.

Há suporte para as seguintes fontes de dados:

- [message](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [event](../resources/event.md)
- [calendar](../resources/calendar.md)
- [contact](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md) 

Também há suporte para os seguintes recursos de grupo:

- grupo [event](../resources/event.md)
- grupo [calendar](../resources/calendar.md)
- grupo [post](../resources/post.md) 

Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.

## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes valores de **scopes** é obrigatório para executar essa API, dependendo do recurso que você está obtendo:

- _Mail.Read_
- _Calendars.Read_
- _Contacts.Read_
- _Group.Read.All_ 

## <a name="http-request"></a>Solicitação HTTP

#### <a name="get-a-resource-instance-using-expand"></a>OBTER uma instância de recurso usando `$expand`
Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Certifique-se de aplicar a [codificação de URL](http://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.

Obtenha uma instância de **message**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Obtenha uma instância de **mailFolder**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Obtenha uma instância de **event**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Obtenha uma instância de **calendar**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Obtenha uma instância de **contact**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Obtenha uma instância de **contactFolder**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
Obtenha uma instância de **group event**:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

Obtenha uma instância de **group post**:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a>OBTER instâncias de recursos usando `$filter`

Obtenha instâncias de um recurso com suporte que tenham a propriedade estendida correspondente a um filtro nas propriedades **id** e **value**. Certifique-se de aplicar a [codificação de URL](http://www.w3schools.com/tags/ref_urlencode.asp) aos seguintes caracteres na cadeia de filtro - barra e espaço.


Obtenha instâncias de **message**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Obtenha instâncias de **mailFolder**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Obtenha instâncias de **event**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Obtenha instâncias de **calendar**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Obtenha instâncias de **contact**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Obtenha instâncias de **contactFolder**:
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
Obtenha instâncias de **group event**:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

Obtenha instâncias de **group post**:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a>Parâmetros
|**Parâmetro**|**Tipo**|**Descrição**|
|:-----|:-----|:-----|
|_Parâmetros de URL_|
|id_value|String|A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.|
|property_value|String|O valor da propriedade estendida a ser correspondida. Obrigatório onde listado na seção **Solicitação HTTP** acima.|

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | <code> de portador|


## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se bem-sucedido, esse método retornará um código de resposta `200 OK`.

#### <a name="get-resource-instance-using-expand"></a>OBTER instância de recurso usando `$expand`
O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) correspondente.
  
#### <a name="get-resource-instances-using-filter"></a>OBTER instâncias de recursos usando `$filter`
O corpo da resposta inclui um ou mais objetos que representam as instâncias de recursos contendo a propriedade estendida correspondente. O corpo da resposta não inclui a propriedade estendida.

## <a name="example"></a>Exemplo
#### <a name="request-1"></a>Solicitação 1

O primeiro exemplo obtém e expande a mensagem especificada, incluindo uma propriedade estendida de valor único. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação removida aqui para facilitar a leitura).

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
##### <a name="response-1"></a>Resposta 1
O corpo da resposta inclui todas as propriedades da mensagem especificada e a propriedade estendida retornada do filtro.

Observação: O objeto **message** mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

****

#### <a name="request-2"></a>Solicitação 2

O segundo exemplo obtém mensagens que possuem a propriedade estendida de valor único especificada no filtro. O filtro retorna a propriedade estendida cujo valor de:
- **id** corresponde à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação removida aqui para facilitar a leitura).
- **value** é igual a `Green`.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/api/v1.0/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

##### <a name="response-2"></a>Resposta 2

Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK`, e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro. O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user_list_messages.md). A resposta não inclui a propriedade estendida correspondente.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->