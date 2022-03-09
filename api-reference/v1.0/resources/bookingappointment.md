---
title: Tipo de recurso bookingAppointment
description: Representa um compromisso do cliente para um bookingService, executado por um conjunto de membros da equipe, fornecido por uma empresa do Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c5e301d6ef48015feb417bf663709fd4024a3c4e
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367612"
---
# <a name="bookingappointment-resource-type"></a>Tipo de recurso bookingAppointment

Namespace: microsoft.graph
 
Representa um compromisso do cliente para [um bookingService](bookingservice.md), executado por um conjunto de membros da equipe, fornecido por uma empresa do Microsoft Bookings.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar compromissos](../api/bookingbusiness-list-appointments.md) |  [coleção bookingAppointment](bookingappointment.md) | Obter uma lista de **objetos bookingAppointment** no [bookingBusiness especificado](../resources/bookingbusiness.md). |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Crie um **novo bookingAppointment** para o [bookingBusiness especificado](../resources/bookingbusiness.md). |
|[Obter bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Leia as propriedades e as relações do **objeto bookingAppointment** .|
|[Update](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Atualize um **objeto bookingAppointment** . |
|[Delete](../api/bookingappointment-delete.md) | Nenhum |**Exclua um objeto bookingAppointment**. |
|[Cancel](../api/bookingappointment-cancel.md)|Nenhum| Cancele **um objeto bookingAppointment** .|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|String|Informações adicionais enviadas ao cliente quando um compromisso é confirmado.|
|customers|[coleção bookingCustomerInformation](../resources/bookingcustomerinformation.md)|Lista as propriedades do cliente para um compromisso. Um compromisso conterá uma lista de informações do cliente e cada unidade indicará as propriedades de um cliente que faz parte desse compromisso. Opcional.|
|customerTimeZone|String|O fuso horário do cliente. Para ver uma lista de valores possíveis, consulte [dateTimeTimeZone](datetimetimezone.md).|
|duração|Duration|O comprimento do compromisso, denotado no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que o compromisso termina.|
|filledAttendeesCount|Int32|O número atual de clientes no compromisso |
|id|Cadeia de caracteres| A ID do **bookingAppointment**. Somente leitura.|
|isLocationOnline|Booliano|If `true`, indica que o compromisso será mantido online. O valor padrão é `false`.|
|joinWebUrl|String|A URL da reunião online para o compromisso.|
|maximumAttendeesCount|Int32|O número máximo de clientes permitidos em um compromisso. Se **maximumAttendeesCount** do serviço for maior que 1, passe as IDs de cliente válidas durante a criação ou atualização de um compromisso. Para criar um cliente, use a [operação Criar bookingCustomer](../api/bookingbusiness-post-customers.md) . |
|optOutOfCustomerEmail|Booliano|Se `true` indicar que [o bookingCustomer](bookingcustomer.md) para esse compromisso não deseja receber uma confirmação para esse compromisso.|
|postBuffer|Duration|O tempo de reserva após o fim do compromisso, para limpeza, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Duration|O tempo de reserva antes do início do compromisso, para preparação, como exemplo. O valor é expresso no [formato ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|price|Duplo|O preço normal de um compromisso para o [bookingService especificado](bookingservice.md).|
|priceType|bookingPriceType| Uma configuração para oferecer flexibilidade para a estrutura de preços dos serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|lembretes|[Coleção bookingReminder](bookingreminder.md)|A coleção de lembretes de clientes enviados para esse compromisso. O valor dessa propriedade está disponível somente ao ler esse **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|String|Uma ID de acompanhamento adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de um membro da equipe em nome do cliente. Só há suporte para compromisso se maxAttendeeCount for 1.|
|serviceId|Cadeia de caracteres|A ID do [bookingService](bookingservice.md) associado a esse compromisso.|
|serviceLocation|[location](location.md)|O local onde o serviço é entregue.|
|serviceName|String|O nome do **bookingService** associado a esse compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, ele será calculado a partir do serviço associado ao compromisso pela **propriedade serviceId** .|
|serviceNotes|String|Observações de [um bookingStaffMember](bookingstaffmember.md). O valor dessa propriedade está disponível somente ao ler esse **bookingAppointment** por sua ID.|
|smsNotificationsEnabled|Booliano|If `true`, indica que as notificações de SMS serão enviadas aos clientes para o compromisso. O valor padrão é `false`.|
|staffMemberIds|Coleção String|A ID de [cada bookingStaffMember](bookingstaffmember.md) agendado neste compromisso.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário que o compromisso começa.|

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
  "customers": [
    {
      "@odata.type": "microsoft.graph.bookingCustomerInformation"
    }
  ],
  "duration": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "isLocationOnline": "Boolean",
  "joinWebUrl": "String",
  "optOutOfCustomerEmail": "Boolean",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": "Integer",
  "priceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
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


