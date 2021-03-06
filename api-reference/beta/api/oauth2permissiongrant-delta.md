---
title: 'oauth2permissiongrant: delta'
description: Obter recém-criados, atualizados ou excluídos oauth2permissiongrants sem executar uma leitura completa de toda a coleção de recursos.
localization_priority: Normal
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e4a4568dc143148597729e5b0981bda606649e27
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442375"
---
# <a name="oauth2permissiongrant-delta"></a>oauth2permissiongrant: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter objetos **oauth2permissiongrant** recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos. Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|oauth2permissiongrant | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para começar a controlar as alterações, você faz uma solicitação incluindo a função delta no recurso **oauth2permissiongrant.**

<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.** Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta uma vez na frente. Em solicitações subsequentes, copie e aplique `nextLink` a URL ou da resposta `deltaLink` anterior. Essa URL já inclui os parâmetros codificados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de `deltaLink` alterações.  Salve e aplique a URL inteira, incluindo esse token, na primeira solicitação da próxima rodada de controle `deltaLink` de alterações para essa coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na `nextLink` mesma coleção de recursos.  |

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade **id** sempre será retornada.
- Há suporte limitado para `$filter`:
  * A única expressão `$filter` com suporte é para controlar alterações para recursos específicos, por sua ID: ou  `$filter=id+eq+{value}` `$filter=id+eq+{value1}+or+id+eq+{value2}` . O número de IDs que você pode especificar é limitado pelo tamanho máximo da URL.


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;token&gt; de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um objeto da coleção `200 OK` [oauth2permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta. A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.

- Se uma URL `nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O **oauth2permissiongrant** continua fazendo solicitações usando `nextLink` a URL até que uma URL seja incluída na `deltaLink` resposta.
- Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Persista e use `deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.

Para obter detalhes, consulte [Using delta query](/graph/delta-query-overview). Por exemplo, solicitações, [consulte Obter alterações incrementais para usuários](/graph/delta-query-users).

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/oauth2permissiongrant-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/oauth2permissiongrant-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/oauth2permissiongrant-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/oauth2permissiongrant-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/beta/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "expiryTime": "2017-08-13T21:41:23.3929007Z",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "startTime": "0001-01-01T00:00:00Z",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


