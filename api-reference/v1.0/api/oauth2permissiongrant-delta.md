---
title: 'oauth2permissiongrant: delta'
description: Obtenha recém-criados, atualizados ou excluídos oauth2permissiongrants sem executar uma leitura completa de toda a coleção de recursos.
ms.localizationpriority: medium
author: psignoret
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 807f77d0d1b4d8030f7dbcd1fae3fdb046b9aaa7
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247004"
---
# <a name="oauth2permissiongrant-delta"></a>oauth2permissiongrant: delta

Namespace: microsoft.graph

Obtenha objetos [oauth2permissiongrant](../resources/oauth2permissiongrant.md) recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos. Para obter detalhes, consulte [Usando a consulta delta](/graph/delta-query-overview).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP


<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

Controlar alterações incorre em uma rodada de uma ou mais **chamadas de função delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `@odata.nextLink` ou `@odata.deltaLink` fornecida na resposta. Você só precisa especificar parâmetros de consulta uma vez. Em solicitações subsequentes, copie e aplique `@odata.nextLink` a URL `@odata.deltaLink` da resposta anterior. A URL inclui os parâmetros codificados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de](/graph/delta-query-overview) estado retornado na `@odata.deltaLink` URL da chamada de função **delta anterior** para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações. Salve e aplique a `@odata.deltaLink` URL inteira, incluindo esse token, na primeira solicitação da próxima rodada de controle de alterações para essa coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na `@odata.nextLink` URL da chamada de função **delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção de recursos. |

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.

- Você pode usar um `$select` parâmetro de consulta para especificar apenas as propriedades necessárias para obter o melhor desempenho. A propriedade **id** sempre será retornada.
- O `$filter` parâmetro de consulta só pode ser usado para controlar alterações em recursos específicos usando a ID do recurso. Por exemplo: `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}`.


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um [objeto de coleção oauth2permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta. A resposta também inclui uma URL `@odata.nextLink` ou uma URL `@odata.deltaLink`.

- Se uma `@odata.nextLink` URL for retornada, páginas adicionais de dados poderão ser recuperadas na sessão. O **oauth2permissiongrant** continua fazendo `@odata.nextLink` solicitações usando a URL até que uma `@odata.deltaLink` URL seja incluída na resposta.
- Se uma `@odata.deltaLink` URL for retornada, nenhum dado sobre o recurso será retornado. Persista e use `@odata.deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.

Para obter detalhes, consulte [Usando a consulta delta](/graph/delta-query-overview). Para obter solicitações de exemplo, [consulte Obter alterações incrementais para usuários](/graph/delta-query-users).

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants/delta
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/oauth2permissiongrant-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/oauth2permissiongrant-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
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

