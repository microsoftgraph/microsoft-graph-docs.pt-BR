---
title: tipo de recurso de bookingAppointment
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c5868788159f0602c1f8a263138c7ce9107c2c94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509837"
---
# <a name="bookingappointment-resource-type"></a>tipo de recurso de bookingAppointment

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um compromisso de cliente para um [bookingService](bookingservice.md), realizado por um conjunto de membros da equipe, fornecidos por uma empresa Microsoft Bookings.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista de compromissos](../api/bookingbusiness-list-appointments.md) |  coleção [bookingAppointment](bookingappointment.md) | Obtenha uma lista de objetos **bookingAppointment** no especificado [bookingbusiness](../resources/bookingbusiness.md). |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Crie um novo **bookingAppointment** para o especificado [bookingbusiness](../resources/bookingbusiness.md). |
|[Obter bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Leia as propriedades e relações do objeto **bookingAppointment** .|
|[Update](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Atualize um objeto **bookingAppointment** . |
|[Delete](../api/bookingappointment-delete.md) | Nenhum |Exclua um objeto **bookingAppointment** . |
|[Cancel](../api/bookingappointment-cancel.md)|Nenhum| Cancele um objeto **bookingAppointment** .|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customerEmailAddress|String|O endereço de SMTP do [bookingCustomer](bookingcustomer.md) quem é o compromisso de reserva.|
|customerId|String|A identificação do [bookingCustomer](bookingcustomer.md) para este compromisso. Se nenhuma identificação for especificada quando um compromisso é criado, um novo objeto **bookingCustomer** é criado. Definir uma vez, você deve considerar o **customerId** imutável.|
|customerLocation|[location](location.md)|Representa informações de localização para o [bookingCustomer](bookingcustomer.md) quem é o compromisso de reserva.|
|NomeDoCliente|String|O nome do cliente.|
|customerNotes|String|Observações do cliente associadas a este compromisso. Você pode obter o valor somente leitura quando este **bookingAppointment** pela sua identificação. <br> Você pode definir essa propriedade somente quando inicialmente criando um compromisso com um novo cliente. Após esse ponto, o valor é computado do cliente representado por **customerId**.|
|customerPhone|String|Número de telefone do cliente.|
|duration|Duration|O comprimento do compromisso, denotado em formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que termina o compromisso.|
|id|String| A identificação do **bookingAppointment**. Somente leitura.|
|invoiceAmount|Duplo|O valor cobrado na fatura.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e o fuso horário da fatura para este compromisso.|
|invoiceId|String|A identificação da fatura.|
|invoiceStatus|string| O status da fatura. Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|A URL da fatura na Microsoft Bookings.|
|optOutOfCustomerEmail|Booliano|True indica que o [bookingCustomer](bookingcustomer.md) para este compromisso não quiser receber uma confirmação para este compromisso.|
|postBuffer|Duration|A quantidade de tempo para reservar após as extremidades de compromisso, para limpando, como exemplo. O valor é expresso em formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Duration|A quantidade de tempo para reservar antes de começa o compromisso, para a preparação, como exemplo. O valor é expresso em formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Price|Duplo|O preço normal para um compromisso para o especificado [bookingService](bookingservice.md).|
|priceType|string| Uma configuração para fornecer flexibilidade para a estrutura de preços dos serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|Lembretes|coleção [bookingReminder](bookingreminder.md)|A coleção de lembretes de cliente enviados para este compromisso. O valor dessa propriedade está disponível somente quando a ler este **bookingAppointment** pela sua identificação.|
|selfServiceAppointmentId|String|Uma ID de controle adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de por um membro da equipe em nome do cliente.|
|serviceId|String|A identificação do [bookingService](bookingservice.md) associado a este compromisso.|
|serviceLocation|[location](location.md)|O local onde o serviço é entregue.|
|serviceName|String|O nome do **bookingService** associado a este compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não especificado, ele é computado do serviço associado ao compromisso pela propriedade **serviceId** .|
|serviceNotes|String|Anotações de um [bookingStaffMember](bookingstaffmember.md). O valor dessa propriedade está disponível somente quando a ler este **bookingAppointment** pela sua identificação.|
|staffMemberIds|String collection|A identificação de cada [bookingStaffMember](bookingstaffmember.md) que esteja agendado neste compromisso.|
|start|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que o compromisso é iniciado.|

## <a name="relationships"></a>Relacionamento
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
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "optOutOfCustomerEmail": true,
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": "string",
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingappointment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
