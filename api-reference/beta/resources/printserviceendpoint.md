---
title: Tipo de recurso printServiceEndpoint
description: Representa o URI e as informações de identificação de uma instância de serviço de impressão.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 3c5d9085614b4c4ad99aa43cb8281a3123eb3741
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176752"
---
# <a name="printserviceendpoint-resource-type"></a>Tipo de recurso printServiceEndpoint

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o URI e as informações de identificação de uma instância de serviço de impressão.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter o ponto de extremidade](../api/printserviceendpoint-get.md) | [printServiceEndpoint](printserviceendpoint.md) | Leia as propriedades e as relações do objeto de ponto de extremidade. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Um nome de exibição legível por humanos para o ponto de extremidade.|
|nome|Cadeia de caracteres|Um nome exclusivo que identifica o serviço que o ponto de extremidade fornece. Os valores possíveis são: `discovery` (Serviço de Descoberta), `notification` (Serviço de Notificação), `ipp` (Serviço IPP) e `registration` (Serviço de Registro). Somente leitura.|
|Uri|Cadeia de Caracteres|O URI que pode ser usado para acessar o serviço.|

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

