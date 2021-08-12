---
title: Tipo de recurso rubricQuality
description: Uma qualidade de uma rubrica.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6230732caf190bc255f63e7eee79af6971d3e4a805f1ead94332c13b6115555b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54211847"
---
# <a name="rubricquality-resource-type"></a>Tipo de recurso rubricQuality

Namespace: microsoft.graph

Uma qualidade de uma rubrica. 

Consulte [educationRubric](educationrubric.md) para ver uma descrição da relação entre as qualidades *rubricas,* níveis e *critérios.*

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|criteria|[Coleção rubricCriterion](rubriccriterion.md)|A coleção de critérios para essa qualidade rubrica.|
|description|[itemBody](itembody.md)|A descrição dessa qualidade rubrica.|
|displayName|Cadeia de caracteres|O nome dessa qualidade rubrica.|
|qualityId|Cadeia de caracteres|A ID desse recurso.|
|weight|Único|Se presente, um peso numérico para essa qualidade.  Os pesos devem adicionar até 100.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

