---
title: Atualizar unifiedRoleDefinition
description: Atualiza as propriedades de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb1cd8a7e8cbef279c5007b3cd721193ff25e518
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218938"
---
# <a name="update-unifiedroledefinition"></a>Atualizar unifiedRoleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades de um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Application                            | RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory |

## <a name="http-request"></a>Solicitação HTTP

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
|description|String| A descrição da definição de função. Somente leitura quando isbuiltem for true. |
|displayName|Cadeia de caracteres| O nome de exibição da definição de função. Somente leitura quando isbuiltem for true. Obrigatório.|
|id|String| O identificador exclusivo da definição de função. Chave, não anulável, somente leitura. |
|isBuiltIn|Booliano| Sinalizador que indica se a definição de função é parte do conjunto padrão incluído no produto ou personalizado. Somente leitura. |
|isEnabled|Boolean| Sinalizador que indica se a função está habilitada para atribuição. Se false, a função não estará disponível para atribuição. Somente leitura quando isbuiltem for true. |
|resourceScopes|Coleção de cadeias de caracteres| Lista de escopos permissões concedidas pela definição de função aplicam-se ao. No momento, só há suporte para "/". Somente leitura quando isbuiltem for true. **NÃO USE. Essa propriedade será preterida em breve. Anexar escopo à atribuição de função.**|
|rolePermissions|coleção [unifiedRolePermission](../resources/unifiedrolepermission.md)| Lista de permissões incluídas na função. Somente leitura quando isbuiltem for true. Obrigatório. |
|templateId|Cadeia de Caracteres| Identificador de modelo personalizado que pode ser definido quando isbuiltem é falso. Esse identificador geralmente é usado se um precisa de um identificador para ser o mesmo em diferentes diretórios. Somente leitura quando isbuiltem for true. |
|versão|String| Indica a versão da definição de função. Somente leitura quando isbuiltem for true.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


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

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.
> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
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
