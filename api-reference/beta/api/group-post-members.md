---
title: Adicionar membros
description: Adicione um membro a um Microsoft 365 ou grupo de segurança por meio da propriedade de navegação de membros.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2fbf9592c6b0659724c87c6391757594f1cfae58
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645533"
---
# <a name="add-members"></a>Adicionar membros

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Adicione um membro a um grupo de segurança ou Microsoft 365 por meio da propriedade de navegação de **membros**.

A tabela a seguir mostra os tipos de membros que podem ser adicionados a grupos de segurança ou grupos do Microsoft 365.

| Tipo de objeto             | Membro do grupo de segurança     | Membro do Microsoft 365 grupo |
|-------------------------|-------------------------------|-------------------------------|
| Usuário                   | ![Pode ser membro do grupo][Yes]   | ![Pode ser membro do grupo][Yes]   |
| Grupo de segurança         | ![Pode ser membro do grupo][Yes]   | ![Não pode ser membro do grupo][No] |
| Grupo Microsoft 365    | ![Não pode ser membro do grupo][No] | ![Não pode ser membro do grupo][No] |
| Dispositivo                 | ![Pode ser membro do grupo][Yes]   | ![Não pode ser membro do grupo][No] |
| Entidade de serviço      | ![Pode ser membro do grupo][Yes]   | ![Não pode ser membro do grupo][No] |
| Contatos organizacionais | ![Pode ser membro do grupo][Yes]   | ![Não pode ser membro do grupo][No] |


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                             |
| :------------------------------------- | :---------------------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                                          |
| Aplicativo                            | GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All |

> [!IMPORTANT]
> Para adicionar membros a um grupo atribuível a função, o usuário ou aplicativo de chamada também deve ser atribuído à permissão _RoleManagement.ReadWrite.Directory_.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{group-id}/members/$ref
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md), [user](../resources/user.md) ou [group](../resources/group.md) a ser adicionado.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta. Esse método retorna um `400 Bad Request` código de resposta quando o objeto já é um membro do grupo. Esse método retorna um `404 Not Found` código de resposta quando o objeto adicionado não existe.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "add_group_member"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{group-id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}
```

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/add-group-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/add-group-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/add-group-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/add-group-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-group-member-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/add-group-member-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/add-group-member-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/add-group-member-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

No corpo da solicitação, forneça uma representação JSON `id` do [objeto directoryObject](../resources/directoryobject.md), [usuário](../resources/user.md) [ou grupo que](../resources/group.md) você deseja adicionar.

### <a name="response"></a>Resposta

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
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
