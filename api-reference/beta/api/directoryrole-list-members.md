---
title: Listar membros
description: Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.
author: abhijeetsinha
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 689c75ffb5957c717e9c35996e5d634df9ce5a28
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63671493"
---
# <a name="list-members"></a>Listar membros

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.

Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API. A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure. Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-id}/members
GET /directoryRoles/roleTemplateId={roleTemplateId}/members
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.
## <a name="examples"></a>Exemplos

### <a name="example-1-get-the-members-of-a-directory-role-using-role-id"></a>Exemplo 1: Obter os membros de uma função de diretório usando a id de função

#### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-directoryrole-members-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-directoryrole-members-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-the-members-of-a-directory-role-using-roletemplateid"></a>Exemplo 2: Obter os membros de uma função de diretório usando roleTemplateId

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

<!-- disabling snippet generation because of an SDK limitation. For more information, see https://github.com/microsoftgraph/msgraph-sdk-dotnet/issues/1041-->

<!-- {
  "blockType": "ignored",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
