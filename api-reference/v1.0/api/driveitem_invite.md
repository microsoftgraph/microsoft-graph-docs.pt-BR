---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
ms.openlocfilehash: c68289049503e70e04b2e403ca09cfc1f67e4096
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268729"
---
# <a name="send-a-sharing-invitation"></a>Enviar um convite de compartilhamento

Envia um convite de compartilhamento para um **DriveItem**.
Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email com um [link de compartilhamento][].

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

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
| mensagem          | Sequência de caracteres                         | Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.
| requireSignIn    | Booleano                        | Especifica se o destinatário do convite precisa entrar para exibir o item compartilhado.
| sendInvitation   | Booleano                        | Se verdadeiro, um [link de compartilhamento][] é enviado ao destinatário. Caso contrário, uma permissão é concedida diretamente, sem o envio de uma notificação.
| funções            | Collection(String)             | Especifique as funções que serão concedidas aos destinatários do convite de compartilhamento.

## <a name="example"></a>Exemplo

Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.com" com uma mensagem sobre um arquivo no qual ele está colaborando.
O convite concede acesso de leitura e gravação ao arquivo para Ryan.

### <a name="http-request"></a>Solicitação HTTP

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.

<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
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
  "roles": [ "write" ]
}
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a>Comentários

* [Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.
* Para obter uma lista das funções disponíveis, consulte [Funções de enumeração](../resources/permission.md#roles-enumeration).

## <a name="error-responses"></a>Respostas de erro

Saiba mais sobre como os erros são retornados no tópico [Respostas de erro][error-response].


[driveRecipient]: ../resources/driverecipient.md
[error-response]: ../../../concepts/errors.md
[link de compartilhamento]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
