---
title: Listar attendanceRecords
description: Obter uma lista de objetos attendanceRecord e suas propriedades.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6cb1ab164f37ed08e8c941f75ea8b5b455dc5dc6
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63670611"
---
# <a name="list-attendancerecords"></a>Listar attendanceRecords
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de [objetos attendanceRecord](../resources/attendancerecord.md) e suas propriedades.

> [!TIP]
> Uma maneira mais conveniente de recuperar registros de participação é fazer com que eles se alimentem com um relatório de participação usando `expand` a opção de consulta. Para obter um exemplo e mais detalhes, consulte [Obter relatório de participação](meetingattendancereport-get.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:----------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante) | OnlineMeetingArtifact.Read.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo | OnlineMeetingArtifact.Read.All |

Para usar a permissão do aplicativo para essa API, os administradores de locatários devem criar uma política de acesso a aplicativos e concedi-la a um usuário. Isso autoriza o aplicativo configurado na política a buscar reuniões online e/ou artefatos de reunião online em nome desse usuário (com a ID do usuário especificada no caminho da solicitação). Para obter mais detalhes, consulte [Permitir que os aplicativos acessem reuniões online em nome de um usuário](/graph/cloud-communication-online-meeting-application-access-policy).

## <a name="http-request"></a>Solicitação HTTP

Para obter registros de participação de um relatório de participação com permissão delegada (`/me`) e app (`/users/{userId}`) :
<!-- {"blockType": "ignored"}-->
``` http
GET /me/onlineMeetings/{meetingId}/attendanceReports/{reportId}/attendanceRecords
GET /users/{userId}/onlineMeetings/{meetingId}/attendanceReports/{reportId}/attendanceRecords
```

>- `userId` é a ID de objeto de um usuário no [Portal de gerenciamento de usuário do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Para obter mais detalhes, consulte [Permitir que os aplicativos acessem reuniões online em nome de um usuário](/graph/cloud-communication-online-meeting-application-access-policy).
>- `meetingId` é a **id** de um [objeto onlineMeeting](../resources/onlinemeeting.md) .
>- `reportId` é a **id** de um [objeto meetingAttendanceReport](../resources/meetingAttendanceReport.md) .

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome            | Descrição               |
| :-------------- | :------------------------ |
| Autorização   | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [objetos attendanceRecord](../resources/attendancerecord.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_attendancerecord"
}
-->

``` http
GET https://graph.microsoft.com/beta/me/onlineMeetings/{meetingId}/attendanceReports/{reportId}/attendanceRecords
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-attendancerecord-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-attendancerecord-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-attendancerecord-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-attendancerecord-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-attendancerecord-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-attendancerecord-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.attendanceRecord)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "emailAddress": "frederick.cormier@contoso.com",
      "totalAttendanceInSeconds": 322,
      "role": "Organizer",
      "registrantId": null,
      "identity": {
        "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4623",
        "displayName": "Frederick Cormier",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-10-05T04:38:27.6027225Z",
          "leaveDateTime": "2021-10-05T04:43:49.7702391Z",
          "durationInSeconds": 322
        }
      ]
    },
    {
      "emailAddress": "lisa.adkins@contoso.com",
      "totalAttendanceInSeconds": 314,
      "role": "Presenter",
      "registrantId": null,
      "identity": {
        "id": "57caaef9-5ed0-48d5-8862-e5abfa71b3e9",
        "displayName": "Lisa Adkins",
        "tenantId": null
      },
      "attendanceIntervals": [
        {
          "joinDateTime": "2021-10-04T23:13:43.3776519Z",
          "leaveDateTime": "2021-10-04T23:18:57.5639338Z",
          "durationInSeconds": 314
        }
      ]
    }
  ]
}
```
