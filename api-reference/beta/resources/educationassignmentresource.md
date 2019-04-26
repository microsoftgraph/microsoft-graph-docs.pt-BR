---
title: tipo de recurso educationAssignmentResource
description: Um objeto envoltório que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica que este recurso irá
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 08a716edabc31c83a7fb3e358fbafd023d5fa784
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334405"
---
# <a name="educationassignmentresource-resource-type"></a>tipo de recurso educationAssignmentResource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto envoltório que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica que esse recurso será copiado para o envio do aluno.  Se o objeto não for copiado, cada aluno verá um link para o recurso na atribuição. O aluno não poderá atualizar esse recurso. Este é um folheto do professor para o aluno com nada para ser ativado. Se o recurso for distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos do envio. Cada aluno poderá modificar a cópia e enviá-la para a gradação.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |Ler propriedades e relações de um objeto **educationAssignmentResource** .|
|[Atualizar](../api/educationassignmentresource-update.md) | [educationAssignmentResource](educationassignmentresource.md) |Atualize um objeto **educationAssignmentResource** . |
|[Delete](../api/educationassignmentresource-delete.md) | Nenhuma |Excluir um objeto **educationAssignmentResource** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|distributeForStudentWork|Boolean|Indica se esse recurso deve ser copiado para cada aluno enviado para modificação e envio.|
|id|String| ID desse recurso. Somente leitura.|
|recurso|[educationResource](educationresource.md)|Objeto de recurso que foi associado a essa atribuição.|

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
  "suppressions": []
}
-->
