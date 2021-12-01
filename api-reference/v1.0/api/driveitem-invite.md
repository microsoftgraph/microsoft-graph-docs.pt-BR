---
author: JeremyKelley
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
ms.localizationpriority: medium
ms.prod: sharepoint
description: Envia um convite de compartilhamento para um driveItem.
doc_type: apiPageType
ms.openlocfilehash: 0ce6f6751d206571a2d55f31e6e90fcb635df4c2
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61241271"
---
# <a name="send-a-sharing-invitation"></a>Enviar um convite de compartilhamento

Namespace: microsoft.graph

Envia um convite de compartilhamento para **um driveItem**.
Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email com um [link de compartilhamento][].

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| Parâmetro        | Tipo                           | Descrição
|:-----------------|:-------------------------------|:-------------------------
| destinatários       | Collection([DriveRecipient][]) | Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.
| mensagem          | String                         | Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.
| requireSignIn    | Booleano                        | Especifica se o destinatário do convite precisa fazer logon para visualizar o item compartilhado.
| sendInvitation   | Booliano                        | Se verdadeiro, um [link de compartilhamento][] será enviado ao destinatário. Caso contrário, uma permissão é concedida diretamente sem enviar uma notificação.
| funções            | Collection(String)             | Especifique as funções que devem ser concedidas aos destinatários do convite de compartilhamento.
| expirationDateTime | DateTimeOffset                       | Especifique o DateTime após o qual a permissão expira. Disponível em OneDrive for Business, SharePoint e contas de OneDrive pessoais premium.
| password           | String                         | A senha definida no convite pelo criador. Opcional e OneDrive somente pessoal.

## <a name="example"></a>Exemplo

Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.com" com uma mensagem sobre um arquivo recebendo colaborações. O convite concede acesso de leitura e gravação ao arquivo para Ryan.

### <a name="http-request"></a>Solicitação HTTP

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@deprecated.GrantedTo": "GrantedTo has been deprecated. Refer to GrantedToV2",
      "grantedTo": {
        "user": {
          "displayName": "Robin Danielsen",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "grantedToV2": {
        "user": {
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20",
          "displayName": "Robin Danielsen"
        },
        "siteUser": {
          "id": "1",
          "displayName": "Robin Danielsen",
          "loginName": "Robin Danielsen"
        }
      },
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "robin@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```

## <a name="remarks"></a>Comentários

* [Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.
* Para ver uma lista de funções disponíveis, consulte [roles property values](../resources/permission.md#roles-property-values).

## <a name="error-responses"></a>Respostas de erro

Leia o tópico [Respostas de Erro][error-response] para obter mais informações sobre como os erros são retornados.


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[link de compartilhamento]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
} -->

