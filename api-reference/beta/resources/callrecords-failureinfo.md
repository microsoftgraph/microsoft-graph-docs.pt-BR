---
title: tipo de recurso failureInfo
description: O tipo failureInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5edd2a501b3e1a5633f0bd01ac36815201eb927d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064371"
---
# <a name="failureinfo-resource-type"></a>tipo de recurso failureInfo

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre o motivo pelo qual uma chamada ou parte de uma chamada falhou.

A falha pode ser de dois tipos: 

- Falha de configuração de chamada
- Queda de chamada intermediário

Se um ou mais fluxos de mídia tiverem qualquer uma dessas falhas, essa falha será propagada no nível do segmento. Se um ou mais segmentos tiverem qualquer uma dessas falhas, essa falha será propagada no nível da sessão.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|motivo|Cadeia de caracteres|Classificação de por que uma chamada ou parte de uma chamada falhou.|
|estágio|Microsoft. Graph. callRecords. failureStage|O estágio quando a falha ocorreu. Os valores possíveis são: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.failureInfo",
  "baseType": null
}-->

```json
{
  "reason": "String",
  "stage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "failureInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


