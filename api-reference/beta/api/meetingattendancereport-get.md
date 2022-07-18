---
title: Obter meetingAttendanceReport
description: Obtenha o relatório de participação de uma reunião online.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 684e4cdd80c74c11d4118aa769bf15882d94ed4d
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704470"
---
# <a name="get-meetingattendancereport"></a>Obter meetingAttendanceReport

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha [o meetingAttendanceReport](../resources/meetingAttendanceReport.md) para um [onlineMeeting](../resources/onlinemeeting.md). Sempre que uma reunião online terminar, um relatório de participação será gerado para essa sessão.

> [!WARNING]
> Esse método não dá suporte a reuniões de canal.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetingArtifact.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application | OnlineMeetingArtifact.Read.All |

Para usar a permissão de aplicativo para essa API, os administradores de locatários devem criar uma política de acesso de aplicativo e concedi-la a um usuário. Isso autoriza o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID de usuário especificada no caminho da solicitação). Para obter mais detalhes, consulte [Permitir que os aplicativos acessem reuniões online em nome de um usuário](/graph/cloud-communication-online-meeting-application-access-policy).

## <a name="http-request"></a>Solicitação HTTP

Para obter um relatório de presença por ID com permissão delegada (`/me`) e de aplicativo (`/users/{userId}`):
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}/attendanceReports/{reportId}
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports/{reportId}
```

Para obter o relatório de participação da sessão mais recente de uma reunião online com permissão delegada (`/me`) e de aplicativo (`/users/{userId}`):
<!-- { "blockType": "ignored" }-->
```http
GET /me/onlineMeetings/{meetingId}/meetingAttendanceReport
GET /users/{userId}/onlineMeetings/{meetingId}/meetingAttendanceReport
```

> [!TIP]
>
>- `userId` é a ID de objeto de um usuário no [Portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Para obter mais detalhes, consulte [Permitir que os aplicativos acessem reuniões online em nome de um usuário](/graph/cloud-communication-online-meeting-application-access-policy).
>- `meetingId` é a **ID de** um [objeto onlineMeeting](../resources/onlinemeeting.md) .
>- `reportId` é a **ID de** um [objeto meetingAttendanceReport](../resources/meetingAttendanceReport.md) .

> [!CAUTION]
>
>- O caminho `/meetingAttendanceReport` foi preterido. No futuro, use o caminho `/attendanceReports` para recuperar relatórios de participação para uma reunião online.
>- O `/meetingAttendanceReport` caminho permanecerá em beta para compatibilidade com versões anteriores. No entanto, para obter a mesma resposta, você precisa adicionar a opção `expand` de consulta. Para obter detalhes, consulte [a seção Parâmetros de consulta](#optional-query-parameters) opcional.

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

> [!TIP]
> A **propriedade attendanceRecords** é uma propriedade de navegação que não é retornada por padrão. Para recuperar **attendanceRecords** na linha, use `$expand=attendanceRecords` a opção de consulta, conforme mostrado no [exemplo 2](#example-2-get-the-latest-attendance-report-for-an-online-meeting).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um [objeto meetingAttendanceReport](../resources/meetingAttendanceReport.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="example-1-get-the-attendance-report-for-an-online-meeting-by-id"></a>Exemplo 1: Obter o relatório de presença de uma reunião online por ID

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get-attendanceReport-by-id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports/2c2c2454-7613-4d6e-9c7c-4cf7a6cdce89?$expand=attendanceRecords
```

#### <a name="response"></a>Resposta

> **Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.

<!-- {
  "blockType": "response",
  "name": "get-attendanceReport-by-id",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('16664f75-11dc-4870-bec6-38c1aaa81431')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ')/attendanceReports('c9b6db1c-d5eb-427d-a5c0-20088d9b22d7')",
  "id": "c9b6db1c-d5eb-427d-a5c0-20088d9b22d7",
  "totalParticipantCount": 1,
  "meetingStartDateTime": "2021-10-05T04:38:23.945Z",
  "meetingEndDateTime": "2021-10-05T04:43:49.77Z",
  "attendanceRecords": [
    {
      "emailAddress": "(email address)",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "(redacted)",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:52.2782182Z",
          "leaveDateTime": "2021-03-16T19:06:47.7218491Z",
          "durationInSeconds": 415
        },
        {
          "joinDateTime": "2021-03-16T19:09:23.9834702Z",
          "leaveDateTime": "2021-03-16T19:16:31.1381195Z",
          "durationInSeconds": 427
        },
        {
          "joinDateTime": "2021-03-16T19:20:27.7094382Z",
          "leaveDateTime": "2021-03-16T19:25:37.7121956Z",
          "durationInSeconds": 310
        }
      ]
    }
  ]
}
```

### <a name="example-2-get-the-latest-attendance-report-for-an-online-meeting"></a>Exemplo 2: Obter o relatório de participação mais recente de uma reunião online

O exemplo a seguir mostra uma solicitação para obter um relatório de presença de reunião para a sessão mais recente de uma reunião online.

#### <a name="request"></a>Solicitação

A solicitação a seguir usa a permissão delegada.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_attendance_report"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-attendance-report-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-attendance-report-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-attendance-report-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-attendance-report-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-attendance-report-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-attendancereport-by-id-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

A solicitação a seguir usa a permissão do aplicativo.
<!-- { "blockType": "ignored" }-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/dc74d9bb-6afe-433d-8eaa-e39d80d3a647/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy/meetingAttendanceReport
```

#### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingAttendanceReport",
  "name": "get_attendance_report"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('dc74d9bb-6afe-433d-8eaa-e39d80d3a647')/onlineMeetings('MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy')/meetingAttendanceReport/$entity",
  "attendanceRecords": [
    {
      "emailAddress": "email address",
      "totalAttendanceInSeconds": 1558,
      "role": "Organizer",
      "identity": {
        "id": "dc74d9bb-6afe-433d-8eaa-e39d80d3a647",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:46.598956Z",
          "leaveDateTime": "2021-03-16T19:25:45.4473057Z",
          "durationInSeconds": 1558
        }
      ]
    },
    {
      "emailAddress": "email address",
      "totalAttendanceInSeconds": 1152,
      "role": "Presenter",
      "identity": {
        "id": "(redacted)",
        "displayName": "(redacted)",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-03-16T18:59:52.2782182Z",
          "leaveDateTime": "2021-03-16T19:06:47.7218491Z",
          "durationInSeconds": 415
        },
        {
          "joinDateTime": "2021-03-16T19:09:23.9834702Z",
          "leaveDateTime": "2021-03-16T19:16:31.1381195Z",
          "durationInSeconds": 427
        },
        {
          "joinDateTime": "2021-03-16T19:20:27.7094382Z",
          "leaveDateTime": "2021-03-16T19:25:37.7121956Z",
          "durationInSeconds": 310
        }
      ]
    }
  ],
  "totalParticipantCount": 2
}
```
