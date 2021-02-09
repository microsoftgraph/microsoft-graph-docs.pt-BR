---
title: Tipo de recurso educationRubric
description: Um rubric de gradação que pode ser anexado a uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 37e1d4a6267f1f1292a72cc7f34b8135483091ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161933"
---
# <a name="educationrubric-resource-type"></a>Tipo de recurso educationRubric

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um rubric de gradação que pode ser anexado a uma atribuição. Um rubric é associado a **um educationUser** (professor) e anexado a um ou mais **recursos educationAssignment.** 

Confira [a visão geral do rubric educacional](/graph/education-rubric-overview) para obter mais informações.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar educationRubric](../api/educationuser-post-rubrics.md) | [educationRubric](educationrubric.md) | Crie um novo objeto educationRubric. |
| [Obter educationRubric](../api/educationrubric-get.md) | [educationRubric](educationrubric.md) | Leia as propriedades e os relacionamentos do objeto educationRubric. |
| [Atualizar educationRubric](../api/educationrubric-update.md) | [educationRubric](educationrubric.md) | Atualize o objeto educationRubric. |
| [Excluir educationRubric](../api/educationrubric-delete.md) | Nenhum(a) | Exclua o objeto educationRubric. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy|[identitySet](identityset.md)|O usuário que criou esse recurso.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|description|[itemBody](itembody.md)|A descrição desse rubric.|
|displayName|String|O nome dessa rubric.|
|grading|[educationAssignmentGradeType](educationassignmentgradetype.md)|O tipo de gradação desse rubric – nulo para um rubric sem pontos ou [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) para um rubric de pontos.|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no tempo em que o recurso foi modificado pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|níveis|[Coleção rubricLevel](rubriclevel.md)|A coleção de níveis que comem esse rubric.|
|qualities|[coleção rubricQuality](rubricquality.md)|A coleção de qualidades que com o mesmo rubric.|

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