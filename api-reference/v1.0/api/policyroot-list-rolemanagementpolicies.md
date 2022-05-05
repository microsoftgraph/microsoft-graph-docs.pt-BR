---
title: Listar roleManagementPolicies
description: Obtenha políticas de gerenciamento de funções e seus detalhes.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4bf5de02bc5a89fc86878ca1773fc16469f84b88
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207634"
---
# <a name="list-rolemanagementpolicies"></a>Listar roleManagementPolicies
Namespace: microsoft.graph

Obtenha políticas de gerenciamento de funções e seus detalhes.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies?$filter=scopeId eq 'scopeId' and scopeType eq 'scopeType'
```

## <a name="query-parameters"></a>Parâmetros de consulta
Esse método requer o parâmetro `$filter` de consulta (`eq`) para definir o escopo da solicitação para **um scopeId** e **um scopeType**. Você também pode usar os parâmetros `$select` de `$expand` consulta e OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de [objetos unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-the-role-management-policies-that-apply-to-azure-ad-roles"></a>Exemplo 1: recuperar as políticas de gerenciamento de função que se aplicam a Azure AD funções

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/roleManagementPolicies?$filter=scopeId eq '/' and scopeType eq 'DirectoryRole'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-unifiedrolemanagementpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/roleManagementPolicies",
    "value": [
        {
            "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448",
            "displayName": "DirectoryRole",
            "description": "DirectoryRole",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "lastModifiedDateTime": null,
            "lastModifiedBy": {
                "displayName": null,
                "id": null
            }
        },
        {
            "id": "DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_23b16f1a-1f8d-4891-93b1-21244cdf6115",
            "displayName": "DirectoryRole",
            "description": "DirectoryRole",
            "isOrganizationDefault": false,
            "scopeId": "/",
            "scopeType": "DirectoryRole",
            "lastModifiedDateTime": null,
            "lastModifiedBy": {
                "displayName": null,
                "id": null
            }
        }
    ]
}
```
