---
title: Tipo de recurso printServiceEndpoint
description: Representa o URI e a identificação de informações para uma instância de serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 0dd339d433be593e6982b6c38818635830a2d471
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516862"
---
# <a name="printserviceendpoint-resource-type"></a>Tipo de recurso printServiceEndpoint

Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Representa o URI e a identificação de informações para uma instância de serviço de impressão.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
| [Obter o ponto de extremidade](../api/printserviceendpoint-get.md) | [printServiceEndpoint](printserviceendpoint.md) | Leia as propriedades e as relações do objeto endpoint. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Um nome de exibição acessível para humanos para o ponto de extremidade.|
|id|Cadeia de caracteres|Um nome exclusivo que identifica o serviço que o ponto de extremidade fornece. Os valores possíveis são: `discovery` (Serviço de Descoberta), `notification` (Serviço de Notificação), `ipp` (Serviço IPP) e `registration` (Serviço de Registro). Somente leitura.|
|uri|Cadeia de caracteres|O URI que pode ser usado para acessar o serviço.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "String (identifier)",
  "displayName": "String",
  "uri": "String"
}
```

