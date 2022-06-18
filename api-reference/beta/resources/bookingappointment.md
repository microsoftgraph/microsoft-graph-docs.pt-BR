---
title: Tipo de recurso bookingAppointment
description: Representa um compromisso do cliente para um bookingService, executado por um conjunto de membros da equipe, fornecido por um Microsoft Bookings negócios.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 18183d9f0694da1c2897cff92a5af7863b3df9c2
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160367"
---
# <a name="bookingappointment-resource-type"></a>Tipo de recurso bookingAppointment

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um compromisso do cliente para [um bookingService](bookingservice.md), executado por um conjunto de membros da equipe, fornecido por um Microsoft Bookings negócios.

> [!NOTE]
> Se você criar um aplicativo personalizado usando permissões de aplicativo, deverá seguir a validação [de regras de negócios](/graph/bookingsbusiness-business-rules).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar compromissos](../api/bookingbusiness-list-appointments.md) |  [coleção bookingAppointment](bookingappointment.md) | Obtenha uma lista de **objetos bookingAppointment** no [bookingbusiness especificado](bookingbusiness.md). |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Crie um **novo bookingAppointment** para o [bookingbusiness especificado](bookingbusiness.md). |
|[Obter bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Leia as propriedades e as relações do **objeto bookingAppointment** .|
|[Atualizar](../api/bookingappointment-update.md) | Nenhum(a)   |Atualize um **objeto bookingAppointment** . |
|[Excluir](../api/bookingappointment-delete.md) | Nenhuma |Exclua **um objeto bookingAppointment** . |
|[Cancel](../api/bookingappointment-cancel.md)|Nenhuma| Cancele **um objeto bookingAppointment** .|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|Cadeia de Caracteres|Informações adicionais que são enviadas ao cliente quando um compromisso é confirmado.|
|anonymousJoinWebUrl|Cadeia de Caracteres|URL da reunião para ingressar anonimamente.
|customerEmailAddress|Cadeia de Caracteres|O endereço SMTP do [bookingCustomer](bookingcustomer.md) que está reservando o compromisso.|
|customerId|Cadeia de Caracteres|A ID do [bookingCustomer](bookingcustomer.md) para este compromisso. Se nenhuma ID for especificada quando um compromisso for criado, um novo objeto **bookingCustomer** será criado. Depois de definido, você deve considerar **a customerId** imutável.|
|customerLocation|[location](location.md)|Representa informações de localização para [o bookingCustomer](bookingcustomer.md) que está reservando o compromisso.|
|Customername|Cadeia de Caracteres|O nome do cliente.|
|customerNotes|Cadeia de Caracteres|Observações do cliente associadas a este compromisso. Você só pode obter o valor ao ler este **bookingAppointment** por sua ID. <br> Você só pode definir essa propriedade ao criar inicialmente um compromisso com um novo cliente. Depois desse ponto, o valor é calculado do cliente representado por **customerId**.|
|customerPhone|Cadeia de Caracteres|O número de telefone do cliente.|
|Clientes|[coleção bookingCustomerInformation](bookingcustomerinformation.md)|Ele lista as propriedades do cliente para um compromisso. Um compromisso conterá uma lista de informações do cliente e cada unidade indicará as propriedades de um cliente que faz parte desse compromisso. Opcional.|
|customerTimeZone|Cadeia de Caracteres|O fuso horário do cliente. Para obter uma lista de valores possíveis, consulte [dateTimeTimeZone](datetimetimezone.md).|
|duração|Duration|O comprimento do compromisso, indicado no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso termina.|
|filledAttendeesCount|Int32|O número atual de clientes no compromisso. |
|id|Cadeia de caracteres| A ID do **bookingAppointment**. Somente leitura.|
|invoiceAmount|Duplo|O valor cobrado na fatura.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário da fatura para este compromisso.|
|invoiceId|Cadeia de Caracteres|A ID da fatura.|
|invoiceStatus|string| O status da fatura. Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|Cadeia de Caracteres|A URL da fatura em Microsoft Bookings.|
|isLocationOnline|Boolean|True indica que o compromisso será mantido online. O valor padrão é falso.|
|joinWebUrl|Cadeia de Caracteres|A URL da reunião online para o compromisso.|
|maximumAttendeesCount|Int32|O número máximo de clientes permitidos em um compromisso. Se **maximumAttendeesCount** do serviço for maior que 1, passe as IDs de cliente válidas ao criar ou atualizar um compromisso. Para criar um cliente, use a [operação Criar bookingCustomer](../api/bookingbusiness-post-customers.md) . |
|optOutOfCustomerEmail|Boolean|True indica que o [bookingCustomer](bookingcustomer.md) para este compromisso não deseja receber uma confirmação para este compromisso.|
|Postbuffer|Duration|A quantidade de tempo a ser reservado após o término do compromisso, para limpeza, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|Prebuffer|Duration|A quantidade de tempo a ser reservado antes do início do compromisso, para preparação, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Preço|Duplo|O preço normal de um compromisso para o [bookingService especificado](bookingservice.md).|
|priceType|bookingPriceType| Uma configuração para fornecer flexibilidade para a estrutura de preços dos serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|Lembretes|[coleção bookingReminder](bookingreminder.md)|A coleção de lembretes de clientes enviados para este compromisso. O valor dessa propriedade está disponível somente ao ler este **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|Cadeia de Caracteres|Uma ID de acompanhamento adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de um membro da equipe em nome do cliente.|
|serviceId|Cadeia de caracteres|A ID do [bookingService](bookingservice.md) associado a este compromisso.|
|serviceLocation|[location](location.md)|O local onde o serviço é entregue.|
|serviceName|Cadeia de Caracteres|O nome do **bookingService** associado a este compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, ele será calculado do serviço associado ao compromisso pela **propriedade serviceId** .|
|serviceNotes|Cadeia de Caracteres|Anotações de [um bookingStaffMember](bookingstaffmember.md). O valor dessa propriedade está disponível somente ao ler este **bookingAppointment** por sua ID.|
|smsNotificationsEnabled|Boolean|True indica SMS notificações serão enviadas aos clientes para o compromisso. O valor padrão é falso.|
|staffMemberIds|Coleção de cadeias de caracteres|A ID de cada [bookingStaffMember](bookingstaffmember.md) agendado neste compromisso.|
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso começa.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingAppointment"
}-->

```json
{
  "customerEmailAddress": "String",
  "customerId": "String",
  "customerLocation": {"@odata.type": "microsoft.graph.location"},
  "customerName": "String",
  "customerNotes": "String",
  "customerPhone": "String",
  "customerTimeZone": "String",
  "customers": [
    {
      "@odata.type": "microsoft.graph.bookingCustomerInformation"
    }
  ],
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "isLocationOnline": "Boolean",
  "joinWebUrl": "String",
  "optOutOfCustomerEmail": true,
  "anonymousJoinWebUrl": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "maximumAttendeesCount": "Integer",
  "filledAttendeesCount": "Integer"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


