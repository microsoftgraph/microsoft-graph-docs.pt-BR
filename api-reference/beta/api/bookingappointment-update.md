---
title: Atualizar bookingappointment
description: Atualize as propriedades de um objeto de bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cde8a309e3544f5ed5cdf84f7c50d33e95084526
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529233"
---
# <a name="update-bookingappointment"></a>Atualizar bookingappointment

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um objeto de [bookingAppointment](../resources/bookingappointment.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Aplicativo | Sem suporte.  |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customerEmailAddress|String|O endereço de SMTP do [bookingCustomer](../resources/bookingcustomer.md) quem é o compromisso de reserva.|
|customerId|String|A identificação do [bookingCustomer](../resources/bookingcustomer.md) para este compromisso. Se nenhuma identificação for especificada quando um compromisso é criado, um novo objeto **bookingCustomer** é criado. Definir uma vez, você deve considerar o **customerId** imutável.|
|customerLocation|[location](../resources/location.md)|Representa informações de localização para o [bookingCustomer](../resources/bookingcustomer.md) quem é o compromisso de reserva.|
|NomeDoCliente|String|O nome do cliente.|
|customerNotes|String|Observações do cliente associadas a este compromisso. Você pode obter o valor somente leitura quando este **bookingAppointment** pela sua identificação. <br> Você pode definir essa propriedade somente quando inicialmente criando um compromisso com um novo cliente. Após esse ponto, o valor é computado do cliente representado por **customerId**.|
|customerPhone|String|Número de telefone do cliente.|
|duration|Duration|O comprimento do compromisso, denotado em formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, hora e fuso horário que termina o compromisso.|
|invoiceAmount|Duplo|O valor cobrado na fatura.|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, hora e o fuso horário da fatura para este compromisso.|
|invoiceId|String|A identificação da fatura.|
|invoiceStatus|string| O status da fatura. Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|A URL da fatura na Microsoft Bookings.|
|optOutOfCustomerEmail|Booliano|True indica que o [bookingCustomer](../resources/bookingcustomer.md) para este compromisso não quiser receber uma confirmação para este compromisso.|
|postBuffer|Duration|A quantidade de tempo para reservar após as extremidades de compromisso, para limpando, como exemplo. O valor é expresso em formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Duration|A quantidade de tempo para reservar antes de começa o compromisso, para a preparação, como exemplo. O valor é expresso em formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Price|Duplo|O preço normal para um compromisso para o especificado [bookingService](../resources/bookingservice.md).|
|priceType|string| Uma configuração para fornecer flexibilidade para a estrutura de preços dos serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|Lembretes|coleção [bookingReminder](../resources/bookingreminder.md)|A coleção de lembretes de cliente enviados para este compromisso. O valor dessa propriedade está disponível somente quando a ler este **bookingAppointment** pela sua identificação.|
|selfServiceAppointmentId|String|Uma ID de controle adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de por um membro da equipe em nome do cliente.|
|serviceId|String|A identificação do [bookingService](../resources/bookingservice.md) associado a este compromisso.|
|serviceLocation|[location](../resources/location.md)|O local onde o serviço é entregue.|
|serviceName|String|O nome do **bookingService** associado a este compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não especificado, ele é computado do serviço associado ao compromisso pela propriedade **serviceId** .|
|serviceNotes|String|Anotações de um [bookingStaffMember](../resources/bookingstaffmember.md). O valor dessa propriedade está disponível somente quando a ler este **bookingAppointment** pela sua identificação.|
|staffMemberIds|String collection|A identificação de cada [bookingStaffMember](../resources/bookingstaffmember.md) que esteja agendado neste compromisso.|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, hora e fuso horário que o compromisso é iniciado.|


## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir altera a data do serviço por um dia e data da nota de atualizados.
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
##### <a name="response"></a>Resposta
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
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
