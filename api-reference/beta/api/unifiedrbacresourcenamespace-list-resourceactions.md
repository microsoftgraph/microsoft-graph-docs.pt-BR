---
title: Listar resourceActions
description: Obter uma lista dos objetos unifiedRbacResourceAction e suas propriedades.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 31e1893bbd57d8971fbe7b4f29001d204c164151
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337979"
---
# <a name="list-resourceactions"></a>Listar resourceActions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista dos [objetos unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/resourceNamespaces/{unifiedRbacResourceNamespaceId}/resourceActions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos `$filter`parâmetros de consulta , `$select`, `$top`e `$skipToken` OData para ajudar a personalizar a resposta. Este método oferece suporte `$filter` (`eq`) **para propriedades actionVerb**, **description**, **id** e **name** . Este método retorna um tamanho de página padrão de 100 **resourceActions** e oferece suporte `$top` e `$skipToken` para pajamento. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [unifiedRbacResourceAction](../resources/unifiedrbacresourceaction.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-get-microsoftdirectory-actions"></a>Exemplo 1: Obter ações microsoft.directory

O exemplo a seguir obtém as ações do namespace de recurso com o identificador de `microsoft.directory`.

Este método retorna um máximo de 100 ações. Se houver mais ações, você poderá usar `@odata.nextLink` para obter o próximo conjunto de ações.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrbacresourceaction_directory"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/resourceNamespaces/microsoft.directory/resourceActions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrbacresourceaction-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrbacresourceaction-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrbacresourceaction-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrbacresourceaction-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrbacresourceaction-directory-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-unifiedrbacresourceaction-directory-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
>**Observação:** O objeto de resposta mostrado aqui foi reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRbacResourceAction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/resourceNamespaces('microsoft.directory')/resourceActions",
    "@odata.nextLink": "https://graph.microsoft.com/beta/roleManagement/directory/resourceNamespaces/microsoft.directory/resourceActions?$skiptoken=bWljcm9z...",
    "value": [
        {
            "actionVerb": null,
            "description": "Create and delete access reviews, and read and update all properties of access reviews in Azure AD",
            "id": "microsoft.directory-accessReviews-allProperties-allTasks",
            "name": "microsoft.directory/accessReviews/allProperties/allTasks",
            "resourceScopeId": null
        },
        {
            "actionVerb": "GET",
            "description": "Read all properties of access reviews",
            "id": "microsoft.directory-accessReviews-allProperties-read-get",
            "name": "microsoft.directory/accessReviews/allProperties/read",
            "resourceScopeId": null
        },
        {
            "actionVerb": null,
            "description": "Manage access reviews of application role assignments in Azure AD",
            "id": "microsoft.directory-accessReviews-definitions.applications-allProperties-allTasks",
            "name": "microsoft.directory/accessReviews/definitions.applications/allProperties/allTasks",
            "resourceScopeId": null
        }
    ]
}
```

### <a name="example-2-get-microsoftinsights-actions"></a>Exemplo 2: Obter ações do microsoft.insights

O exemplo a seguir obtém as ações do namespace de recurso com o identificador de `microsoft.insights`.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrbacresourceaction_insights"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/resourceNamespaces/microsoft.insights/resourceActions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrbacresourceaction-insights-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrbacresourceaction-insights-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrbacresourceaction-insights-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrbacresourceaction-insights-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrbacresourceaction-insights-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-unifiedrbacresourceaction-insights-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRbacResourceAction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/resourceNamespaces('microsoft.insights')/resourceActions",
    "value": [
        {
            "actionVerb": null,
            "description": "Manage all aspects of Insights app",
            "id": "microsoft.insights-allEntities-allProperties-allTasks",
            "name": "microsoft.insights/allEntities/allProperties/allTasks",
            "resourceScopeId": null
        },
        {
            "actionVerb": null,
            "description": "Read all aspects of Viva Insights",
            "id": "microsoft.insights-allEntities-allProperties-read",
            "name": "microsoft.insights/allEntities/allProperties/read",
            "resourceScopeId": null
        },
        {
            "actionVerb": "PATCH",
            "description": "Deploy and manage programs in Insights app",
            "id": "microsoft.insights-programs-allProperties-update-patch",
            "name": "microsoft.insights/programs/allProperties/update",
            "resourceScopeId": null
        },
        {
            "actionVerb": null,
            "description": "Run and manage queries in Viva Insights",
            "id": "microsoft.insights-queries-allProperties-allTasks",
            "name": "microsoft.insights/queries/allProperties/allTasks",
            "resourceScopeId": null
        },
        {
            "actionVerb": "GET",
            "description": "View reports and dashboard in Insights app",
            "id": "microsoft.insights-reports-allProperties-read-get",
            "name": "microsoft.insights/reports/allProperties/read",
            "resourceScopeId": null
        }
    ]
}
```
