---
title: Adicionar membros
description: Adicione um membro a um Microsoft 365 ou grupo de segurança por meio da propriedade de navegação de membros.
ms.localizationpriority: high
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 781a90f75e070feb17380e4538a340b88831b422
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397627"
---
# <a name="add-members"></a>Adicionar membros

Namespace: microsoft.graph

Adicione um membro a um grupo de segurança ou Microsoft 365 por meio da propriedade de navegação de **membros**.

A tabela a seguir mostra os tipos de membros que podem ser adicionados a grupos de segurança ou grupos do Microsoft 365.

| Tipo de objeto             | Membro de grupos de segurança     | Membro do Microsoft 365 grupo |
|-------------------------|-------------------------------|-------------------------------|
| Usuários                   | ![Pode ser membro do grupo][Yes]   | ![Pode ser membro do grupo][Yes]   |
| Grupos de segurança         | ![Pode ser membro do grupo][Yes]   | ![Não pode ser membro do grupo][No] |
| Grupos do Microsoft 365    | ![Não pode ser membro do grupo][No] | ![Não pode ser membro do grupo][No] |
| Dispositivos                 | ![Pode ser membro do grupo][Yes]   | ![Não pode ser membro do grupo][No] |
| Entidades de serviço      | ![Pode ser membro do grupo][Yes]   | ![Não pode ser membro do grupo][No] |
| Contatos organizacionais | ![Pode ser membro do grupo][Yes]   | ![Não pode ser membro do grupo][No] |

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                |
| :------------------------------------- | :------------------------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All    |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                                             |
| Aplicativo                            | GroupMember.ReadWrite.All, Group.ReadWrite.All and Directory.ReadWrite.All |

> [!IMPORTANT]
> Para adicionar membros a um grupo atribuível a função, o usuário ou aplicativo de chamada também deve ser atribuído à permissão _RoleManagement.ReadWrite.Directory_.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                       |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md), [group](../resources/group.md) ou [organizational contact](../resources/orgcontact.md) a ser adicionado.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta. Esse método retorna um `400 Bad Request` código de resposta quando o objeto já é um membro do grupo. Esse método retorna um `404 Not Found` código de resposta quando o objeto adicionado não existe.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-a-member-to-a-group"></a>Exemplo 1: adicionar um membro a um grupo

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "add_member_to_group"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{group-id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/add-member-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/add-member-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/add-member-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/add-member-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-member-to-group-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/add-member-to-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)

[!INCLUDE [sample-code](../includes/snippets/powershell/add-member-to-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

No corpo da solicitação, forneça uma representação JSON da ID do objeto directoryObject, usuário ou grupo que deseja adicionar.

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-add-multiple-members-to-a-group-in-a-single-request"></a>Exemplo 2: adicionar vários membros a um grupo em uma única solicitação

Esse exemplo mostra como adicionar vários membros a um grupo com suporte vinculado OData em uma operação PATCH. Observe que é possível adicionar até 20 membros em uma única solicitação. Não há suporte para a operação POST. Se houver uma condição de erro no corpo da solicitação, nenhum membro será adicionado e o código de resposta apropriado será retornado.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "add_multiple_members_to_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{group-id}
Content-type: application/json

{
  "members@odata.bind": [
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
    "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
    ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/add-multiple-members-to-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/add-multiple-members-to-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/add-multiple-members-to-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/add-multiple-members-to-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-multiple-members-to-group-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/add-multiple-members-to-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/add-multiple-members-to-group-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/add-multiple-members-to-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

No corpo da solicitação, forneça uma representação JSON da ID do objeto directoryObject, usuário ou grupo que deseja adicionar.

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Confira também

- [Adicionar membro à equipe](team-post-members.md)
- [Atualizar a função do membro na equipe](team-update-members.md)
- [Remover membro da equipe](team-delete-members.md)



[Yes]: /graph/images/yesandnosymbols/greencheck.svg
[No]: /graph/images/yesandnosymbols/no.svg

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api/group-post-members.md:
      Failed to parse enumeration values for type microsoft.graph.add. Table requires a column header named one of the following: Member, Name, Value"
  ]
}-->
