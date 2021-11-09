---
title: Tipo de recurso cloudPcStatusDetails
description: Os detalhes do status do computador na nuvem.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 28735467ef1bc233f5ba6d5ecc3144d64e31df3e
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780895"
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
|additionalInformation|[Coleção KeyValuePair](../resources/keyvaluepair.md)|Quaisquer informações adicionais sobre o status do computador na nuvem.|

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
