---
title: Tipo de recurso bookingAppointment
description: Representa um compromisso do cliente para um bookingService, executado por um conjunto de membros da equipe, fornecido por uma empresa do Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: ac5c39da4a9f6ad0ffc352007f10bc4d2dd68eff
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367717"
---
# <a name="bookingappointment-resource-type"></a>Tipo de recurso bookingAppointment

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um compromisso do cliente para [um bookingService](bookingservice.md), executado por um conjunto de membros da equipe, fornecido por uma empresa do Microsoft Bookings.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar compromissos](../api/bookingbusiness-list-appointments.md) |  [coleção bookingAppointment](bookingappointment.md) | Obter uma lista de **objetos bookingAppointment** no [bookingbusiness especificado](../resources/bookingbusiness.md). |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Crie um **novo bookingAppointment** para o [bookingbusiness especificado](../resources/bookingbusiness.md). |
|[Obter bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Leia as propriedades e as relações do **objeto bookingAppointment** .|
|[Update](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Atualize um **objeto bookingAppointment** . |
|[Delete](../api/bookingappointment-delete.md) | Nenhuma |**Exclua um objeto bookingAppointment**. |
|[Cancel](../api/bookingappointment-cancel.md)|Nenhuma| Cancele **um objeto bookingAppointment** .|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|String|Informações adicionais enviadas ao cliente quando um compromisso é confirmado.|
|customerEmailAddress|String|O endereço SMTP do [bookingCustomer](bookingcustomer.md) que está reservando o compromisso.|
|customerId|String|A ID do [bookingCustomer](bookingcustomer.md) para esse compromisso. Se nenhuma ID for especificada quando um compromisso for criado, um novo **objeto bookingCustomer** será criado. Depois de definido, você deve considerar **o customerId** imutável.|
|customerLocation|[location](location.md)|Representa informações de local para [o bookingCustomer](bookingcustomer.md) que está reservando o compromisso.|
|customerName|String|O nome do cliente.|
|customerNotes|String|Observações do cliente associado a esse compromisso. Você só pode obter o valor ao ler **esse bookingAppointment** por sua ID. <br> Você só pode definir essa propriedade ao criar um compromisso com um novo cliente inicialmente. Após esse ponto, o valor é calculado a partir do cliente representado por **customerId**.|
|customerPhone|String|O número de telefone do cliente.|
|customers|[coleção bookingCustomerInformation](../resources/bookingcustomerinformation.md)|Lista as propriedades do cliente para um compromisso. Um compromisso conterá uma lista de informações do cliente e cada unidade indicará as propriedades de um cliente que faz parte desse compromisso. Opcional.|
|customerTimeZone|String|O fuso horário do cliente. Para ver uma lista de valores possíveis, consulte [dateTimeTimeZone](datetimetimezone.md).|
|duração|Duration|O comprimento do compromisso, denotado no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que o compromisso termina.|
|filledAttendeesCount|Int32|O número atual de clientes no compromisso. |
|id|Cadeia de caracteres| A ID do **bookingAppointment**. Somente leitura.|
|invoiceAmount|Duplo|O valor cobrado na fatura.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário da fatura para esse compromisso.|
|invoiceId|Cadeia de caracteres|A ID da fatura.|
|invoiceStatus|string| O status da fatura. Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|A URL da fatura no Microsoft Bookings.|
|isLocationOnline|Booliano|True indica que o compromisso será mantido online. O valor padrão é falso.|
|joinWebUrl|String|A URL da reunião online para o compromisso.|
|maximumAttendeesCount|Int32|O número máximo de clientes permitidos em um compromisso. Se **maximumAttendeesCount** do serviço for maior que 1, passe as IDs de cliente válidas durante a criação ou atualização de um compromisso. Para criar um cliente, use a [operação Criar bookingCustomer](../api/bookingbusiness-post-customers.md) . |
|optOutOfCustomerEmail|Booliano|True indica que [o bookingCustomer](bookingcustomer.md) para esse compromisso não deseja receber uma confirmação para esse compromisso.|
|postBuffer|Duration|O tempo de reserva após o fim do compromisso, para limpeza, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Duration|O tempo de reserva antes do início do compromisso, para preparação, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|price|Duplo|O preço normal de um compromisso para o [bookingService especificado](bookingservice.md).|
|priceType|bookingPriceType| Uma configuração para oferecer flexibilidade para a estrutura de preços dos serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|lembretes|[Coleção bookingReminder](bookingreminder.md)|A coleção de lembretes de clientes enviados para esse compromisso. O valor dessa propriedade está disponível somente ao ler esse **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|String|Uma ID de acompanhamento adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de um membro da equipe em nome do cliente.|
|serviceId|Cadeia de caracteres|A ID do [bookingService](bookingservice.md) associado a esse compromisso.|
|serviceLocation|[location](location.md)|O local onde o serviço é entregue.|
|serviceName|String|O nome do **bookingService** associado a esse compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, ele será calculado a partir do serviço associado ao compromisso pela **propriedade serviceId** .|
|serviceNotes|Cadeia de caracteres|Observações de [um bookingStaffMember](bookingstaffmember.md). O valor dessa propriedade está disponível somente ao ler esse **bookingAppointment** por sua ID.|
|smsNotificationsEnabled|Booliano|True indica que as notificações de SMS serão enviadas aos clientes para o compromisso. O valor padrão é falso.|
|staffMemberIds|String collection|A ID de [cada bookingStaffMember](bookingstaffmember.md) agendado neste compromisso.|
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário que o compromisso começa.|

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


