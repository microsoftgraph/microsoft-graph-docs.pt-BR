---
title: Tipo de recurso educationRubric
description: Uma rubrica de classificação que pode ser anexada a uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2e5c9713de4da614c8bfb0f6332930edb8ad775b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721576"
---
# <a name="educationrubric-resource-type"></a>Tipo de recurso educationRubric

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma rubrica de classificação que pode ser anexada a uma atribuição. Uma rubrica é associada a um **educationUser** (professor) e anexada a um ou mais recursos **educationAssignment.** 

Consulte [Education rubric overview para](/graph/education-rubric-overview) obter mais informações.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar educationRubric](../api/educationuser-post-rubrics.md) | [educationRubric](educationrubric.md) | Crie um novo objeto educationRubric. |
| [Obter educationRubric](../api/educationrubric-get.md) | [educationRubric](educationrubric.md) | Ler propriedades e relações do objeto educationRubric. |
| [Atualizar educationRubric](../api/educationrubric-update.md) | [educationRubric](educationrubric.md) | Atualize o objeto educationRubric. |
| [Excluir educationRubric](../api/educationrubric-delete.md) | Nenhum(a) | Exclua o objeto educationRubric. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy|[identitySet](identityset.md)|O usuário que criou esse recurso.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|description|[itemBody](itembody.md)|A descrição dessa rubrica.|
|displayName|Cadeia de caracteres|O nome dessa rubrica.|
|grading|[educationAssignmentGradeType](educationassignmentgradetype.md)|O tipo de classificação dessa rubrica -- nulo para uma rubrica sem pontos ou [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) para um rubric de pontos.|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no tempo em que o recurso foi modificado pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|levels|[Coleção rubricLevel](rubriclevel.md)|A coleção de níveis que comem essa rubrica.|
|qualidades|[Coleção rubricQuality](rubricquality.md)|A coleção de qualidades que com isso é rubrica.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [{"@odata.type": "microsoft.graph.rubricLevel"}],
  "qualities": [{"@odata.type": "microsoft.graph.rubricQuality"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubric resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->