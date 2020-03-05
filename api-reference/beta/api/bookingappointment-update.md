---
title: Atualizar bookingappointment
description: Atualiza as propriedades de um objeto bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e2af9b0a547ecea9895802d3f4ab4666a243ed9f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441281"
---
# <a name="update-bookingappointment"></a>Atualizar bookingappointment

Namespace: Microsoft. Graph

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
|customerEmailAddress|String|O endereço SMTP do [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.|
|Box|String|A ID do [bookingCustomer](../resources/bookingcustomer.md) para este compromisso. Se nenhuma ID for especificada quando um compromisso for criado, será criado um novo objeto **bookingCustomer** . Depois de definido, considere o **CustomerID** imutável.|
|customerLocation|[location](../resources/location.md)|Representa as informações de local para o [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.|
|Customer|String|O nome do cliente.|
|customerNotes|String|Observações do cliente associado a este compromisso. Você pode obter o valor somente ao ler este **bookingAppointment** por sua ID. <br> Você pode definir essa propriedade somente quando criar inicialmente um compromisso com um novo cliente. Após esse ponto, o valor é calculado a partir do cliente representado por **CustomerID**.|
|customerPhone|String|O número de telefone do cliente.|
|duration|Duração|O comprimento do compromisso, indicado no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso termina.|
|invoiceAmount|Duplo|O valor cobrado na fatura.|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário da fatura para este compromisso.|
|faturaid|String|A ID da fatura.|
|invoiceStatus|string| O status da fatura. Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|A URL da fatura em Microsoft bookings.|
|optOutOfCustomerEmail|Boolean|True indica que o [bookingCustomer](../resources/bookingcustomer.md) para este compromisso não deseja receber uma confirmação desse compromisso.|
|Buffer|Duração|A quantidade de tempo para reservar depois que o compromisso termina, para limpeza, como um exemplo. O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|antes do buffer|Duração|A quantidade de tempo para reservar antes de o compromisso começar, para preparação, como um exemplo. O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|descontos|Duplo|O preço regular de um compromisso para o [bookingService](../resources/bookingservice.md)especificado.|
|PriceType|string| Uma configuração para fornecer flexibilidade para a estrutura de preços de serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|lembretes|coleção [bookingReminder](../resources/bookingreminder.md)|O conjunto de lembretes do cliente enviado para este compromisso. O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|String|Uma ID de controle adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de por um membro da equipe em nome do cliente.|
|serviceId|String|A ID da [bookingService](../resources/bookingservice.md) associada a este compromisso.|
|serviceLocation|[location](../resources/location.md)|O local onde o serviço é entregue.|
|serviceName|String|O nome do **bookingService** associado a este compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, será calculado a partir do serviço associado ao compromisso pela propriedade **ServiceId** .|
|Notas|String|Observações de um [bookingStaffMember](../resources/bookingstaffmember.md). O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.|
|staffMemberIds|String collection|A ID de cada [bookingStaffMember](../resources/bookingstaffmember.md) que está agendado neste compromisso.|
|iniciar|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário de início do compromisso.|


## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir altera a data de serviço por um dia e também atualiza a data da fatura.

# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

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
  ]
}
-->
