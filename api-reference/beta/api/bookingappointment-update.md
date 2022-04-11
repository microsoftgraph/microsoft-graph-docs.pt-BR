---
title: Atualizar bookingAppointment
description: Atualize as propriedades de um objeto bookingAppointment no bookingBusiness especificado.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: fcbbb774d3981a1174493e2305c78e2042988985
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755548"
---
# <a name="update-bookingappointment"></a>Atualizar bookingAppointment

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto bookingAppointment](../resources/bookingappointment.md) no [bookingBusiness especificado](../resources/bookingbusiness.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  BookingsAppointment.ReadWrite.All, Bookings. ReadWrite.All, Bookings. Manage.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.   |
|Application | BookingsAppointment.ReadWrite.All, Bookings. Read.All  |

> [!NOTE]
> Se você criar um aplicativo personalizado usando permissões de aplicativo, deverá seguir a validação [de regras de negócios](/graph/bookingsbusiness-business-rules).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | {code} do portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customerEmailAddress|Cadeia de caracteres|O endereço SMTP do [bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.|
|customerId|String|A ID do [bookingCustomer](../resources/bookingcustomer.md) para este compromisso. Se nenhuma ID for especificada quando um compromisso for criado, um novo objeto **bookingCustomer** será criado. Depois de definido, você deve considerar **a customerId** imutável.|
|customerLocation|[location](../resources/location.md)|Representa informações de localização para [o bookingCustomer](../resources/bookingcustomer.md) que está reservando o compromisso.|
|Customername|Cadeia de caracteres|O nome do cliente.|
|customerNotes|String|Observações do cliente associadas a este compromisso. Você só pode obter o valor ao ler este **bookingAppointment** por sua ID. <br> Você só pode definir essa propriedade ao criar inicialmente um compromisso com um novo cliente. Depois desse ponto, o valor é calculado do cliente representado por **customerId**.|
|customerPhone|String|O número de telefone do cliente.|
|Clientes|[coleção bookingCustomerInformation](../resources/bookingcustomerinformation.md)|Ele lista as propriedades do cliente para um compromisso. Um compromisso conterá uma lista de informações do cliente e cada unidade indicará as propriedades de um cliente que faz parte desse compromisso. Opcional.|
|customerTimeZone|String|O fuso horário do cliente. Para obter uma lista de valores possíveis, consulte [dateTimeTimeZone](../resources/datetimetimezone.md).|
|duração|Duração|O comprimento do compromisso, indicado no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso termina.|
|invoiceAmount|Duplo|O valor cobrado na fatura.|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário da fatura para este compromisso.|
|invoiceId|Cadeia de caracteres|A ID da fatura.|
|invoiceStatus|string| O status da fatura. Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|A URL da fatura em Microsoft Bookings.|
|filledAttendeesCount|Int32|O número atual de clientes no compromisso. Obrigatório.|
|isLocationOnline|Boolean|True indica que o compromisso será mantido online. O valor padrão é falso.|
|maximumAttendeesCount|Int32|O número máximo de clientes permitidos no compromisso. Obrigatório. |
|optOutOfCustomerEmail|Boolean|True indica que o [bookingCustomer](../resources/bookingcustomer.md) para este compromisso não deseja receber uma confirmação para este compromisso.|
|Postbuffer|Duração|A quantidade de tempo a ser reservado após o término do compromisso, para limpeza, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|Prebuffer|Duração|A quantidade de tempo a ser reservado antes do início do compromisso, para preparação, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Preço|Duplo|O preço normal de um compromisso para o [bookingService especificado](../resources/bookingservice.md).|
|priceType|bookingPriceType| Uma configuração para fornecer flexibilidade para a estrutura de preços dos serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|Lembretes|[coleção bookingReminder](../resources/bookingreminder.md)|A coleção de lembretes de clientes enviados para este compromisso. O valor dessa propriedade está disponível somente ao ler este **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|String|Uma ID de acompanhamento adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de um membro da equipe em nome do cliente.|
|serviceId|Cadeia de caracteres|A ID do [bookingService](../resources/bookingservice.md) associado a este compromisso.|
|serviceLocation|[location](../resources/location.md)|O local onde o serviço é entregue.|
|serviceName|Cadeia de caracteres|O nome do **bookingService** associado a este compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, ele será calculado do serviço associado ao compromisso pela **propriedade serviceId** .|
|serviceNotes|String|Anotações de [um bookingStaffMember](../resources/bookingstaffmember.md). O valor dessa propriedade está disponível somente ao ler este **bookingAppointment** por sua ID.|
|smsNotificationsEnabled|Booliano|True indica que as notificações por SMS serão enviadas aos clientes para o compromisso. O valor padrão é falso.|
|staffMemberIds|String collection|A ID de cada [bookingStaffMember](../resources/bookingstaffmember.md) agendado neste compromisso.|
|iniciar|[dateTimeTimeZone](../resources/datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso começa.|

> [!NOTE]
> Se o número máximo de clientes (**maximumAttedeesCount**) permitido no [serviço](../resources/bookingservice.md) for maior que 1:
> - Verifique se os clientes existem no Calendário de Reserva. Caso contrário, crie usando a [operação Criar bookingCustomer](bookingbusiness-post-customers.md) .
> - Passe as IDs de cliente válidas ao criar ou atualizar o compromisso. Se a ID do cliente não for válida, esse cliente não será incluído no objeto de compromisso.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`. Ele não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

O exemplo a seguir altera a data do serviço por dia e atualiza a data da fatura.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA=
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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingappointment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookingappointment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

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


