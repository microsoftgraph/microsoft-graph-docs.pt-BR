---
title: Tipo de recurso educationRubricOutcome
description: Um educationOutcome que fornece uma rubrica de notas.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 831cac7de7510ebc83cf6dc0ddbf5190d1e3d9d9
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685065"
---
# <a name="educationrubricoutcome-resource-type"></a>Tipo de recurso educationRubricOutcome

Namespace: microsoft.graph

Um [educationOutcome](educationoutcome.md) que fornece uma rubrica de notas.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Atualizar educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Atualize o objeto educationOutcome. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|Identificador exclusivo para educationRubricOutcome.|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no tempo em que o recurso foi modificado pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|publishedRubricQualityFeedback|[Coleção rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Uma cópia da propriedade rubricQualityFeedback que é feita quando a nota é liberada para o aluno.|
|publishedRubricQualitySelectedLevels|[Coleção rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|Uma cópia da propriedade rubricQualitySelectedLevels que é feita quando a nota é liberada para o aluno.|
|rubricQualityFeedback|[Coleção rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Uma coleção de comentários específicos para cada qualidade dessa rubrica.|
|rubricQualitySelectedLevels|[Coleção rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|O nível que o professor selecionou para cada qualidade ao classificar essa tarefa.|

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
  "id": "String (identifier)",
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

