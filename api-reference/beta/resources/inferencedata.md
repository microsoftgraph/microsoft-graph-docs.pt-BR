---
title: tipo de recurso inferenceData
description: tipo de recurso inferenceData
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 412d96d3eb497681e65dacd2f7a0576b4071a9aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016488"
---
# <a name="inferencedata-resource-type"></a>tipo de recurso inferenceData

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso [inferenceData](inferencedata.md) fornece detalhes adicionais sobre uma entidade que foi criada através de informações de referência sobre o usuário. Essas informações estarão presentes sempre que os dados dentro de uma entidade específica tiverem sido derivados de uma máquina de aprendizado ou de outro processo de sistema Iterando sobre os dados.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo        | Descrição                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|confidenceScore        |Duplo       | A pontuação de confiança reflete a precisão dos dados inferidos sobre o usuário.   |
|userHasVerifiedAccuracy|Booliano      | Registros se o usuário confirmou essa inferência como true ou false.        |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceData",
  "baseType": null
}-->

```json
{
  "confidenceScore": 1024,
  "userHasVerifiedAccuracy": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

