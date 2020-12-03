---
title: tipo de recurso cloudPcStatusDetails
description: Os detalhes do status do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61260bc7f3437fe1f10575afc616462eec2e47dc
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563828"
---
# <a name="cloudpcstatusdetails-resource-type"></a>tipo de recurso cloudPcStatusDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os detalhes do status do PC de nuvem.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|String|O código associado ao status do PC de nuvem.|
|mensagem|String|A mensagem de status.|
|additionalInformation|Coleção [KeyValuePair](../resources/keyvaluepair.md)|Informações adicionais sobre o status do PC de nuvem.|

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
