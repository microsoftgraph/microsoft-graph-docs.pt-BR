---
title: tipo de recurso de bookingSchedulingPolicy
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 15f9e0dea22a7cfb5eab437bcc023fe3387bb2ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805359"
---
# <a name="bookingschedulingpolicy-resource-type"></a>tipo de recurso de bookingSchedulingPolicy

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.
 
Representa o conjunto de diretivas que determinam como os compromissos devem ser criados em um calendário do Microsoft Bookings.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowStaffSelection|Booliano|True se permitir que os clientes escolham uma pessoa específica para a reserva.|
|maximumAdvance|Duração|Número máximo de dias de antecedência que pode ser feita uma reserva. Ela segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|minimumLeadTime|Duração|A quantidade mínima de tempo antes dos quais devem ser feitos reservas e cancelamentos. Ela segue o formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|sendConfirmationsToOwner|Booliano| True para notificar os negócios via email quando uma reserva é criada ou alterada. Use o endereço de email especificado na propriedade **email** da entidade **bookingBusiness** para os negócios. |
|timeSlotInterval|Duração|Duração de cada intervalo de tempo, denotado em formato [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
