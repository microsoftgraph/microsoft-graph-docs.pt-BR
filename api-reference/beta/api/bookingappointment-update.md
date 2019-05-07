---
title: Atualizar bookingappointment
description: Atualiza as propriedades de um objeto bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 32596ae8528f6c73ae4b82852baaed0031db7b57
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636209"
---
# <a name="update-bookingappointment"></a>Atualizar bookingappointment

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades de um objeto [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All   |
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
| Authorization  | Portador {código}|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customerEmailAddress|Cadeia de caracteres|O endereço SMTP do [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.|
|Box|Cadeia de caracteres|A ID do [bookingCustomer](../resources/bookingcustomer.md) para este compromisso. Se nenhuma ID for especificada quando um compromisso for criado, será criado um novo objeto **bookingCustomer** . Depois de definido, considere o **CustomerID** imutável.|
|customerLocation|[location](../resources/location.md)|Representa as informações de local para o [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.|
|Customer|Cadeia de caracteres|O nome do cliente.|
|customerNotes|Cadeia de caracteres|Observações do cliente associado a este compromisso. Você pode obter o valor somente ao ler este **bookingAppointment** por sua ID. <br> Você pode definir essa propriedade somente quando criar inicialmente um compromisso com um novo cliente. Após esse ponto, o valor é calculado a partir do cliente representado por **CustomerID**.|
|customerPhone|Cadeia de caracteres|O número de telefone do cliente.|
|duration|Duração|O comprimento do compromisso, indicado no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso termina.|
|invoiceAmount|Duplo|O valor cobrado na fatura.|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário da fatura para este compromisso.|
|faturaid|Cadeia de caracteres|A ID da fatura.|
|invoiceStatus|cadeia de caracteres| O status da fatura. Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|Cadeia de caracteres|A URL da fatura em Microsoft bookings.|
|optOutOfCustomerEmail|Booliano|True indica que o [bookingCustomer](../resources/bookingcustomer.md) para este compromisso não deseja receber uma confirmação desse compromisso.|
|Buffer|Duração|A quantidade de tempo para reservar depois que o compromisso termina, para limpeza, como um exemplo. O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|antes do buffer|Duração|A quantidade de tempo para reservar antes de o compromisso começar, para preparação, como um exemplo. O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|descontos|Duplo|O preço regular de um compromisso para o [bookingService](../resources/bookingservice.md)especificado.|
|PriceType|cadeia de caracteres| Uma configuração para fornecer flexibilidade para a estrutura de preços de serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|lembretes|coleção [bookingReminder](../resources/bookingreminder.md)|O conjunto de lembretes do cliente enviado para este compromisso. O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|Cadeia de caracteres|Uma ID de controle adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de por um membro da equipe em nome do cliente.|
|serviceId|Cadeia de caracteres|A ID da [bookingService](../resources/bookingservice.md) associada a este compromisso.|
|serviceLocation|[location](../resources/location.md)|O local onde o serviço é entregue.|
|serviceName|Cadeia de caracteres|O nome do **bookingService** associado a este compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, será calculado a partir do serviço associado ao compromisso pela propriedade **ServiceId** .|
|Notas|Cadeia de caracteres|Observações de um [bookingStaffMember](../resources/bookingstaffmember.md). O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.|
|staffMemberIds|Coleção de cadeias de caracteres|A ID de cada [bookingStaffMember](../resources/bookingstaffmember.md) que está agendado neste compromisso.|
|iniciar|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário de início do compromisso.|


## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir altera a data de serviço por um dia e também atualiza a data da fatura.
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
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[Basic](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingappointment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingappointment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
