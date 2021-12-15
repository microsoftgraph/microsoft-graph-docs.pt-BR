---
title: Atualizar bookingStaffMember
description: Atualize as propriedades de um bookingStaffMember no bookingBusiness especificado.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e0101a297b48a64fa38d494e53a1315011bfcf0f
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526439"
---
# <a name="update-bookingstaffmember"></a>Atualizar bookingstaffmember

Namespace: microsoft.graph

Atualize as propriedades de [um bookingStaffMember](../resources/bookingstaffmember.md) no [bookingBusiness especificado.](../resources/bookingbusiness.md)
## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | {code} do portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Booliano|True significa que, se o membro da equipe for um usuário Microsoft 365, a API do Microsoft Bookings usará o calendário pessoal do membro da equipe no Microsoft 365, bem como a propriedade **workingHours** para determinar a disponibilidade. |
|displayName|Cadeia de caracteres|O nome do membro da equipe, conforme exibido para os clientes.|
|emailAddress|String|O endereço de email do membro da equipe. Isso pode estar no mesmo Microsoft 365 locatário que a empresa ou em um domínio de email diferente. Esse endereço de email será usado **se a propriedade sendConfirmationsToOwner** estiver definida como na política `true` de agendamento da empresa.|
|role|string| A função do membro da equipe na empresa. Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`.|
|timeZone|Cadeia de caracteres|O fuso horário do membro da equipe. Para uma lista de valores possíveis, consulte [dateTimeTimeZone](../resources/datetimetimezone.md).|
|useBusinessHours|Booliano|True significa que a disponibilidade do membro da equipe é determinada pela **propriedade businessHours** da empresa. False significa que a disponibilidade é determinada pela configuração da propriedade **workingHouse** do membro da equipe.|
|workingHours|[Coleção bookingWorkHours](../resources/bookingworkhours.md)|O intervalo de horas a cada dia da semana que o membro da equipe está disponível para reserva.|

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
O exemplo a seguir altera a agenda do membro da equipe para ter as segundas-feiras de folga.

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingStaffMember",
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[

            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "endTime":"17:00:00.0000000",
                    "startTime":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "endTime":"17:00:00.0000000",
                    "startTime":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "endTime":"17:00:00.0000000",
                    "startTime":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "endTime":"17:00:00.0000000",
                    "startTime":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```

### <a name="response"></a>Resposta
Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


