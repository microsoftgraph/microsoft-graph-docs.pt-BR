---
title: Excluir unifiedRoleDefinition
description: Exclua um objeto unifiedRoleDefinition.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6669181c336d2f70268cd82eabd06cc7452ec001
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525509"
---
# <a name="delete-unifiedroledefinition"></a>Excluir unifiedRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Exclua um objeto unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) para um provedor RBAC.

No momento, há suporte para os seguintes provedores RBAC:
- Cloud PC
- gerenciamento de dispositivos (Intune)
- directory (Azure AD) 

## <a name="permissions"></a>Permissions

Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha entre as tabelas a permissão menos privilegiada necessária para chamar essa API. Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference). 

### <a name="for-a-cloud-pc-provider"></a>Para um provedor de computadores na nuvem

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | CloudPC.ReadWrite.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | CloudPC.ReadWrite.All  |

### <a name="for-a-device-management-intune-provider"></a>Para um provedor de gerenciamento de dispositivos (Intune)

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  DeviceManagementRBAC.ReadWrite.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | DeviceManagementRBAC.ReadWrite.All |

### <a name="for-a-directory-azure-ad-provider"></a>Para um provedor de diretório (Azure AD)

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para excluir uma definição de função para um provedor de gerenciamento de dispositivos:
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/deviceManagement/roleDefinitions/{id}
```

Para excluir uma definição de função para um provedor de diretórios:
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

Para excluir uma definição de função para um provedor de computadores na nuvem:
<!-- { "blockType": "ignored" } -->
```http
DELETE /roleManagement/cloudPc/roleDefinitions/{id}

```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example-1-delete-a-unifiedroledefinition-resource-for-a-directory-provider"></a>Exemplo 1: excluir um **recurso unifiedRoleDefinition** para um provedor de diretórios

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-unifiedroledefinition-go-snippets.md)]
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="example-2-delete-a-unifiedroledefinition-resource-for-a-cloud-pc-provider"></a>Exemplo 2: excluir um **recurso unifiedRoleDefinition** para um provedor de computadores na nuvem
### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition_cloudpc"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/cloudPc/roleDefinitions/b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
