---
title: 'mailFolder: delta'
description: Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.
ms.localizationpriority: medium
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1512efecdeeea0c5b98eea57801f32dab093db0f
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246745"
---
# <a name="mailfolder-delta"></a>mailFolder: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.

Uma chamada de função **delta** de pastas de email em uma caixa de correio é semelhante a uma solicitação GET, exceto que, aplicando adequadamente os [tokens de estado](/graph/delta-query-overview) em uma ou mais dessas chamadas, permite consultar alterações incrementais nas pastas de email. Isso permite manter e sincronizar um armazenamento local de pastas de email do usuário sem ter que sempre buscar todas as pastas de email dessa caixa de correio.

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
GET /me/mailFolders/delta
GET /users/{id}/mailFolders/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações em pastas de email corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `@odata.nextLink` ou `@odata.deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `@odata.nextLink` ou `@odata.deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `@odata.deltaLink` da chamada de função **delta** anterior da mesma coleção de pastas de email indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `@odata.deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações da coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL `@odata.nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas na mesma coleção de pastas de email. |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:----------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | string  | application/json. Obrigatório. |
| Preferir | cadeia de caracteres  | odata.maxpagesize={x}. Opcional. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [mailFolder](../resources/mailfolder.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de pastas de email no corpo da resposta a 2.

Para controlar as alterações nas pastas de email de uma caixa de correio, faça uma ou mais chamadas de função **delta**, com os tokens de estado apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta. 

Você pode encontrar um exemplo semelhante que mostra como usar os tokens de estado para controlar alterações em mensagens de uma pasta de email: [Obtenha alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages). As principais diferenças entre o controle de pastas de email e o controle de mensagens em uma pasta encontram-se nas URLs das solicitações da consulta delta e nas respostas da consulta que retornam **mailFolder** em vez de coleções de **mensagens**.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/delta

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-delta-java-snippets.md)]
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
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "wellKnownName": "wellKnownName-value"
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
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


