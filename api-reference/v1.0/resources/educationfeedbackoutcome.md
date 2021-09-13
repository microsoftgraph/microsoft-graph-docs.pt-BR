---
title: Tipo de recurso educationFeedbackOutcome
description: Um educationOutcome que fornece comentários na forma de texto.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 120e7b603ca1d441b696e0fe50c64cb5d0373b7f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036652"
---
# <a name="educationfeedbackoutcome-resource-type"></a>Tipo de recurso educationFeedbackOutcome

Namespace: microsoft.graph

Representa comentários em [um objeto educationOutcome](educationoutcome.md) na forma de texto. 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Atualizar educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Atualizar o objeto educationOutcome. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|comentários|[educationFeedback](educationfeedback.md)|Comentários escritos do professor para o aluno.|
|publishedFeedback|[educationFeedback](educationfeedback.md)|Uma cópia da propriedade feedback que é feita quando a nota é liberada para o aluno.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "keyProperty": "id"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "publishedFeedback": {"@odata.type": "microsoft.graph.educationFeedback"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

