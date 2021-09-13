---
title: Tipo de recurso educationOutcome
description: O resultado da classificação de uma atribuição.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bc600835885037177df3a4e1039a2c6b1ad052ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036624"
---
# <a name="educationoutcome-resource-type"></a>Tipo de recurso educationOutcome

Namespace: microsoft.graph

O resultado da classificação de uma atribuição. 

Esta é uma classe base; os tipos derivados [são educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md)e [educationRubricOutcome](educationrubricoutcome.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Atualizar educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Atualizar o objeto educationOutcome. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

