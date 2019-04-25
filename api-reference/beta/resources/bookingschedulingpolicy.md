---
title: tipo de recurso bookingSchedulingPolicy
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3dee3314818d46c4131526dc92565eb4f8ca6ea2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543720"
---
# <a name="bookingschedulingpolicy-resource-type"></a>tipo de recurso bookingSchedulingPolicy

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa o conjunto de políticas que determinam como os compromissos devem ser criados em um calendário do Microsoft bookings.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowStaffSelection|Booliano|True se para permitir que os clientes escolham uma pessoa específica para a reserva.|
|maximumAdvance|Duração|Número máximo de dias de antecedência que uma reserva pode ser feita. Ele segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|minimumLeadTime|Duração|A quantidade mínima de tempo antes da qual as reservas e os cancelamentos devem ser feitos. Ele segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|sendConfirmationsToOwner|Booliano| True para notificar a empresa por email quando uma reserva é criada ou alterada. Use o endereço de email especificado na propriedade **email** da entidade **bookingBusiness** para a empresa. |
|timeSlotInterval|Duração|Duração de cada intervalo de tempo, indicado no formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingschedulingpolicy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
