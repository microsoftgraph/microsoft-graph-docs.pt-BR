---
title: tipo de recurso cloudPcStatusDetails
description: Os detalhes do status do PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 647c13878e054fbac6c1f43f565bd2788d19a9de
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378265"
---
# <a name="cloudpcstatusdetails-resource-type"></a>tipo de recurso cloudPcStatusDetails

Namespace: microsoft.graph

Os detalhes do status do PC de nuvem.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|código|Cadeia de Caracteres|O código associado ao status do PC de nuvem.|
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
