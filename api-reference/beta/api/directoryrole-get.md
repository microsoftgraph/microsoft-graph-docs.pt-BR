---
title: Obter directoryRole
description: Recupere as propriedades de um objeto directoryRole.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: dd6f1328611a04633161c461891f0754219f8ea2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999255"
---
# <a name="get-directoryrole"></a>Obter directoryRole

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades de um objeto directoryRole.

Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API. A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure. Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-id}
GET /directoryRoles/roleTemplateId={roleTemplateId}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método não **dá suporte** a nenhum parâmetro de [consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, `$filter` não há suporte aqui).

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.
## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-definition-of-a-directory-role-using-role-id"></a>Exemplo 1: Obter a definição de uma função de diretório usando a id de função
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryrole-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
    "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
    "deletedDateTime": null,
    "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
    "displayName": "Directory Readers",
    "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```


### <a name="example-2-get-the-definition-of-a-directory-role-using-roletemplateid"></a>Exemplo 2: Obter a definição de uma função de diretório usando roleTemplateId
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryrole-templateid-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
    "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
    "deletedDateTime": null,
    "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
    "displayName": "Directory Readers",
    "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
