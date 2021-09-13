---
title: Atualizar unifiedRoleDefinition
description: Atualize as propriedades de um objeto unifiedRoleDefinition.
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fc93caf0471c1f8c0e3d73b895a530b809656548
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59097810"
---
# <a name="update-unifiedroledefinition"></a>Atualizar unifiedRoleDefinition

Namespace: microsoft.graph

Atualize as propriedades de [um objeto unifiedRoleDefinition.](../resources/unifiedroledefinition.md) Não é possível atualizar funções in-lo-

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | RoleManagement.ReadWrite.Directory |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | RoleManagement.ReadWrite.Directory |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
    
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | Portador {token} |
| Content-Type | application/json. Obrigatório. |
    
## <a name="request-body"></a>Corpo da solicitação
    
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para o melhor desempenho, não inclua valores existentes que não foram alterados.
    
A tabela a seguir mostra as propriedades que são necessárias ao atualizar [unifiedRoleDefinition](../resources/unifiedroledefinition.md).

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String| A descrição da definição de função. Somente leitura quando **isBuiltIn** é `true` . |
|displayName|Cadeia de caracteres| O nome de exibição da definição de função. Somente leitura quando **isBuiltIn** é `true` . Obrigatório.|
|isEnabled|Booliano| Sinalizador indicando se a função está habilitada para atribuição. Se `false` , a função não está disponível para atribuição. Somente leitura quando **isBuiltIn** for true. |
|resourceScopes|Coleção de cadeias de caracteres| Lista de escopos e permissões às que a definição de função se aplica. Atualmente, `/` só há suporte. Somente leitura quando **isBuiltIn** for true. **NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**|
|rolePermissions|[Coleção unifiedRolePermission](../resources/unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando **isBuiltIn** é `true` . Obrigatório. |
|templateId|String| Identificador de modelo personalizado que pode ser definido **quando isBuiltIn** é `false` . Esse identificador normalmente é usado se um identificador precisa ser o mesmo em diretórios diferentes. Somente leitura quando **isBuiltIn** é `true` . |
|versão|String| Indica a versão da definição de função. Somente leitura quando **isBuiltIn** é `true` .|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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

---



### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 OK
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

