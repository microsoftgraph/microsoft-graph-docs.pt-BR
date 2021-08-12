---
title: Tipo de recurso educationFeedbackOutcome
description: Um educationOutcome que fornece comentários na forma de texto.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5d3e28fa7ee3157a1cf05b2fcf4818878e292702738c5b3e813bccbf39caff9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146920"
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

