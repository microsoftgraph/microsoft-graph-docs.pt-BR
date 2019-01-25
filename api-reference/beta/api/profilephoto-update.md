---
title: Atualizar profilephoto
description: Atualizar a foto para qualquer usuário no locatário incluindo assinado do usuário, ou o grupo especificado ou o contato. Desde daí
localization_priority: Normal
ms.openlocfilehash: f8191716471cba565b27ef316b5b13e3b32ecaff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521128"
---
# <a name="update-profilephoto"></a>Atualizar profilephoto

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar a foto para qualquer usuário no locatário incluindo assinado do usuário, ou o grupo especificado ou o contato. Como no momento, há um limite de 4MB no tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar ao menos de 4MB.

Use apenas PUT para essa operação na versão beta.

> **Observação** A operação de atualização de foto no beta suporta apenas o usuário comercial ou caixas de correio da escola e caixas de correio não pessoais.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Foto de perfil do entrou no **usuário**:<br/>User.ReadWrite, User.ReadWrite.All<br /><br />Para recurso de **grupo**:<br />Group.ReadWrite.All<br /><br />Para recurso de **contato**:<br />Contacts.ReadWrite |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Para recurso de **usuário**:<br/>User.ReadWrite.All<br /><br />Para recurso de **grupo**:<br />Group.ReadWrite.All<br /><br />Para recurso de **contato**:<br />Contacts.ReadWrite |

> **Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão de aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário. Para saber mais, veja como [obter acesso sem um usuário conectado](/graph/auth-v2-service).

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
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
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
    "Error: /api-reference/beta/api/profilephoto-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
