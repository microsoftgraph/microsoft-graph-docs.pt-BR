---
title: Atualizar bookingAppointment
description: Atualize as propriedades de um objeto bookingAppointment no bookingBusiness especificado.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 429d6331bdff07c7e3c8010b6801725c42f8efc4
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856068"
---
# <a name="update-bookingappointment"></a>Atualizar bookingAppointment

Namespace: microsoft.graph

Atualize as propriedades de [um objeto bookingAppointment](../resources/bookingappointment.md) no [bookingBusiness especificado](../resources/bookingbusiness.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | BookingsAppointment.ReadWrite.All, Bookings.Read.All  |

> [!NOTE]
> Se você criar um aplicativo personalizado usando permissões de aplicativo, deverá seguir a validação [de regras de negócios](/graph/bookingsbusiness-business-rules).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /solutions/bookingBusinesses/{id}/appointments/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | {code} do portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|Clientes|[coleção bookingCustomerInformation](../resources/bookingcustomerinformation.md)|Ele lista as propriedades do cliente para um compromisso. Um compromisso conterá uma lista de informações do cliente e cada unidade indicará as propriedades de um cliente que faz parte desse compromisso. Opcional.|
|customerTimeZone|Cadeia de caracteres|O fuso horário do cliente. Para obter uma lista de valores possíveis, consulte [dateTimeTimeZone](../resources/datetimetimezone.md).|
|duração|Duração|O comprimento do compromisso, indicado no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso termina.|
|filledAttendeesCount|Int32|O número atual de clientes no compromisso. Obrigatório.|
|isLocationOnline|Booliano|If `true`, indica que o compromisso será mantido online. O valor padrão é falso.|
|maximumAttendeesCount|Int32|O número máximo de clientes permitidos no compromisso. Obrigatório. |
|optOutOfCustomerEmail|Booliano|If `true`, indica que [o bookingCustomer](../resources/bookingcustomer.md) para este compromisso não deseja receber uma confirmação para este compromisso.|
|Postbuffer|Duração|A quantidade de tempo a ser reservado após o término do compromisso, para limpeza, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|Prebuffer|Duração|A quantidade de tempo a ser reservado antes do início do compromisso, para preparação, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Preço|Duplo|O preço normal de um compromisso para o [bookingService especificado](../resources/bookingservice.md).|
|priceType|bookingPriceType| Uma configuração para fornecer flexibilidade para a estrutura de preços dos serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|Lembretes|[coleção bookingReminder](../resources/bookingreminder.md)|A coleção de lembretes de clientes enviados para este compromisso. O valor dessa propriedade está disponível somente ao ler este **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|String|Uma ID de acompanhamento adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de um membro da equipe em nome do cliente. Só há suporte para compromisso se maxAttendeeCount for 1.|
|serviceId|Cadeia de caracteres|A ID do [bookingService](../resources/bookingservice.md) associado a este compromisso.|
|serviceLocation|[location](../resources/location.md)|O local onde o serviço é entregue.|
|serviceName|String|O nome do **bookingService** associado a este compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, ele será calculado do serviço associado ao compromisso pela **propriedade serviceId** .|
|serviceNotes|Cadeia de caracteres|Anotações de [um bookingStaffMember](../resources/bookingstaffmember.md). O valor dessa propriedade está disponível somente ao ler este **bookingAppointment** por sua ID.|
|smsNotificationsEnabled|Booliano|If `true`, indica que as notificações por SMS serão enviadas aos clientes para o compromisso. O valor padrão é falso.|
|staffMemberIds|Coleção de cadeias de caracteres|A ID de cada [bookingStaffMember](../resources/bookingstaffmember.md) agendado neste compromisso.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso começa.|

> [!NOTE]
> Se o número máximo de clientes (**maximumAttedeesCount**) permitido no [serviço](../resources/bookingservice.md) for maior que 1:
> - Verifique se os clientes existem no Calendário de Reserva. Caso contrário, crie usando a [operação Criar bookingCustomer](bookingbusiness-post-customers.md) .
> - Passe as IDs de cliente válidas ao criar ou atualizar o compromisso. Se a ID do cliente não for válida, esse cliente não será incluído no objeto de compromisso.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`. Ele não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

O exemplo a seguir altera a data do serviço por dia.

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "endDateTime":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "startDateTime":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
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
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->