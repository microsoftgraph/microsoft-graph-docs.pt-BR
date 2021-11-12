---
title: 'message: delta'
description: Obtenha um conjunto de mensagens que foram adicionadas, excluídas ou atualizadas em uma pasta especificada.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a12377bcc74e721f3e43bb378051bca7248ff34b
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60947270"
---
# <a name="message-delta"></a>message: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha um conjunto de mensagens que foram adicionadas, excluídas ou atualizadas em uma pasta especificada.

Uma chamada de função **delta** de mensagens em uma pasta é semelhante a uma solicitação GET, exceto que, aplicando adequadamente os [tokens de estado](/graph/delta-query-overview) em uma ou mais dessas chamadas, permite [consultar alterações incrementais nas mensagens dessa pasta](/graph/delta-query-messages). Isso permite manter e sincronizar um armazenamento local de mensagens do usuário sem ter de buscar todo o conjunto de mensagens do usuário sempre que precisar dele.  

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.ReadBasic, Mail.Read, Mail.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Mail.ReadBasic, Mail.Read, Mail.ReadWrite    |
|Aplicativo | Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages/delta
GET /users/{id}/mailFolders/{id}/messages/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações em mensagens corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | cadeia de caracteres | Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior da mesma coleção de mensagens indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de mensagens. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 
- Suporte à consulta delta `$select`, `$top` e `$expand` para mensagens. 
- Há suporte limitado para `$filter` e `$orderby`:
  * As únicas expressões `$filter` suportadas são `$filter=receivedDateTime+ge+{value}` ou `$filter=receivedDateTime+gt+{value}`.
  * A única expressão `$orderby` suportada é `$orderby=receivedDateTime+desc`. Se você não incluir uma expressão `$orderby`, a ordem de retorno não será garantida. 
- Não há suporte para `$search`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:----------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | string  | application/json. Obrigatório. |
| Preferir | cadeia de caracteres  | odata.maxpagesize={x}. Opcional. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [message](../resources/message.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de mensagens no corpo da resposta a dois.

Para controlar alterações nas mensagens em uma pasta, faça uma ou mais chamadas de função **delta** para obter o conjunto de alterações incrementais desde a última consulta delta. Veja um exemplo que mostra uma série de chamadas de consulta delta em [Obter alterações incrementais para mensagens em uma pasta](/graph/delta-query-messages).
 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/{id}/messages/delta

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Se a solicitação for bem-sucedida, a resposta incluiria um token de estado que é um _skipToken_  
(em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.

A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.

Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders/{id}/messages/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "internetMessageId": "internetMessageId-value",
      "subject": "subject-value",
      "body": {
        "contentType": "contentType-value",
        "content": "content-value"
      }
    }
  ]
}
```

### <a name="see-also"></a>Confira também

- [Consulta delta do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


