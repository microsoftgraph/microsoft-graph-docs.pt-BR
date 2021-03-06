---
title: tipo de recurso de fileserviceendpoint
description: Representa as informações de identificação e URI de uma instância de serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8b9289807778c1a44940d8e8eb0d9163ed12f006
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985857"
---
# <a name="printserviceendpoint-resource-type"></a>tipo de recurso de fileserviceendpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de identificação e URI de uma instância de serviço de impressão.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter o ponto de extremidade](../api/printserviceendpoint-get.md) | [fileserviceendpoint](printserviceendpoint.md) | Leia as propriedades e os relacionamentos do objeto de ponto de extremidade. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String|Um nome de exibição legível para o ponto de extremidade.|
|nome|String|Um nome exclusivo que identifica o serviço que o ponto de extremidade fornece. Os valores possíveis são: `discovery` (serviço de descoberta), `notification` (serviço de notificação), `ipp` (serviço IPP) e `registration` (serviço de registro). Somente leitura.|
|URI|String|O URI que pode ser usado para acessar o serviço.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}-->

```json
{
  "displayName": "String",
  "name": "String (identifier)",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printServiceEndpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

