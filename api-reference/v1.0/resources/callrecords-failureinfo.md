---
title: Tipo de recurso failureInfo
description: O tipo failureInfo
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cabfe56215863385a55ded34914f78fdd856a0d7f341ac4cde1220f37cab77fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160083"
---
# <a name="failureinfo-resource-type"></a>Tipo de recurso failureInfo

Namespace: microsoft.graph.callRecords

Representa informações sobre por que uma chamada ou parte de uma chamada falhou.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|motivo|Cadeia de caracteres|Classificação do motivo pelo qual uma chamada ou parte de uma chamada falhou.|
|stage|microsoft.graph.callRecords.failureStage|O estágio em que ocorreu a falha. Os valores possíveis são: `unknown`, `callSetup`, `midcall`, `unknownFutureValue`.|

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
