---
title: Atualizar onlineMeeting
description: Atualize as propriedades de uma reunião online.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d7579a29132a3f122d525b81ab04f7d3fa49b6e8
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870048"
---
# <a name="update-onlinemeeting"></a>Atualizar onlineMeeting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do objeto [onlineMeeting](../resources/onlinemeeting.md) especificado.

Consulte [a seção Solicitar corpo](#request-body) para a lista de propriedades que suportam a atualização.

## <a name="permissions"></a>Permissões

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | OnlineMeetings.ReadWrite                    |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | OnlineMeetings.ReadWrite.All*                |

> [!IMPORTANT]
> \*Os administradores [](/graph/cloud-communication-online-meeting-application-access-policy) devem criar uma política de acesso a aplicativos e concedi-la a um usuário, autorizando o aplicativo configurado na política para atualizar uma reunião online em nome desse usuário (ID do usuário especificada no caminho da solicitação).

## <a name="http-request"></a>Solicitação HTTP
Para atualizar o onlineMeeting especificado por meio da ID de reunião com o token delegado:
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

Para atualizar o onlineMeeting especificado pela ID de reunião com o token de aplicativo:
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
> - `userId`é a ID do objeto de um usuário no portal de gerenciamento [de usuários do Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade) Para obter mais detalhes, consulte [política de acesso ao aplicativo](/graph/cloud-communication-online-meeting-application-access-policy).
> - `meetingId`é a **id** de um [objeto onlineMeeting.](../resources/onlinemeeting.md)

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
A tabela abaixo lista as propriedades que podem ser atualizadas. No corpo da solicitação, inclua apenas as propriedades que precisam ser atualizadas, com as seguintes exceções:

- Ajustar a data/hora inicial ou final de uma reunião online sempre requer as propriedades **startDateTime** e **endDateTime** no corpo da solicitação.
- Ajustar o **campo de** participantes  da propriedade participantes, como adicionar ou remover um participante à reunião, sempre requer a lista completa de participantes no corpo da solicitação.

| Propriedade             | Tipo                                                         | Descrição                                                                                                                                    |
|----------------------|--------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| startDateTime        | DateTime                                                     | O horário de início da reunião em UTC.                                                                                                                 |
| endDateTime          | DateTime                                                     | A hora de término da reunião em UTC.                                                                                                                   |
| assunto              | Cadeia de caracteres                                                       | O assunto da reunião online.                                                                                                             |
| participants         | [meetingParticipants](../resources/meetingparticipants.md)   | Os participantes associados à reunião online. Isso inclui o organizador e os participantes.                                            |
| isEntryExitAnnounced | Boolean                                                      | Se os chamadores ingressarão ou sairão.                                                                                         |
| lobbyBypassSettings  | [lobbyBypassSettings](../resources/lobbyBypassSettings.md)   | Especifica quais participantes podem ignorar o lobby da reunião.                                                                                     |
| allowedPresenters    | onlineMeetingPresenters                                      | Especifica quem pode ser um apresentador em uma reunião. Os valores possíveis são todos, organização, roleIsPresenter, organizador e unknownFutureValue. |

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a>Exemplo 1: atualizar o startDateTime, endDateTime e assunto

#### <a name="request"></a>Solicitação

> **Observação:** A ID da reunião foi truncada para capacidade de leitura.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "role": "presenter",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"+1-900-555-0100",
      "tollFreeNumber":"+1-800-555-0100",
      "dialinUrl":"url"
   }
}
```

#### <a name="example-2-update-the-lobbybypasssettings"></a>Exemplo 2: atualizar o lobbyBypassSettings
> **Observação:** A ID da reunião foi truncada para capacidade de leitura.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
    "creationDateTime":"2020-07-03T00:23:39.444642Z",
    "startDateTime":"2020-09-09T21:33:30.8546353Z",
    "endDateTime":"2020-09-09T22:03:30.8566356Z",
    "joinWebUrl":"(redacted)",
    "subject":"Patch Meeting Subject",
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                    "displayName": null,
                    "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


