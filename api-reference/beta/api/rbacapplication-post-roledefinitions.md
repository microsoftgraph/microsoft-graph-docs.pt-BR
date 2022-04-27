---
title: Criar unifiedRoleDefinition
description: Crie um novo objeto unifiedRoleDefinition.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7ed0b30e2e2f1a2c7c0b995cc8062a4bf0e68fde
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061080"
---
# <a name="create-unifiedroledefinition"></a>Criar unifiedRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) para um provedor RBAC.

No momento, há suporte para os seguintes provedores RBAC:
- PC na nuvem
- gerenciamento de dispositivo (Intune)
- directory (Azure AD)

## <a name="permissions"></a>Permissões

Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha entre as tabelas a permissão menos privilegiada necessária para chamar essa API. Para saber mais, incluindo [ter cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher permissões mais privilegiadas, consulte [Permissões](/graph/permissions-reference). 

### <a name="for-a-cloud-pc-provider"></a>Para um provedor de PC na nuvem

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | RoleManagement.ReadWrite.CloudPC, CloudPC.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.ReadWrite.CloudPC, CloudPC.ReadWrite.All  |

### <a name="for-a-device-management-intune-provider"></a>Para um provedor de gerenciamento de dispositivos (Intune)

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  DeviceManagementRBAC.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | DeviceManagementRBAC.ReadWrite.All |

### <a name="for-a-directory-azure-ad-provider"></a>Para um provedor de diretório (Azure AD)

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para criar uma definição de função para um provedor de gerenciamento de dispositivo:
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/deviceManagement/roleDefinitions
```

Para criar uma definição de função para um provedor de diretório:
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/directory/roleDefinitions
```

Para criar uma definição de função para um provedor de PC na nuvem:
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/cloudPc/roleDefinitions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do [objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar uma roleDefinition.

| Parâmetro | Tipo | Descrição|
|:---------------|:--------|:----------|
|displayName |string |O nome de exibição para a definição de função.|
|isEnabled |Booliano |Sinalizador que indica se a função está habilitada para atribuição. Se for false, a função não estará disponível para atribuição.|
|rolePermissions |[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md) |Lista de permissões incluídas na função.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` o código de resposta e um novo objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.

## <a name="example-1create-a-custom-role-for-a-directory-provider"></a>Exemplo 1: Criar uma função personalizada para um provedor de diretório

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroledefinition-from-rbacapplication-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroledefinition-from-rbacapplication-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "description": "Update basic properties of application registrations",
    "displayName": "Application Registration Support Administrator",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/standard/read",
                "microsoft.directory/applications/basic/update"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('d5eec5e0-6992-4c6b-b430-0f833f1a815a')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-create-a-custom-role-for-a-cloud-pc-provider"></a>Exemplo 2: Criar uma função personalizada para um provedor de PC na nuvem

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication_cloudpc"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/cloudPc/roleDefinitions
Content-type: application/json

{
  "description": "An example custom role",
  "displayName": "ExampleCustomRole",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "Microsoft.CloudPC/CloudPCs/Read"
            ]
        }
    ],
    "condition" : "null"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-unifiedroledefinition-from-rbacapplication-cloudpc-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-unifiedroledefinition-from-rbacapplication-cloudpc-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPc/roleDefinitions/$entity",
    "id": "b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff",
    "description": "An example custom role",
    "displayName": "ExampleCustomRole",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "Microsoft.CloudPC/CloudPCs/Read"
            ],
            "condition": null
        }
    ],
    "resourceScopes":["/"]
}
```
