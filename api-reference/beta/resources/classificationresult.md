---
title: Tipo de recurso classificationResult
description: Representa o resultado de uma solicitação de classificação.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5ecc16197ef4671c6e83883bc69aed45b3ffa200
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941817"
---
# <a name="classificationresult-resource-type"></a>Tipo de recurso classificationResult

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado de uma operação de classificação do Mecanismo de Classificação da Microsoft. Os resultados da classificação de dados da Proteção de Informações do Azure, do Office e de outros serviços da Microsoft podem retornar um conjunto bem [definido de tipos de classificação.](/office365/securitycompliance/what-the-sensitive-information-types-look-for) Esses tipos podem ser fornecidos à API [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) para resolver uma informação confidenciais para um rótulo de Proteção de Informações da Microsoft. 

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo  | Descrição                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| confidenceLevel | Int32 | O nível de confiança, de 0 a 100, do resultado.                         |
| Count           | Int32 | O número de instâncias do tipo de informação específico na entrada. |
| sensitiveTypeId | GUID  | O GUID do tipo de informação confidenciais descoberto.                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.classificationResult",
  "baseType": null
}-->

```json
{
  "confidenceLevel": 1024,
  "count": 1024,
  "sensitiveTypeId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "classificationResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->