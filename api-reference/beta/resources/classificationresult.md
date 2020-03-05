---
title: tipo de recurso classificationResult
description: Representa o resultado de uma solicitação de classificação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5281156752ceb290772daf841530b4ddb80350d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507660"
---
# <a name="classificationresult-resource-type"></a>tipo de recurso classificationResult

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o resultado de uma operação de classificação do mecanismo de classificação da Microsoft. Os resultados de classificação de dados da proteção de informações do Azure, Office e outros serviços da Microsoft podem retornar um [conjunto bem definido de tipos de classificação](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for). Esses tipos podem ser fornecidos para a API [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) para resolver informações confidenciais em um rótulo de proteção de informações da Microsoft. 

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo  | Descrição                                                            |
| :-------------- | :---- | :--------------------------------------------------------------------- |
| confidenceLevel | Int32 | O nível de confiança, de 0 a 100, do resultado.                         |
| Count           | Int32 | O número de instâncias do tipo de informação específico na entrada. |
| sensitiveTypeId | GUID  | O GUID do tipo de informação confidencial descoberto.                 |

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
