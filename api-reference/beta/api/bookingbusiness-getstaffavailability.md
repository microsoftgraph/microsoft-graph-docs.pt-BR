---
title: 'bookingsBusiness: getStaffAvailability'
description: Obtenha as informações de disponibilidade dos membros da equipe de um Microsoft Bookings calendário.
ms.localizationpriority: medium
author: kwekua
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 692342668636e26258e9b7bf4a770f91d76c9b36
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668878"
---
# <a name="bookingsbusiness-getstaffavailability"></a>bookingsBusiness: getStaffAvailability

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha as informações de disponibilidade [dos membros da equipe](../resources/bookingstaffmember.md) de [um Microsoft Bookings calendário](../resources/bookingappointment.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte.   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Calendar.Read, Calendar.ReadWrite, Bookings.Read.All, Calendars.ReadWrite  |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/getStaffAvailability
```

## <a name="request-header"></a>Cabeçalho da solicitação

|Nome |Descrição |
|:--------------|:------------|
|Autorização |{code} do portador. Obrigatório. |
|Content-Type| application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, passe a lista de IDs de equipe junto com dois outros parâmetros do tipo de recurso [dateTimeTimeZone](/graph/resources/datetimetimezone) chamados **startDateTime** e **endDateTime**. Eles correspondem aos dois carimbos de data/hora entre os quais a disponibilidade da equipe será retornada.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma [coleção staffAvailabilityItem](../resources/staffavailabilityitem.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getstaffavailability"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/getStaffAvailability 
Content-Type: application/json 

{ 
    "staffIds": [ 
        "311a5454-08b2-4560-ba1c-f715e938cb79" 
    ], 
    "startDateTime": { 
        "dateTime": "2022-01-25T00: 00: 00", 
        "timeZone": "India Standard Time" 
    }, 
    "endDateTime": { 
        "dateTime": "2022-01-26T17: 00: 00", 
        "timeZone": "Pacific Standard Time" 
    } 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getstaffavailability-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getstaffavailability-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getstaffavailability-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-getstaffavailability-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/bookingbusiness-getstaffavailability-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

O exemplo a seguir mostra a resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.staffAvailabilityItem",
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{ 
    "staffAvailabilityItem": [ 
        { 
            "staffId": "311a5454-08b2-4560-ba1c-f715e938cb79", 
            "availabilityItems": [ 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T15:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Busy", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T15:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T16:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T16:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-25T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-25T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-26T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-26T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                } 
            ] 
        } 
    ] 
}
```
<!-- 
In the response body, for each staff member, their available windows are returned. The types of status of the windows are explained below.

|Type      | Explanation              |
|:--------------------|:---------------------------------------------------------|
|Available | The staff member is available in the given window.   |
|slotAvailable | The staff member has an appointment in the given window. The appointment is for a service which has **maxAttendeecount** more than 1. The customer can join this appointment as there are empty slots available.   |
|Busy | The staff member has an appointment in the given window. Either the staff member has an appointment for a service which has **maxAttendeecount** equal to 1 or the staff has an appointment for a service with **maxAttendeecount** more than 1 but without any available slots.  |


-->
