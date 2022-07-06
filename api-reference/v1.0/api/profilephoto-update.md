---
title: Atualizar profilePhoto
description: Atualize a foto do usuário conectado, ou do grupo ou cotato especificado.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fb3ccef7898305dbd76f891ff85019da853187dc
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645480"
---
# <a name="update-profilephoto"></a>Atualizar profilePhoto

Namespace: microsoft.graph

Atualize a foto do **usuário** conectado, ou do **grupo** ou **cotato** especificado.

Devido ao limite atual de 4 MB no tamanho total de cada solicitação REST, o tamanho da foto que você pode adicionar também é limitado a 4 MB. A seguir estão as dimensões com suporte para fotos HD em Exchange Online: `48x48`, `64x64`, , `96x96`, `120x120`, `240x240`, `432x432``360x360`, `504x504`e `648x648`.

Você pode usar PATCH ou PUT para esta operação na versão 1.0.

> **Nota:** Essa operação dá suporte apenas a caixas de correio corporativas ou de estudante de um usuário e não a caixas de correio pessoais.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="to-update-the-profile-photo-of-the-signed-in-user"></a>Para atualizar a foto do perfil do usuário conectado

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   User.ReadWrite, User.ReadWrite.All           |
|Delegado (conta pessoal da Microsoft)      |   Sem suporte.            |
|Aplicativo      |    User.ReadWrite.All           |

### <a name="to-update-the-profile-photo-of-a-group"></a>Para atualizar a foto de perfil de um grupo

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   Group.ReadWrite.All           |
|Delegado (conta pessoal da Microsoft)      |   Sem suporte.            |
|Aplicativo      |    Group.ReadWrite.All           |

### <a name="to-update-the-profile-photo-of-a-contact"></a>Para atualizar a foto de perfil de um contato

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)      |   Contacts.ReadWrite           |
|Delegado (conta pessoal da Microsoft)      |   Sem suporte.            |
|Aplicativo      |    Contacts.ReadWrite           |

> [!NOTE]
> 1. Para atualizar a foto de qualquer usuário na organização, seu aplicativo deve ter a permissão de aplicativo *User.ReadWrite.All* e chamar essa API em sua própria identidade, não em nome de um usuário. Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service). Atualizar a foto do usuário conectado requer apenas a *permissão User.ReadWrite* .
> 2. Atualmente, há um [problema conhecido](/graph/known-issues#groups) ao acessar fotos de grupo usando permissões de aplicativos.
> 3. Atualmente, não há suporte para a atualização da foto de um usuário usando o Microsoft API do Graph em locatários Azure AD B2C.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | image/jpeg. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Inclua os dados binários da foto no corpo da solicitação.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `200 OK`.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
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

### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

