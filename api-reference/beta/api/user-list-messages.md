---
title: Listar mensagens
description: 'Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário). '
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 24083f158863077d6dcb6b2af55a2a16db1e83e7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052611"
---
# <a name="list-messages"></a>Listar mensagens

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário). 

Dependendo do tamanho da página e dos dados da caixa de correio, a obtenção de mensagens de uma caixa de correio pode incorrer em várias solicitações. O tamanho de página padrão é 10 mensagens. Use `$top` para personalizar o tamanho da página, no intervalo de 1 a 1000.

Para melhorar o tempo de resposta da operação, use `$select` para especificar as propriedades exatas de que você precisa; consulte [exemplo 1](#example-1-list-all-messages) abaixo. Ajuste os valores para `$select` e `$top`, especialmente quando você deve usar um tamanho de página maior, pois retornar uma página com centenas de mensagens, cada uma com uma carga útil de resposta completa, pode acionar o [tempo limite do gateway](/graph/errors#http-status-codes) (HTTP 504).

Para obter a próxima página de mensagens, basta aplicar a URL inteira retornada em `@odata.nextLink` à próxima solicitação de obtenção de mensagens. Esta URL inclui todos os parâmetros de consulta que você especificou na solicitação inicial. 

Não tente extrair o valor `$skip` da URL `@odata.nextLink` para manipular respostas. Essa API usa o valor `$skip` para manter a contagem de todos os itens pelos quais passou na caixa de correio do usuário para retornar uma página de itens do tipo mensagem. Portanto, é possível que, mesmo na resposta inicial, o valor `$skip` seja maior que o tamanho da página. Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).

Você pode filtrar as mensagens e obter apenas aquelas que incluem [uma](../resources/mention.md) menção do usuário que está dentro. Veja um [exemplo](#request-2) abaixo. Por padrão, `GET /me/messages` a operação não retorna a propriedade **mentions.** Use o `$expand` parâmetro de consulta para encontrar detalhes de cada [menção em uma mensagem](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message).

Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:

* Se o aplicativo tiver permissões de aplicativo ou
* Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário. Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).

> **Observação** Lembre-se da [questão conhecida](/graph/known-issues#get-messages-returns-chats-in-microsoft-teams) essa operação inclui mensagens de chat do Microsoft Teams em sua resposta.
 
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.ReadBasic, Mail.Read, Mail.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Mail.ReadBasic, Mail.Read, Mail.ReadWrite    |
|Aplicativo | Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

Para obter todas as mensagens na caixa de correio do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

Para obter mensagens em uma pasta específica na caixa de correio do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

Para obter todas as mensagens na caixa de correio do usuário que incluem uma **menção** do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

Você pode usar `$filter` o parâmetro de consulta na propriedade **mentionsPreview** para obter as mensagens que mencionam o usuário de assinatura.

### <a name="using-filter-and-orderby-in-the-same-query"></a>Uso de filtro e orderby na mesma consulta
Ao usar `$filter` e `$orderby` na mesma consulta para obter mensagens, lembre-se de especificar as propriedades das seguintes maneiras:

1. As propriedades que aparecem em `$orderby` também devem aparecer em `$filter`. 
2. As propriedades que aparecem em `$orderby` estão na mesma ordem que em `$filter`.
3. As propriedades presentes em `$orderby` aparecem em `$filter` antes de qualquer propriedade que não esteja presente.

Ao não fazer isso, o seguinte erro surge:

- Código de erro: `InefficientFilter`
- Mensagem de erro: `The restriction or sort order is too complex for this operation.`

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Prefer: outlook.body-content-type | string | O formato das propriedades **body** e **uniqueBody** a serem retornadas. Os valores podem ser "text" ou "html". Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML. Opcional. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [de](../resources/message.md) mensagem no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="example-1-list-all-messages"></a>Exemplo 1: Listar todas as mensagens
#### <a name="request"></a>Solicitação
O primeiro exemplo obtém as 10 principais mensagens padrão na caixa de correio do usuário de entrada. Ele usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta. 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=sender,subject
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Para obter a próxima página de mensagens, aplique a URL retornada em `@odata.nextLink` a uma solicitação GET subsequente.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages(sender,subject)",
  "value": [
    {
      "@odata.etag": "W/\"CQAAABYAAADHcgC8Hl9tRZ/hc1wEUs1TAAAwR4Hg\"",
      "id": "AAMkAGUAAAwTW09AAA=",
      "subject": "You have late tasks!",
      "sender": {
        "emailAddress": {
          "name": "Microsoft Planner",
          "address": "noreply@Planner.Office365.com"
        }
      }
    }
  ]
}
```

### <a name="example-2-use-filter-to-get-all-messages-satisfying-a-specific-condition"></a>Exemplo 2: use $filter para obter todas as mensagens que satisfazem uma condição específica
#### <a name="request"></a>Solicitação
O próximo exemplo filtra todas as mensagens na caixa de correio do usuário de entrada para aqueles que mencionam o usuário. Ele também usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta. 

O exemplo também incorpora a codificação de URL para os caracteres de espaço na cadeia de caracteres do parâmetro de consulta.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-with-mentions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-with-mentions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-with-mentions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-with-mentions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

### <a name="example-3-use-prefer-header-to-get-the-message-body-and-uniquebody-is-text-format"></a>Exemplo 3: use o header prefer para obter o corpo da mensagem e uniqueBody é o formato de texto
#### <a name="request"></a>Solicitação
O terceiro exemplo mostra como usar um header para obter as propriedades body e `Prefer: outlook.body-content-type="text"` **uniqueBody**  de cada mensagem no formato de texto.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messages-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messages-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messages-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-messages-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
  "value":[
    {
      "@odata.type":"#microsoft.graph.eventMessageRequest",
      "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
      "id":"AAMkAGIAAAoZCfIAAA=",
      "subject":"Orientation ",
      "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
      "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
      },
      "uniqueBody":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
