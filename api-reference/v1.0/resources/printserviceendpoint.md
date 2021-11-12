---
title: Tipo de recurso printServiceEndpoint
description: Representa o URI e a identificação de informações para uma instância de serviço de impressão.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 812e9367be06760e56299bd62c88c154f1c25c49
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60924198"
---
# <a name="printserviceendpoint-resource-type"></a>Tipo de recurso printServiceEndpoint

Namespace: microsoft.graph

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

