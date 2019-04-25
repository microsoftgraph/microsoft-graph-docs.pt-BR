---
title: tipo de recurso bookingAppointment
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c5868788159f0602c1f8a263138c7ce9107c2c94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535501"
---
# <a name="bookingappointment-resource-type"></a>tipo de recurso bookingAppointment

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um compromisso de cliente para um [bookingService](bookingservice.md), executado por um conjunto de membros da equipe, fornecido por uma empresa de livros da Microsoft.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar compromissos](../api/bookingbusiness-list-appointments.md) |  coleção [bookingAppointment](bookingappointment.md) | Obtenha uma lista de objetos **bookingAppointment** no [bookingbusiness](../resources/bookingbusiness.md)especificado. |
|[Criar bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Crie um novo **bookingAppointment** para o [bookingbusiness](../resources/bookingbusiness.md)especificado. |
|[Obter bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Leia as propriedades e os relacionamentos do objeto **bookingAppointment** .|
|[Update](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Atualizar um objeto **bookingAppointment** . |
|[Excluir](../api/bookingappointment-delete.md) | Nenhum |Excluir um objeto **bookingAppointment** . |
|[Cancel](../api/bookingappointment-cancel.md)|Nenhum| Cancelar um objeto **bookingAppointment** .|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customerEmailAddress|String|O endereço SMTP do [bookingCustomer](bookingcustomer.md) que está reservando o compromisso.|
|Box|String|A ID do [bookingCustomer](bookingcustomer.md) para este compromisso. Se nenhuma ID for especificada quando um compromisso for criado, será criado um novo objeto **bookingCustomer** . Depois de definido, considere o **CustomerID** imutável.|
|customerLocation|[location](location.md)|Representa as informações de local para o [bookingCustomer](bookingcustomer.md) que está reservando o compromisso.|
|Customer|String|O nome do cliente.|
|customerNotes|String|Observações do cliente associado a este compromisso. Você pode obter o valor somente ao ler este **bookingAppointment** por sua ID. <br> Você pode definir essa propriedade somente quando criar inicialmente um compromisso com um novo cliente. Após esse ponto, o valor é calculado a partir do cliente representado por **CustomerID**.|
|customerPhone|String|O número de telefone do cliente.|
|duration|Duração|O comprimento do compromisso, indicado no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que o compromisso termina.|
|id|String| A ID do **bookingAppointment**. Somente leitura.|
|invoiceAmount|Duplo|O valor cobrado na fatura.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário da fatura para este compromisso.|
|faturaid|String|A ID da fatura.|
|invoiceStatus|string| O status da fatura. Os possíveis valores são: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|A URL da fatura em Microsoft bookings.|
|optOutOfCustomerEmail|Booliano|True indica que o [bookingCustomer](bookingcustomer.md) para este compromisso não deseja receber uma confirmação desse compromisso.|
|Buffer|Duração|A quantidade de tempo para reservar depois que o compromisso termina, para limpeza, como um exemplo. O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|antes do buffer|Duração|A quantidade de tempo para reservar antes de o compromisso começar, para preparação, como um exemplo. O valor é expresso no formato [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|descontos|Duplo|O preço regular de um compromisso para o [bookingService](bookingservice.md)especificado.|
|PriceType|string| Uma configuração para fornecer flexibilidade para a estrutura de preços de serviços. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|lembretes|coleção [bookingReminder](bookingreminder.md)|O conjunto de lembretes do cliente enviado para este compromisso. O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.|
|selfServiceAppointmentId|String|Uma ID de controle adicional para o compromisso, se o compromisso tiver sido criado diretamente pelo cliente na página de agendamento, em vez de por um membro da equipe em nome do cliente.|
|serviceId|String|A ID da [bookingService](bookingservice.md) associada a este compromisso.|
|serviceLocation|[location](location.md)|O local onde o serviço é entregue.|
|serviceName|String|O nome do **bookingService** associado a este compromisso.<br>Essa propriedade é opcional ao criar um novo compromisso. Se não for especificado, será calculado a partir do serviço associado ao compromisso pela propriedade **ServiceId** .|
|Notas|String|Observações de um [bookingStaffMember](bookingstaffmember.md). O valor dessa propriedade está disponível somente ao se ler este **bookingAppointment** por sua ID.|
|staffMemberIds|Coleção de cadeias de caracteres|A ID de cada [bookingStaffMember](bookingstaffmember.md) que está agendado neste compromisso.|
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário de início do compromisso.|

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
