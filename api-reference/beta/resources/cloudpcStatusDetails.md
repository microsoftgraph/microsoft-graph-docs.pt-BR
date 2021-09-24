---
title: Tipo de recurso cloudPcStatusDetails
description: Os detalhes do status do computador na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ae9054e92279d976d65aafc72ac2c38190c88b84
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507813"
---
# <a name="cloudpcstatusdetails-resource-type"></a>Tipo de recurso cloudPcStatusDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os detalhes do status do computador na nuvem.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|Cadeia de caracteres|O código associado ao status do computador na nuvem.|
|mensagem|String|A mensagem de status.|
|additionalInformation|[Coleção KeyValuePair](../resources/keyvaluepair.md)|Qualquer informação adicional sobre o status do computador na nuvem.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcStatusDetails",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcStatusDetails",
  "code": "String",
  "message": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```
