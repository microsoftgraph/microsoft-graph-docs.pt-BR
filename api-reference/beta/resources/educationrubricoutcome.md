---
title: tipo de recurso educationRubricOutcome
description: Um educationOutcome que fornece uma amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 93e6585a6963a6f31c2613e2f2e12cce7246b7d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501007"
---
# <a name="educationrubricoutcome-resource-type"></a>tipo de recurso educationRubricOutcome

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um [educationOutcome](educationoutcome.md) que fornece um amostra rubric com a classificação.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Atualizar educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Atualize o objeto educationOutcome. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no momento em que o recurso foi modificado pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|publishedRubricQualityFeedback|coleção [rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Uma cópia da propriedade rubricQualityFeedback que é feita quando a nota é liberada para o aluno.|
|publishedRubricQualitySelectedLevels|coleção [rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|Uma cópia da propriedade rubricQualitySelectedLevels que é feita quando a nota é liberada para o aluno.|
|rubricQualityFeedback|coleção [rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Uma coleção de comentários específicos para cada qualidade desse amostra rubric.|
|rubricQualitySelectedLevels|coleção [rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|O nível que o professor selecionou para cada qualidade e, ao mesmo tempo, grada esta atribuição.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "publishedRubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "publishedRubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}],
  "rubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "rubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubricOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->