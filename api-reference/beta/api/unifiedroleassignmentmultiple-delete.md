---
title: Excluir unifiedRoleAssignmentMultiple
description: Exclua um objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6d888d8755ca39fd4cfb7e9b8d4c93c18bfcb487
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534078"
---
# <a name="delete-unifiedroleassignmentmultiple"></a>Excluir unifiedRoleAssignmentMultiple

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Exclua um objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) de um provedor RBAC. 

Isso é aplicável a um aplicativo RBAC que oferece suporte a várias entidades e escopos. No momento, há suporte para os seguintes provedores RBAC:
- Cloud PC 
- gerenciamento de dispositivos (Intune)

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a>Permissões

Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API. Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference). 

### <a name="for-cloud-pc-provider"></a>Para provedor de computadores na nuvem

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  CloudPC.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | CloudPC.ReadWrite.All  |

### <a name="for-device-management-intune-provider"></a>Para o provedor de gerenciamento de dispositivos (Intune)

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  DeviceManagementRBAC.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | DeviceManagementRBAC.ReadWrite.All |



## <a name="http-request"></a>Solicitação HTTP

Para excluir um unifiedRoleAssignmentMultiple para um provedor de computadores na nuvem:
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/cloudPC/roleAssignments/{id}
```

Para excluir um unifiedRoleAssignmentMultiple para um provedor do Intune:
<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome | Descrição |
|:---- |:----------- |
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="example-1-delete-a-unifiedroleassignmentmultiple-in-an-intune-provider"></a>Exemplo 1: Excluir um unifiedRoleAssignmentMultiple em um provedor do Intune

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-delete-a-unifiedroleassignmentmultiple-in-a-cloud-pc-provider"></a>Exemplo 2: Excluir um unifiedRoleAssignmentMultiple em um provedor de computadores na nuvem

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/id
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroleassignmentmultiple-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


