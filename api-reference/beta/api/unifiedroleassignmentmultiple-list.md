---
title: Listar UnifiedRoleAssignmentMultiple
description: Recupere as propriedades e os relacionamentos do objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f66bb02a1cb38757e18c31004c67dea7bea7b37
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990287"
---
# <a name="list-unifiedroleassignmentmultiple"></a>Listar UnifiedRoleAssignmentMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista de objetos [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) . Use isso para obter uma lista de atribuições de função no Microsoft Intune. Para outros aplicativos do Micrsoft 365 (como o Azure AD), use o [unifiedRoleAssignment](../resources/unifiedroleassignment.md).

## <a name="permissions"></a>Permissões

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:--------------- |:------------------------------------------- |
| Delegada (conta corporativa ou de estudante) | DeviceManagementRBAC. Read. All, DeviceManagementRBAC. ReadWrite. All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Application | DeviceManagementRBAC. Read. All, DeviceManagementRBAC. ReadWrite. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Você pode filtrar as `roleDefinitionId` Propriedades ou `principalId` . A `roleDefinitionId` propriedade pode ser uma ID de objeto role ou uma ID de objeto de modelo de função. Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
|:---- |:----------- |
| Autorização | Bearer {token}. Required. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.
> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "value": [ 
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
            "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
       },
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "2BNpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SWRD-2",
            "roleDefinitionId": "9e47fc6f-2d7a-464c-944e-d3dd0de522e4",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "53a6c08d-0227-41bd-8bc6-2728df6be749", "a4991fe1-6d7c-427c-969b-bda6df78c458"],
            "appScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0"]
       }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignmentsMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
