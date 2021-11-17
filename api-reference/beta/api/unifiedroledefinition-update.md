---
title: Atualizar unifiedRoleDefinition
description: Atualize as propriedades de um objeto unifiedRoleDefinition.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1b276ef09c72d4945b74fff5ee660c20ab95cb10
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017034"
---
# <a name="update-unifiedroledefinition"></a>Atualizar unifiedRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto unifiedRoleDefinition](../resources/unifiedroledefinition.md) para um provedor RBAC.

No momento, há suporte para os seguintes provedores RBAC:
- gerenciamento de dispositivos (Intune)
- directory (Azure AD) 

> [!NOTE]
> No momento, o provedor RBAC do computador na nuvem dá suporte apenas à [lista](rbacapplication-list-roledefinitions.md) e [obter](unifiedroledefinition-get.md) operações.

## <a name="permissions"></a>Permissões

Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API. Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, pesquise as seguintes permissões na referência [Permissões.](/graph/permissions-reference) 

### <a name="for-device-management-intune-provider"></a>Para o provedor de gerenciamento de dispositivos (Intune)

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  DeviceManagementRBAC.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | DeviceManagementRBAC.ReadWrite.All |

### <a name="for-directory-azure-ad-provider"></a>Provedor do Azure AD (Diretório)

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

Para atualizar uma definição de função para um provedor de gerenciamento de dispositivos:
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

Para atualizar uma definição de função para um provedor de diretórios:
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String| A descrição da definição de função. Somente leitura quando isBuiltIn for true. |
|displayName|String| O nome de exibição da definição de função. Somente leitura quando isBuiltIn for true. Obrigatório.|
|id|Cadeia de caracteres| O identificador exclusivo para a definição de função. Chave, não anulada, somente leitura. |
|isBuiltIn|Booliano| Sinalizador indicando se a definição de função faz parte do conjunto padrão incluído no produto ou personalizado. Somente leitura. |
|isEnabled|Booliano| Sinalizador indicando se a função está habilitada para atribuição. Se for false, a função não estará disponível para atribuição. Somente leitura quando isBuiltIn for true. |
|resourceScopes|Coleção de cadeias de caracteres| Lista de permissões de escopo concedidas pela definição de função a que se aplicam. Atualmente, apenas "/" é suportado. Somente leitura quando isBuiltIn for true. **NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**|
|rolePermissions|[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando isBuiltIn for true. Obrigatório. |
|templateId|Cadeia de caracteres| Identificador de modelo personalizado que pode ser definido quando isBuiltIn é false. Esse identificador normalmente é usado se um identificador precisa ser o mesmo em diretórios diferentes. Somente leitura quando isBuiltIn for true. |
|inheritsPermissionsFrom| [Coleção unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Coleção somente leitura de definições de função que a definição de função determinada herda. Somente funções do Azure AD integrados suportam esse atributo. |
|versão|String| Indica a versão da definição de função. Somente leitura quando isBuiltIn for true.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

O exemplo a seguir atualiza **um unifiedRoleDefinition** para um provedor de diretórios.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-unifiedroledefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


