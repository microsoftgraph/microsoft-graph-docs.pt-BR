---
title: tipo de recurso de bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519882"
---
# <a name="bookingservice-resource-type"></a>tipo de recurso de bookingService

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa informações sobre um serviço específico fornecido por um [bookingBusiness](bookingbusiness.md), como o nome do serviço, preço e a equipe que geralmente fornece tal serviço.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista de serviços](../api/bookingbusiness-list-services.md) | coleção [bookingService](bookingservice.md) | Obtenha uma lista de objetos **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md).|
|[Criar bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Crie um **bookingService** para o especificado [bookingbusiness](../resources/bookingbusiness.md). |
|[Obter bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Obtenha as propriedades e relacionamentos de um objeto **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md).|
|[Update](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |Atualize um objeto **bookingService** o especificado [bookingbusiness](../resources/bookingbusiness.md). |
|[Delete](../api/bookingservice-delete.md) | Nenhum |Exclua um objeto **bookingService** no especificado [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|defaultDuration|Duration|O comprimento padrão do serviço, representado em número de dias, horas, minutos e segundos. Por exemplo, P11D23H59M59.999999999999S. |
|defaultLocation|[location](location.md)|A localização física padrão para o serviço.|
|defaultPrice|Duplo|O preço monetários padrão para o serviço.|
|defaultPriceType|string|A maneira padrão de serviço é cobrada. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|coleção [bookingReminder](bookingreminder.md)|O padrão é definido de lembretes para um compromisso desse serviço. O valor dessa propriedade está disponível somente quando a ler este **bookingService** pela sua identificação.|
|description|String|Uma descrição de texto para o serviço.|
|displayName|String|Um nome de serviço.|
|emailAddress|String|Um email:  |
|id|String|A identificação desse serviço, em um formato GUID. Somente leitura.|
|isHiddenFromCustomers|Booliano|True significa que esse serviço não está disponível para os clientes de reserva.|
|Observações|String|Informações adicionais sobre esse serviço.|
|postBuffer|Duration|Encerra o tempo de buffer após um compromisso para este serviço e antes que a próxima compromisso do cliente pode ser agendado.|
|preBuffer|Duration|O tempo de buffer antes de um compromisso para esse serviço pode iniciar.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|O conjunto de diretivas que determinam como compromissos para esse tipo de serviço devem ser criados e gerenciados.|
|staffMemberIds|String collection|Representa os [membros da equipe](bookingstaffmember.md) que forneça esse serviço. |

## <a name="relationships"></a>Relacionamento
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
