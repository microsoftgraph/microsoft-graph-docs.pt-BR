---
title: 'application: delta'
description: Obtenha aplicativos recém-criados, atualizados ou excluídos sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte Usando a Consulta Delta para obter detalhes.
ms.localizationpriority: medium
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: a92d9a6ad83d69d5ef7a11e49b31786d716c6d36
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247200"
---
# <a name="application-delta"></a>application: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha aplicativos recém-criados, atualizados ou excluídos sem precisar executar uma leitura completa de toda a coleção de recursos. Consulte [Usando a Consulta Delta para](/graph/delta-query-overview) obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para começar a controlar as alterações, você faz uma solicitação, incluindo a função delta no recurso do aplicativo. 

<!-- { "blockType": "ignored" } -->
```http
GET /applications/delta
```

### <a name="query-parameters"></a>Parâmetros de consulta

Controlar alterações incorre em uma rodada de uma ou mais **chamadas de função delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `@odata.nextLink` ou `@odata.deltaLink` fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente. Em solicitações subsequentes, copie e aplique a URL `@odata.nextLink` ou `@odata.deltaLink` da resposta anterior, já que essa URL inclui os parâmetros codificados desejados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de](/graph/delta-query-overview) estado retornado na `@odata.deltaLink` URL da chamada de função **delta anterior** para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações. Salve e aplique toda a URL `@odata.deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.|
| $skiptoken | string | Um [token de](/graph/delta-query-overview) estado retornado na `@odata.nextLink` URL da chamada de função **delta anterior** , indicando que há mais alterações a serem controladas na mesma coleção de recursos. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de Consulta OData para ajudar a personalizar a resposta.

- Você pode usar um parâmetro de consulta `$select` como em qualquer solicitação GET para especificar somente as propriedades necessárias para obter melhor desempenho. A propriedade _id_ sempre será retornada. 

- Há suporte limitado para `$filter`:
  * A única expressão com suporte `$filter` é para controlar alterações para recursos específicos, por sua ID:  `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}`. O número de IDs que você pode especificar é limitado pelo comprimento máximo da URL.


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | &lt;Token&gt; de portador|
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se tiver êxito, este método retornará o `200 OK` código de resposta e [o objeto de](../resources/application.md) coleção de aplicativos no corpo da resposta. A resposta também inclui uma URL nextLink ou uma URL deltaLink. 

- Se uma URL `@odata.nextLink` é retornada, existem páginas de dado adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `@odata.nextLink` até uma URL `@odata.deltaLink` ser incluída na resposta.

- Se uma URL `@odata.deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Persista e use `@odata.deltaLink` a URL para saber mais sobre as alterações no recurso no futuro.

Confira:</br>
- [Usando a Consulta Delta](/graph/delta-query-overview) para obter detalhes</br>
- [Obter as alterações incrementais para usuários](/graph/delta-query-users) para solicitações de um exemplo.</br>

### <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/application-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/application-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#applications",
  "@odata.nextLink":"https://graph.microsoft.com/beta/applications/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
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
  "description": "application: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



