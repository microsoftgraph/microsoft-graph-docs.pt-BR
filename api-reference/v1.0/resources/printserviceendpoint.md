---
title: Tipo de recurso printServiceEndpoint
description: Representa o URI e a identificação de informações para uma instância de serviço de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7534e538c81c543671d996c7765125eafcad9d67cddbb13ad406d06edb8b9912
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178035"
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

