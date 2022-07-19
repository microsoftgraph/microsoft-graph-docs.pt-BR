---
title: Atualizar profilephoto
description: Atualize a foto para qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato ou equipe especificado.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: people
author: kevinbellinger
ms.openlocfilehash: 4e930f96076f37ee39ef578c4f091af75cf9acc6
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855753"
---
# <a name="update-profilephoto"></a>Atualizar profilephoto

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize a foto do contato, grupo, equipe ou usuário especificado em um locatário. O tamanho da foto que você pode atualizar deve ter menos de 8 MB.

Use PUT somente para esta operação.

> **Observação**: ao atualizar a foto **do** usuário, esta operação tenta primeiro atualizar a foto no Microsoft 365. Se isso falhar (devido ao usuário não ter uma caixa de correio), essa API tentará atualizar a foto no Azure Active Directory.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="to-update-the-profile-photo-of-a-contact"></a>Para atualizar a foto de perfil de um contato

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   Contacts.ReadWrite           |
|Delegado (conta pessoal da Microsoft)      |   Sem suporte.            |
|Aplicativo      |    Contacts.ReadWrite           |

### <a name="to-update-the-profile-photo-of-a-group"></a>Para atualizar a foto de perfil de um grupo

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   Group.ReadWrite.All           |
|Delegado (conta pessoal da Microsoft)      |   Sem suporte.            |
|Aplicativo      |    Group.ReadWrite.All           |

### <a name="to-update-the-profile-photo-of-a-team"></a>Para atualizar a foto de perfil de uma equipe

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                            |
|:---------------------------------------|:-----------------------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | TeamSettingsReadWriteAll, GroupReadWriteAll **, DirectoryReadWriteAll** |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                         |
| Aplicativo                            | Sem suporte.                                                         |

[!INCLUDE [teamwork-permissions-note](../../../includes/teamwork-permissions-note.md)]

### <a name="to-update-the-profile-photo-of-the-signed-in-user"></a>Para atualizar a foto do perfil do usuário conectado

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   User.ReadWrite, User.ReadWrite.All           |
|Delegado (conta pessoal da Microsoft)      |   Sem suporte.            |
|Aplicativo      |    User.ReadWrite.All           |

> [!NOTE]
> 1. Para atualizar a foto de qualquer usuário na organização, seu aplicativo deve ter a permissão de aplicativo *User.ReadWrite.All* e chamar essa API em sua própria identidade, não em nome de um usuário. Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service). Atualizar a foto do usuário conectado requer apenas a *permissão User.ReadWrite* .
> 2. Atualmente, há um [problema conhecido](/graph/known-issues#groups) ao acessar fotos de grupo usando permissões de aplicativos.
> 3. Atualmente, não há suporte para a atualização da foto de um usuário usando o Microsoft API do Graph em locatários Azure AD B2C.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```

Para atualizar a foto de uma equipe:

<!-- { "blockType": "ignored" } -->

```http
PUT /groups/{teamId}/photo/$value
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | image/jpeg. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Inclua os dados binários da foto no corpo da solicitação.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta ou um `204 No Content` código de resposta para atualizar a foto de uma equipe.

## <a name="examples"></a>Exemplos
### <a name="example-1-update-the-profile-photo-of-the-user"></a>Exemplo 1: atualizar a foto do perfil do usuário
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

### <a name="example-2-update-the-photo-of-a-team"></a>Exemplo 2: Atualizar a foto de uma equipe

#### <a name="request"></a>Solicitação
A seguir está um exemplo de uma solicitação para atualizar uma foto da equipe.

<!-- {
  "blockType": "request",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8491e/photo/$value
Content-type: image/jpeg

Binary data for the image
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
