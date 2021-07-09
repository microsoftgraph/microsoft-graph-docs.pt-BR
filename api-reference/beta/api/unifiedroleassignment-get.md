---
title: Obter unifiedRoleAssignment
description: Recupere as propriedades e as relações de um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 238b2e1d6049ec53d779fddba830338b13b6f781
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351033"
---
# <a name="get-unifiedroleassignment"></a>Obter unifiedRoleAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações de um [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)

## <a name="permissions"></a>Permissões

Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API. Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).

### <a name="for-directory-azure-ad-provider"></a>Provedor do Azure AD (Diretório)

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

### <a name="for-entitlement-management-provider"></a>Para provedor de gerenciamento de direitos

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

Obter uma atribuição de função para um provedor de diretórios:

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

Obter uma atribuição de função para o provedor de gerenciamento de direitos:

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) solicitado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1--get-details-of-a-role-assignment"></a>Exemplo 1 : Obter detalhes de uma atribuição de função

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0"
}
```

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a>Exemplo 2: Obter detalhes de uma atribuição de função com `$expand`

#### <a name="request"></a>Solicitação

A seguir, um exemplo da solicitação com o `$expand` parâmetro de consulta.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "roleDefinition": {
      "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
      "displayName": "Billing Administrator",
      "description": "Can perform common billing related tasks like updating payment information.",
      "rolePermissions": [
        {
          "allowedResourceActions": [
            "microsoft.commerce.billing/allEntities/allTasks",
            "microsoft.directory/organization/basic/update",
          ],
          "excludedResourceActions": []
        }],
      "isEnabled": true,
      },
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "principal": {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d ",
      "userPrincipalName": "alice@contoso.com",
      "displayName": "Alice Smith"
    },
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScope": {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Contoso_Seattle_Admins"
    }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


