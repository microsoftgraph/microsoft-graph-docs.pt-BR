---
title: Listar appRoleAssignments concedidos para uma entidade de serviço
description: Recuperar uma lista de atribuições de funções do aplicativo concedidas para uma entidade de serviço.
ms.localizationpriority: high
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 491c5c4f9bca722409f5c93921f0932c9c9de85b
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63669848"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a>Listar appRoleAssignments concedidos para uma entidade de serviço

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recuperar uma lista de [appRoleAssignment](../resources/approleassignment.md) que os usuários, grupos ou entidades de serviço de cliente receberam para a determinada entidade de serviço do recurso.

Por exemplo, se a entidade de serviço do recurso for a entidade de serviço para a API do Microsoft Graph, isso retornará todas as entidades de serviço que receberam todas as permissões de aplicativo para o Microsoft Graph.

Se a entidade de serviço do recurso for um aplicativo com funções de aplicativo concedidas a usuários e grupos, isso retornará todos as funções de aplicativo dos usuários e grupos atribuídas para esse aplicativo.

>**Observação** Essa solicitação pode ter atrasos de replicação para atribuições de função de aplicativo que foram concedidas ou removidas recentemente.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição                |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação para recuperar as atribuições das funções de aplicativo que foram concedidas a uma entidade de serviço.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignedTo
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/serviceprincipal-get-approleassignedto-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/serviceprincipal-get-approleassignedto-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments",
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "creationTimestamp": "2021-02-02T04:22:45.9480566Z",
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "principalDisplayName": "MOD Administrator",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



