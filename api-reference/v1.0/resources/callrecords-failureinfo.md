---
title: Tipo de recurso failureInfo
description: O tipo failureInfo
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 86309f5ea3d9ff31e605ecdd39c98b644cf680ae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025570"
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
