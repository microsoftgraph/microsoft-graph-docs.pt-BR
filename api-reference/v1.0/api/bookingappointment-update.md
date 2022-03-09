---
title: Atualizar bookingAppointment
description: Atualize as propriedades de um objeto bookingAppointment no bookingBusiness especificado.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d1b2e9863f8cc98cd2d17b9867817bb804dc3217
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367969"
---
# <a name="update-bookingappointment"></a>Atualizar bookingAppointment

Namespace: microsoft.graph

Atualize as propriedades de [um objeto bookingAppointment](../resources/bookingappointment.md) no [bookingBusiness especificado](../resources/bookingbusiness.md).
## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegada (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

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
|customers|[coleção bookingCustomerInformation](../resources/bookingcustomerinformation.md)|Lista as propriedades do cliente para um compromisso. Um compromisso conterá uma lista de informações do cliente e cada unidade indicará as propriedades de um cliente que faz parte desse compromisso. Opcional.|
|customerTimeZone|Cadeia de caracteres|O fuso horário do cliente. Para ver uma lista de valores possíveis, consulte [dateTimeTimeZone](../resources/datetimetimezone.md).|
|duração|Duration|O comprimento do compromisso, denotado no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, hora e fuso horário que o compromisso termina.|
|filledAttendeesCount|Int32|O número atual de clientes no compromisso. Obrigatório.|
|isLocationOnline|Booliano|If `true`, indica que o compromisso será mantido online. O valor padrão é falso.|
|maximumAttendeesCount|Int32|O número máximo de clientes permitidos no compromisso. Obrigatório. |
|optOutOfCustomerEmail|Booliano|If `true`, indica que [o bookingCustomer](../resources/bookingcustomer.md) para esse compromisso não deseja receber uma confirmação para esse compromisso.|
|postBuffer|Duration|O tempo de reserva após o fim do compromisso, para limpeza, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Duration|O tempo de reserva antes do início do compromisso, para preparação, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|price|Duplo|O preço normal de um compromisso para o [bookingService especificado](../resources/bookingservice.md).|
|priceType|bookingPriceType| Uma configuração para oferecer flexibilidade para a estrutura de preços dos serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|lembretes|[Coleção bookingReminder](../resources/bookingreminder.md)|A coleção de lembretes de clientes enviados para esse compromisso. O valor dessa propriedade está disponível somente ao ler esse **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|String|Uma ID de acompanhamento adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de um membro da equipe em nome do cliente. Só há suporte para compromisso se maxAttendeeCount for 1.|
|serviceId|Cadeia de caracteres|A ID do [bookingService](../resources/bookingservice.md) associado a esse compromisso.|
|serviceLocation|[location](../resources/location.md)|O local onde o serviço é entregue.|
|serviceName|Cadeia de caracteres|O nome do **bookingService** associado a esse compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, ele será calculado a partir do serviço associado ao compromisso pela **propriedade serviceId** .|
|serviceNotes|Cadeia de caracteres|Observações de [um bookingStaffMember](../resources/bookingstaffmember.md). O valor dessa propriedade está disponível somente ao ler esse **bookingAppointment** por sua ID.|
|smsNotificationsEnabled|Booliano|If `true`, indica que as notificações de SMS serão enviadas aos clientes para o compromisso. O valor padrão é falso.|
|staffMemberIds|Coleção String|A ID de [cada bookingStaffMember](../resources/bookingstaffmember.md) agendado neste compromisso.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário que o compromisso começa.|

> [!NOTE]
> Se o número máximo de clientes (**maximumAttedeesCount**) permitido no [serviço](../resources/bookingservice.md) for maior que 1:
> - Certifique-se de que os clientes existam no Calendário da Reserva. Se não o fazem, crie usando a [operação Criar bookingCustomer](bookingbusiness-post-customers.md) .
> - Passe as IDs de cliente válidas ao criar ou atualizar o compromisso. Se a ID do cliente não for válida, esse cliente não será incluído no objeto appointment.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
O exemplo a seguir altera a data do serviço por um dia.

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


