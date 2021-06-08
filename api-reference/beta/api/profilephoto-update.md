---
title: Atualizar profilephoto
description: Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. Desde lá
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: e6ccd0fe70f2e48c890df074c6a7865cbf502f83
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787587"
---
# <a name="update-profilephoto"></a>Atualizar profilephoto

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize a foto para qualquer usuário no locatário, incluindo o usuário ou o grupo ou contato especificado. Como atualmente há um limite de 8 MB no tamanho total de cada solicitação REST, o tamanho da foto que você pode adicionar é limitado a menos de 8 MB.

Use SOMENTE PUT para essa operação.

> **Observação**: ao atualizar a **foto do usuário,** essa operação tenta primeiro atualizar a foto no Microsoft 365. Se isso falhar (devido ao usuário não ter uma caixa de correio), essa API tentará atualizar a foto no Azure Active Directory.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Foto de perfil do usuário **de entrada**:<br/>User.ReadWrite, User.ReadWrite.All<br /><br />Para recurso de **grupo**:<br />Group.ReadWrite.All<br /><br />Para recurso de **contato**:<br />Contacts.ReadWrite |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Para recurso de **usuário**:<br/>User.ReadWrite.All<br /><br />Para recurso de **grupo**:<br />Group.ReadWrite.All<br /><br />Para recurso de **contato**:<br />Contacts.ReadWrite |

> **Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão do aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário. Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service). A atualização da foto do usuário in-loco requer apenas a permissão User.ReadWrite.

> **Observação:** Há um [problema conhecido](/graph/known-issues#groups)ao acessar fotos de grupo usando permissões de aplicativo.

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

Se tiver êxito, este método retornará um código de resposta `200 OK`.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
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


