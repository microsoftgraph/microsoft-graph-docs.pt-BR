---
title: tipo de recurso inferenceData
description: tipo de recurso inferenceData
localization_priority: Normal
author: kevinbellinger
ms.prod: profile
doc_type: resourcePageType
ms.openlocfilehash: 2097dc14de984f3d1517b4d17e8043f38411b89a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496170"
---
# <a name="inferencedata-resource-type"></a>tipo de recurso inferenceData

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso [inferenceData](inferencedata.md) fornece detalhes adicionais sobre uma entidade que foi criada através de informações de referência sobre o usuário. Essas informações estarão presentes sempre que os dados dentro de uma entidade específica tiverem sido derivados de uma máquina de aprendizado ou de outro processo de sistema Iterando sobre os dados.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo        | Descrição                                                                     |
|:----------------------|:------------|:--------------------------------------------------------------------------------|
|confidenceScore        |Duplo       | A pontuação de confiança reflete a precisão dos dados inferidos sobre o usuário.   |
|userHasVerifiedAccuracy|Boolean      | Registros se o usuário confirmou essa inferência como true ou false.        |

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