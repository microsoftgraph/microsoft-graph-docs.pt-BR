---
title: tipo de recurso de educationAssignmentResource
description: Um objeto wrapper que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica as datas que este recurso será
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529226"
---
# <a name="educationassignmentresource-resource-type"></a>tipo de recurso de educationAssignmentResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto wrapper que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica as datas que este recurso será copiado para o envio de student.  Se o objeto não for copiado, a cada aluno verão um link para o recurso na atribuição. O aluno não poderão atualizar esse recurso. Este é um folheto do professor ao aluno com nada a ser ativado. Se o recurso é distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos de envio. Cada aluno poderá modificar suas cópias e enviá-la para a classificação.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |Leia as propriedades e os relacionamentos de um objeto **educationAssignmentResource** .|
|[Update](../api/educationassignmentresource-update.md) | [educationAssignmentResource](educationassignmentresource.md) |Atualize um objeto **educationAssignmentResource** . |
|[Delete](../api/educationassignmentresource-delete.md) | Nenhum |Exclua um objeto **educationAssignmentResource** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|distributeForStudentWork|Booliano|Indica se este recurso deve ser copiado para cada envio estudante para envio e modificação.|
|id|String| Identificação desse recurso. Somente leitura.|
|recurso|[educationResource](educationresource.md)|Objeto de recurso que tiver sido associado essa atribuição.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
