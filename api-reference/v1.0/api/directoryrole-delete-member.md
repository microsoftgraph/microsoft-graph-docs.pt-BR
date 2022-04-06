---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fc53b761f5ff9201416604fb71e58c8f04e57270
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63672564"
---
# <a name="remove-directory-role-member"></a>Remover membro da função de diretório

Namespace: microsoft.graph

Remova um membro de um [directoryRole](../resources/directoryrole.md).

Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API. A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure. Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | RoleManagement.ReadWrite.Directory    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.ReadWrite.Directory |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{role-id}/members/{id}/$ref
DELETE /directoryRoles/roleTemplateId={roleTemplateId}/members/{id}/$ref
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-remove-directory-role-member-using-role-id"></a>Exemplo 1: Remover membro da função de diretório usando a id de função

#### <a name="request"></a>Solicitação

Neste exemplo, substitua `f8e85ed8-f66f-4058-b170-3efae8b9c6e5` pelo valor **de id** `bb165b45-151c-4cf6-9911-cd7188912848` da função de diretório e pelo valor **de id** do usuário ou objeto de diretório que você deseja desasinalhar da função de diretório.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_objectId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-roletemplateid"></a>Exemplo 2: Remover membro da função de diretório usando roleTemplateId

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Substitua `9f06204d-73c1-4d4c-880a-6edb90606fd8` pelo valor de sua roleTemplateId e `bb165b45-151c-4cf6-9911-cd7188912848` pelo valor **de id** do usuário do objeto directory.

<!-- disabling snippet generation because of an SDK limitation. For more information, see https://github.com/microsoftgraph/msgraph-sdk-dotnet/issues/1041-->

<!-- {
  "blockType": "ignored",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=9f06204d-73c1-4d4c-880a-6edb90606fd8/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```


#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

