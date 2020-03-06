---
title: tipo de recurso bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 2bdf2fa686023ce33233722b3cd05f2984d1cabb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507898"
---
# <a name="bookingservice-resource-type"></a>tipo de recurso bookingService

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa informações sobre um serviço específico fornecido por um [bookingBusiness](bookingbusiness.md), como o nome do serviço, o preço e a equipe que geralmente fornece esse serviço.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar serviços](../api/bookingbusiness-list-services.md) | coleção [bookingService](bookingservice.md) | Obtenha uma lista de objetos **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.|
|[Criar bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Crie um **bookingService** para o [bookingbusiness](../resources/bookingbusiness.md)especificado. |
|[Obter bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Obtenha as propriedades e os relacionamentos de um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado.|
|[Update](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |Atualize um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado. |
|[Delete](../api/bookingservice-delete.md) | None |Exclua um objeto **bookingService** no [bookingbusiness](../resources/bookingbusiness.md)especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|defaultduration|Duração|O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos. Por exemplo, P11D23H59M 59.999999999999 S. |
|DefaultLocation|[location](location.md)|O local físico padrão para o serviço.|
|defaultprice|Duplo|O preço monetário padrão do serviço.|
|defaultpricetype|string|O modo padrão pelo qual o serviço é cobrado. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultlembrers|coleção [bookingReminder](bookingreminder.md)|O conjunto padrão de lembretes para um compromisso desse serviço. O valor dessa propriedade está disponível somente ao se ler este **bookingService** por sua ID.|
|description|String|Uma descrição de texto para o serviço.|
|displayName|Cadeia de caracteres|Um nome de serviço.|
|emailAddress|String|Um endereço de email|
|id|String|A ID do serviço, em um formato GUID. Somente leitura.|
|isHiddenFromCustomers|Boolean|True significa que este serviço não está disponível para os clientes para reserva.|
|notes|Cadeia de caracteres|Informações adicionais sobre este serviço.|
|Buffer|Duração|O tempo para o buffer após o término de um compromisso desse serviço e antes do próximo compromisso do cliente pode ser registrado.|
|antes do buffer|Duração|O tempo para o buffer antes que um compromisso para este serviço possa ser iniciado.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|O conjunto de políticas que determinam como os compromissos desse tipo de serviço devem ser criados e gerenciados.|
|staffMemberIds|String collection|Representa os [membros da equipe](bookingstaffmember.md) que fornecem esse serviço. |

## <a name="relationships"></a>Relações
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
  "suppressions": []
}
-->
