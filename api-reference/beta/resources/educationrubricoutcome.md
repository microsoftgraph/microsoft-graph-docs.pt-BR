---
title: Tipo de recurso educationRubricOutcome
description: Um educationOutcome que fornece um rubric de notas
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c8132159fa70c175a46a43a13ebce981299f2431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161905"
---
# <a name="educationrubricoutcome-resource-type"></a>Tipo de recurso educationRubricOutcome

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um [educationOutcome](educationoutcome.md) que fornece um rubric de notas.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Atualizar educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Atualize o objeto educationOutcome. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no tempo em que o recurso foi modificado pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|publishedRubricQualityFeedback|[Coleção rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Uma cópia da propriedade rubricQualityFeedback que é feita quando a nota é liberada para o aluno.|
|publishedRubricQualitySelectedLevels|[Coleção rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|Uma cópia da propriedade rubricQualitySelectedLevels que é feita quando a nota é liberada para o aluno.|
|rubricQualityFeedback|[Coleção rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Uma coleção de comentários específicos para cada qualidade dessa rubric.|
|rubricQualitySelectedLevels|[Coleção rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|O nível que o professor selecionou para cada qualidade durante a gradação dessa atribuição.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
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

