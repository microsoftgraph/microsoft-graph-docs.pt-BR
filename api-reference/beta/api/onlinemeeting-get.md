---
title: Obter onlineMeeting
description: Recupere as propriedades e as relações de um objeto onlineMeeting.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6c87a2357674f50d281bafe8a9fc3661ee0dae5a
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645502"
---
# <a name="get-onlinemeeting"></a>Obter onlineMeeting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere as propriedades e as relações de um [objeto onlineMeeting](../resources/onlinemeeting.md) .

Por exemplo, você pode:

- Obtenha detalhes de um onlineMeeting usando [videoTeleconferenceId](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid), [ID](#example-2-retrieve-an-online-meeting-by-meeting-id) de reunião, [joinWebURL](#example-3-retrieve-an-online-meeting-by-joinweburl) ou [joinMeetingId](#example-4-retrieve-an-online-meeting-by-joinmeetingid).
- Use o `/attendeeReport` caminho para obter o relatório de participantes de um evento ao vivo do [Microsoft Teams](/microsoftteams/teams-live-events/what-are-teams-live-events) na forma de um link de download, conforme mostrado no [exemplo 5](#example-5-fetch-the-attendee-report-of-a-teams-live-event).
- Use o `/recording` e os `/alternativeRecording` caminhos para obter as gravações de um evento ao vivo do [Teams](/microsoftteams/teams-live-events/what-are-teams-live-events) na forma de um link de download, conforme mostrado no [exemplo 6](#example-6-fetch-the-recording-of-a-teams-live-event).

O relatório de participantes do evento ao vivo do Teams e as gravações de eventos ao vivo do Teams são artefatos de reunião online. Para obter detalhes, consulte [artefatos e permissões](/graph/cloud-communications-online-meeting-artifacts) de reunião online.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                            |
|:---------------------------------------|:---------------------------------------------------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | OnlineMeetingArtifact.Read.All, OnlineMeetings.Read, OnlineMeetings.ReadWrite          |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                                         |
| Aplicativo                            | OnlineMeetingArtifact.Read.All, OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All  |

Para usar a permissão do aplicativo para essa API, os administradores de [](/graph/cloud-communication-online-meeting-application-access-policy) locatários devem criar uma política de acesso de aplicativo e concedi-la a um usuário para autorizar o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID de usuário especificada no caminho da solicitação).

> [!CAUTION]
> Somente as _permissões OnlineMeetingArtifact.Read.All_ serão necessárias se você buscar artefatos de reunião online. Você ainda pode buscar artefatos de reunião sem eles até **15 de janeiro de 2022**. Para obter detalhes, consulte [artefatos e permissões](/graph/cloud-communications-online-meeting-artifacts) de reunião online.

## <a name="http-request"></a>Solicitação HTTP

Para obter uma **reunião online usando a** ID da reunião com permissão delegada (`/me`) e de aplicativo (`/users/{userId}`):
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}
GET /users/{userId}/onlineMeetings/{meetingId}
```
Essas URLs de solicitação aceitam o token de usuário do organizador e do participante convidado (permissão delegada) ou a ID de usuário (permissão do aplicativo).

Para obter um **onlineMeeting usando** **videoTeleconferenceId** com permissão de aplicativo:
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{videoTeleconferenceId}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{videoTeleconferenceId}'
```

Para obter um **onlineMeeting usando** **joinWebUrl** com permissão delegada (`/me`) e de aplicativo (`/users/{userId}`):
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings?$filter=JoinWebUrl%20eq%20'{joinWebUrl}'
GET /users/{userId}/onlineMeetings?$filter=JoinWebUrl%20eq%20'{joinWebUrl}'
```

Para obter uma **onlineMeeting usando** **joinMeetingId** com permissão delegada (`/me`) e de aplicativo (`/users/{userId}`):
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings?$filter=joinMeetingIdSettings/joinMeetingId%20eq%20'{joinMeetingId}'
GET /users/{userId}/onlineMeetings?$filter=joinMeetingIdSettings/joinMeetingId%20eq%20'{joinMeetingId}'
```

Para obter o relatório do participante de um [evento ao vivo do Teams](/microsoftteams/teams-live-events/what-are-teams-live-events) com permissão delegada (`/me`) e de aplicativo (`/users/{userId}`):
<!-- { "blockType": "ignored" }-->

```http
GET /me/onlineMeetings/{meetingId}/attendeeReport
GET /users/{userId}/onlineMeetings/{meetingId}/attendeeReport
```

Para obter as gravações de um evento ao [vivo do Teams](/microsoftteams/teams-live-events/what-are-teams-live-events) com permissão delegada (`/me`) e de aplicativo (`/users/{userId}`):
<!-- { "blockType": "ignored" }-->

```http
GET /me/onlineMeetings/{meetingId}/recording
GET /me/onlineMeetings/{meetingId}/alternativeRecording
GET /users/{userId}/onlineMeetings/{meetingId}/recording
GET /users/{userId}/onlineMeetings/{meetingId}/alternativeRecording
```

> [!NOTE]
>- O caminho `/app` foi preterido. Daqui em diante, use o caminho `/communications`.
>- `userId` é a ID de objeto de um usuário no [Portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Para obter mais detalhes, consulte [Permitir que os aplicativos acessem reuniões online em nome de um usuário](/graph/cloud-communication-online-meeting-application-access-policy).
>- `meetingId` é a **ID de** um [objeto onlineMeeting](../resources/onlinemeeting.md) .
> - **videoTeleconferenceId** é gerado para usuários licenciados do Cloud-Video-Interop e pode ser encontrado em um [objeto onlineMeeting](../resources/onlinemeeting.md) . Para obter detalhes, consulte [a ID de conferência do VTC](/microsoftteams/cloud-video-interop-for-teams-set-up).
>- `joinWebUrl` deve ser codificado por URL.
>- `joinMeetingId` é a ID da reunião a ser usada para ingressar em uma reunião.

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |
| Accept-Language | Idioma. Opcional.       |

Se a solicitação contiver um `Accept-Language`cabeçalho HTTP, o `content` de `joinInformation` estará na variante de idioma e código de idioma especificada `Accept-Language` no cabeçalho. O conteúdo padrão será em inglês.

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `200 OK`. A resposta também inclui um dos seguintes:

- Se você buscar uma reunião online por ID de reunião, esse método retornará um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.
- Se você buscar uma reunião online por **videoTeleconferenceId** ou **joinWebUrl**, esse método retornará uma coleção que contém apenas um objeto [onlineMeeting](../resources/onlinemeeting.md) no corpo da resposta.
- Se você buscar o relatório de participação de uma reunião online, esse método retornará um objeto [meetingAttendanceReport](../resources/meetingAttendanceReport.md) no corpo da resposta.
- Se você buscar o relatório do participante ou a gravação de um Evento ao Vivo do **Microsoft Teams**, `Location` esse método retornará um cabeçalho que indica o URI para o relatório ou gravação do participante, respectivamente.

> [!NOTE]
>- **JoinMeetingIdSettings** pode não ser gerado para algumas reuniões pré-agendadas se a reunião tiver sido criada antes do suporte a esse recurso.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-an-online-meeting-by-videoteleconferenceid"></a>Exemplo 1: Recuperar uma reunião online por videoTeleconferenceId

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["123456789"],
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-onlinemeeting-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-onlinemeeting-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "55534478",
    "tollFreeNumber": "55390588",
    "ConferenceId": "9999999",
    "dialinUrl": "https://dialin.teams.microsoft.com/6787A136-B9B8-4D39-846C-C0F1FF937F10?id=xxxxxxx"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c868258e3cebf7bee0d@thread.skype",
    "messageId": "153867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa674c-875-432d-bd41-3720e0a%22%2c%22Oid%22%3a%2f7296-5fa4-42ca-bae8-6a4b8%22%7d",
  "participants": {
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "11296-5fa4-42ca-bae8-6a2b4b8",
            "tenantId": "aa674c-8475-432d-bd41-39f2e0a",
            "displayName": "Tyler Stein"
          }
        },
        "upn": "upn-value",
        "role": "attendee"
      }
    ],
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "58ede-f3cc-42eb-b2c1-e53ec96",
          "tenantId": "a7bdc-8475-432d-bd41-39f2e0a",
          "displayName": "Jasmine Miller"
        }
      },
      "upn": "upn-value",
      "role": "presenter"
    }
  },
  "startDateTime": "2018-05-30T00:30:00Z",
  "subject": "Test Meeting.",
  "videoTeleconferenceId": "123456789",
  "lobbyBypassSettings": {
    "scope": "everyone",
    "isDialInBypassEnabled": true
  },
  "joinMeetingIdSettings": {
    "isPasscodeRequired": false,
    "joinMeetingId": "1234567890",
    "passcode": null
  },
  "isEntryExitAnnounced": true,
  "allowedPresenters": "everyone",
  "allowMeetingChat": "enabled",
  "allowTeamworkReactions": true
}
```
>**Observação:** Se 'Accept-Language: ja' for especificado para indicar japonês, por exemplo, a resposta incluirá o seguinte.

```json
    "joinInformation": {
        "content": "data%3Atext%2Fhtml%2C%0A++%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A%09+%3C%2Fdiv%3E%0A++++%3Cdiv+class%3D%22me-email-text%22+style%3D%22color%3A%23252424%3Bfont-family%3A'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3B%22%3E%0A+++%3Cdiv+style%3D%22margin-top%3A+24px%3B+margin-bottom%3A+10px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-headline%22%0A++++++++++++++style%3D%22font-size%3A+18px%3Bfont-family%3A'Segoe+UI+Semibold'%2C'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3Btext-decoration%3A+underline%3Bcolor%3A+%236264a7%3B%22%0A++++++++++++++href%3D%22https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%252279a788bf-86f1-41af-91ab-000000000000%2522%252c%2522Oid%2522%253a%2522d4a060b5-a8fc-450c-837b-000000000000%2522%257d%22%0A++++++++++++++target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3EMicrosoft+Teams+%E4%BC%9A%E8%AD%B0%E3%81%AB%E5%8F%82%E5%8A%A0%3C%2Fa%3E%0A++++++%3C%2Fdiv%3E%0A%09+%3Cdiv%3E%0A++++%0A++++++%3Cdiv%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+14px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22%0A++++++++++href%3D%22tel%3A%2B16477490000%2C%2C11160000%26%2335%3B+%22+target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3E%2B16477490000%3C%2Fa%3E%0A++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%26nbsp%3B++(%E6%9C%89%E6%96%99)+%3C%2Fspan%3E%0A++++++%3C%2Fdiv%3E%0A++++%0A++%3C%2Fdiv%3E%0A%0A%09+%0A++++++%3Cdiv+style%3D%22margin-top%3A+10px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++++++%E4%BC%9A%E8%AD%B0+ID%3A%0A++++++++%3C%2Fspan%3E%0A++++++%3Cspan+style%3D%22font-size%3A+14px%3B%22%3E%0A++++++++111+000+00%23%0A++++++%3C%2Fspan%3E%0A++++%3C%2Fdiv%3E%0A++++%0A%09+%0A++++++++%3Cdiv+style%3D%22margin-bottom%3A+24px%3B%22%3E%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fdialin.teams.microsoft.com%2F8bf6e654-57eb-4b85-aeaf-36c84429b2fe%3Fid%3D11160000%22+rel%3D%22noreferrer+noopener%22%3E%E6%9C%80%E5%AF%84%E3%82%8A%E3%81%AE%E5%9B%BD%E3%81%AE%E9%9B%BB%E8%A9%B1%E7%95%AA%E5%8F%B7%E3%82%92%E6%A4%9C%E7%B4%A2%3C%2Fa%3E%0A+++++++++%7C%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fmysettings.lync.com%2Fpstnconferencing%22+rel%3D%22noreferrer+noopener%22%3E%0A++++++++PIN+%E3%82%92%E3%83%AA%E3%82%BB%E3%83%83%E3%83%88%3C%2Fa%3E%0A+++++++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Faka.ms%2FJoinTeamsMeeting%22+rel%3D%22noreferrer+noopener%22%3ETeams+%E3%81%AE%E8%A9%B3%E7%B4%B0%E3%82%92%E8%A1%A8%E7%A4%BA%3C%2Fa%3E%0A+++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fteams.microsoft.com%2FmeetingOptions%2F%3ForganizerId%3Dd4a060b5-a8fc-450c-837b-000000000000%26tenantId%3D79a788bf-86f1-41af-91ab-000000000000%26threadId%3D19_meeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%40thread.v2%26messageId%3D0%26language%3Dja%22+rel%3D%22noreferrer+noopener%22%3E%E4%BC%9A%E8%AD%B0%E3%81%AE%E3%82%AA%E3%83%97%E3%82%B7%E3%83%A7%E3%83%B3%3C%2Fa%3E%0A++++%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%E3%83%93%E3%83%87%E3%82%AA%E4%BC%9A%E8%AD%B0%E3%83%87%E3%83%90%E3%82%A4%E3%82%B9%E3%81%A7%E5%8F%82%E5%8A%A0%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A12px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22%22%3E000000000%40t.abcd.vc%3C%2Fa%3E+VTC+%E4%BC%9A%E8%AD%B0+ID%3A+0180300000%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A+12px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22https%3A%2F%2Fdialin.abcd.vc%2Fteams%2F%3Fkey%3D000000000%26conf%3D0180308922%22%3E%E4%BB%A3%E6%9B%BF+VTC+%E3%81%AE%E3%83%80%E3%82%A4%E3%83%A4%E3%83%AB%E6%96%B9%E6%B3%95%3C%2Fa%3E%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++%0A++++++%3C%2Fdiv%3E%0A++++++%3Cdiv+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++%0A++++++%3C%2Fdiv%3E%0A++++%0A+++++%3C%2Fdiv%3E%0A%09+%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A++%3C%2Fdiv%3E%22%2C%0A",
        "contentType": "Html"
    }  
```

### <a name="example-2-retrieve-an-online-meeting-by-meeting-id"></a>Exemplo 2: Recuperar uma reunião online por ID de reunião
Você pode recuperar informações de reunião por meio da ID de reunião com um token de usuário ou de aplicativo. A ID da reunião é fornecida no objeto de resposta ao criar um [onlineMeeting](../resources/onlinemeeting.md). Essa opção está disponível para dar suporte a casos de uso em que a ID da reunião é conhecida, como quando um aplicativo cria a reunião online pela primeira vez usando o API do Graph e, em seguida, recupera informações de reunião posteriormente como uma ação separada.

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

> **Nota:** A ID da reunião foi truncada para legibilidade.

A solicitação a seguir usa um token de usuário.
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy
```

A solicitação a seguir usa um token de aplicativo.
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 

```json
{
    "id": "MSpkYzE3Njc0Yy04MWQ5L1F6WGhyZWFkLnYy",
    "creationDateTime": "2020-09-29T22:35:33.1594516Z",
    "startDateTime": "2020-09-29T22:35:31.389759Z",
    "endDateTime": "2020-09-29T23:35:31.389759Z",
    "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4YxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22c581-5130-43e9-88f3-fc82cde37%22%2c%22Oid%22%3a%22674c-81d9-4adb-bb2-8f62e4622%22%7d",
    "subject": null,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "allowMeetingChat": "enabled",
    "allowTeamworkReactions": true,
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc174c-81d9-4adb-bfb2-8f4622",
                    "displayName": null,
                    "tenantId": "9081-5130-43e9-88f3-fcde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    },
    "joinMeetingIdSettings": {
        "isPasscodeRequired": false,
        "joinMeetingId": "1234567890",
        "passcode": null
    }
}
```

### <a name="example-3-retrieve-an-online-meeting-by-joinweburl"></a>Exemplo 3: Recuperar uma reunião online por joinWebUrl
Você pode recuperar informações de reunião por meio do JoinWebUrl usando um token de usuário ou aplicativo. Essa opção está disponível para dar suporte a casos de uso em que a ID da reunião não é conhecida, mas o JoinWebUrl é, como quando um usuário cria uma reunião (por exemplo, no cliente do Microsoft Teams) e um aplicativo separado precisa recuperar detalhes da reunião como uma ação de acompanhamento.

#### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.

A solicitação a seguir usa um token de usuário.
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings?$filter=JoinWebUrl%20eq%20'https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%2522909c6581-5130-43e9-88f3-fcb3582cde37%2522%252c%2522Oid%2522%253a%2522dc17674c-81d9-4adb-bfb2-8f6a442e4622%2522%257d'
```

A solicitação a seguir usa um token de aplicativo.
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings?$filter=JoinWebUrl%20eq%20'https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%2522909c6581-5130-43e9-88f3-fcb3582cde37%2522%252c%2522Oid%2522%253a%2522dc17674c-81d9-4adb-bfb2-8f6a442e4622%2522%257d'
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 

```json
{
    "value": [
        {
            "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_MGQ4MDQyEtZWVkODYxODYzMmY2@thread.v2",
            "creationDateTime": "2020-09-29T22:35:33.1594516Z",
            "startDateTime": "2020-09-29T22:35:31.389759Z",
            "endDateTime": "2020-09-29T23:35:31.389759Z",
            "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2N2%40thread.v2/0?context=%7b%22Tid%22%3a%229581-5130-43e9-8f3-fcb35e37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
            "subject": null,
            "autoAdmittedUsers": "EveryoneInCompany",
            "isEntryExitAnnounced": true,
            "allowedPresenters": "everyone",
            "allowMeetingChat": "enabled",
            "allowTeamworkReactions": true,
            "videoTeleconferenceId": "(redacted)",
            "participants": {
                "organizer": {
                    "upn": "(redacted)",
                    "role": "presenter",
                    "identity": {
                        "user": {
                            "id": "dc4c-81d9-4adb-bfb2-8f4622",
                            "displayName": null,
                            "tenantId": "9091-5130-43e9-88f3-fcbe38",
                            "identityProvider": "AAD"
                        }
                    }
                },
                "attendees": [],
                "producers": [],
                "contributors": []
            },
            "lobbyBypassSettings": {
                "scope": "organization",
                "isDialInBypassEnabled": false
            },
            "joinMeetingIdSettings": {
                "isPasscodeRequired": false,
                "joinMeetingId": "1234567890",
                "passcode": null
            }
        }
    ]
}
```

### <a name="example-4-retrieve-an-online-meeting-by-joinmeetingid"></a>Exemplo 4: Recuperar uma reunião online por joinMeetingId
Você pode recuperar informações de reunião por meio **do joinMeetingId** usando um usuário ou um token de aplicativo.

#### <a name="request"></a>Solicitação

A solicitação a seguir usa um token de usuário.
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings?$filter=joinMeetingIdSettings/joinMeetingId%20eq%20'1234567890'
```

A solicitação a seguir usa um token de aplicativo.
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings?$filter=joinMeetingIdSettings/joinMeetingId%20eq%20'1234567890'
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 

```json
{
    "value": [
        {
            "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622_19:meeting_MGQ4MDQyNTLTlkM2EtZWVkODYxODYzMmY2@thread.v2",
            "creationDateTime": "2020-09-29T22:35:33.1594516Z",
            "startDateTime": "2020-09-29T22:35:31.389759Z",
            "endDateTime": "2020-09-29T23:35:31.389759Z",
            "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTM2EtZWVkODYxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
            "subject": null,
            "autoAdmittedUsers": "EveryoneInCompany",
            "isEntryExitAnnounced": true,
            "allowedPresenters": "everyone",
            "allowMeetingChat": "enabled",
            "allowTeamworkReactions": true,
            "videoTeleconferenceId": "(redacted)",
            "participants": {
                "organizer": {
                    "upn": "(redacted)",
                    "role": "presenter",
                    "identity": {
                        "user": {
                            "id": "dc174c-81d9-4adb-bfb2-8f6622",
                            "displayName": null,
                            "tenantId": "9091-5130-43e9-88f3-fce38",
                            "identityProvider": "AAD"
                        }
                    }
                },
                "attendees": [],
                "producers": [],
                "contributors": []
            },
            "lobbyBypassSettings": {
                "scope": "organization",
                "isDialInBypassEnabled": false
            },
            "joinMeetingIdSettings": {
                "isPasscodeRequired": false,
                "joinMeetingId": "1234567890",
                "passcode": null
            }
        }
    ]
}
```

### <a name="example-5-fetch-the-attendee-report-of-a-teams-live-event"></a>Exemplo 5: Buscar o relatório de participante de um evento ao vivo do Teams

O exemplo a seguir mostra uma solicitação para baixar um relatório de participantes.

#### <a name="request"></a>Solicitação

A solicitação a seguir usa a permissão delegada.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attendee_report"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/attendeeReport
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendee-report-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendee-report-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendee-report-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendee-report-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-attendee-report-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-attendee-report-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


A solicitação a seguir usa a permissão do aplicativo.

<!-- { "blockType": "ignored" }-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/attendeeReport
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_attendee_report"
} -->

```http
HTTP/1.1 302 Found
Location: https://01-a-noam.dog.attend.teams.microsoft.com/broadcast/909c6581-5130-43e9-88f3-fcb3582cde37/dc17674c-81d9-4adb-bfb2-8f6a442e4622/19%3Ameeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw%40thread.v2/0/resource/attendeeReport
```

### <a name="example-6-fetch-the-recording-of-a-teams-live-event"></a>Exemplo 6: Buscar a gravação de um evento ao vivo do Teams

O exemplo a seguir mostra uma solicitação para baixar uma gravação.

#### <a name="request"></a>Solicitação

A solicitação a seguir usa a permissão delegada.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_live_event_recording"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/recording
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-live-event-recording-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-live-event-recording-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-live-event-recording-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-live-event-recording-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-live-event-recording-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-live-event-recording-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


A solicitação a seguir usa a permissão do aplicativo.
<!-- { "blockType": "ignored" }-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/recording
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_live_event_recording"
} -->

```http
HTTP/1.1 302 Found
Location: https://01-a-noam.dog.attend.teams.microsoft.com/broadcast/909c6581-5130-43e9-88f3-fcb3582cde37/dc17674c-81d9-4adb-bfb2-8f6a442e4622/19%3Ameeting_ZWE0YzQwMzItYjEyNi00NjJjLWE4MjYtOTUxYjE1NmFjYWIw%40thread.v2/0/resource/recording
```
