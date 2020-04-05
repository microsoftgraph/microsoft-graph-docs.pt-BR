---
author: JeremyKelley
description: Envia um convite de compartilhamento para um DriveItem.
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 594df009c38ff1d7384207e7486392f24d7a8dbd
ms.sourcegitcommit: 6db0b7a473594653dda332ce7da45ea2ad90772b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43146398"
---
# <a name="send-a-sharing-invitation"></a>Enviar um convite de compartilhamento

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Envia um convite de compartilhamento para um **DriveItem**. Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email aos destinatários para notificá-los de que o item foi compartilhado.

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

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

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

| Parâmetro        | Tipo                                            | Descrição                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| destinatários       | Collection([DriveRecipient](../resources/driverecipient.md)) | Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.                                            |
| mensagem          | String                                          | Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres. |
| requireSignIn    | Booleano                                         | Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.            |
| sendInvitation   | Booliano                                         | Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).            |
| funções            | Collection(String)                              | Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.                         |
| expirationDateTime | DateTimeOffset                       | Especifique o DateTime após o qual a permissão expira. Disponível em contas pessoais do OneDrive para o OneDrive for Business, SharePoint e Premium.
| password           | String                         | A senha definida no convite pelo criador. Opcional e o OneDrive somente pessoal

## <a name="example"></a>Exemplo

Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.org" com uma mensagem sobre um arquivo no qual ele está colaborando.
O convite concede acesso de leitura e gravação ao arquivo para Ryan.

### <a name="http-request"></a>Solicitação HTTP

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
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

---


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
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="partial-success-response"></a>Resposta parcial com êxito

Ao convidar vários destinatários, é possível que a notificação tenha êxito em alguns e falha para outras pessoas.
Nesse caso, o serviço retorna uma resposta de êxito parcial com um código de status HTTP 207.
Quando o sucesso parcial for retornado, a resposta para cada destinatário com falha conterá um `error` objeto com informações sobre o que deu errado e como corrigi-lo.

Veja um exemplo da resposta parcial.  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
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
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a>Erros do SendNotification
A seguir estão alguns erros adicionais que seu aplicativo pode encontrar nos objetos aninhados `innererror` ao enviar uma notificação falha. Os aplicativos não são necessários para lidar com eles.

| Código                           | Descrição
|:-------------------------------|:--------------------------------------------------------------------------------------
| accountVerificationRequired    | A verificação da conta é necessária para desbloquear o envio de notificações.
| hipCheckRequired               | É necessário resolver a verificação HIP (Host Intrusion Prevention) para desbloquear o envio de notificações.
| exchangeInvalidUser            | A caixa de correio do usuário atual não foi encontrada.
| exchangeOutOfMailboxQuota      | Fora da cota.
| exchangeMaxRecipients          | Foi excedido o número máximo de destinatários que podem receber notificações ao mesmo tempo.

>**Observação:** O serviço pode adicionar novos códigos de erro ou parar de retornar os antigos a qualquer momento.

## <a name="remarks"></a>Comentários

* [Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.
* Para obter uma lista de funções disponíveis, consulte [funções valores de propriedade](../resources/permission.md#roles-property-values).

## <a name="error-responses"></a>Respostas de erro

Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
}
-->
