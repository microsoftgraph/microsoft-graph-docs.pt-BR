---
title: Tipo de recurso educationAssignmentResource
description: Um objeto wrapper que armazena os recursos associados a uma atribuição.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 671ef56a579eeeba7c2f013310e9034aac7c4dae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036722"
---
# <a name="educationassignmentresource-resource-type"></a>Tipo de recurso educationAssignmentResource

Namespace: microsoft.graph

Um objeto wrapper que armazena os recursos associados a uma atribuição. 

O wrapper adiciona **a propriedade distributeForStudentWork** e indica que esse recurso será copiado para o envio do aluno.  Se o objeto não for copiado, cada aluno verá um link para o recurso na atribuição. O aluno não poderá atualizar esse recurso. Esta é uma apostila do professor para o aluno sem nada para ser entregue. Se o recurso for distribuído, cada aluno receberá uma cópia desse recurso na lista de recursos de seu envio. Cada aluno poderá modificar sua cópia e enviar para a classificação.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationAssignmentResource](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |Leia propriedades e relações de um **objeto educationAssignmentResource.**|
|[Delete](../api/educationassignmentresource-delete.md) | None |**Exclua um objeto educationAssignmentResource.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|distributeForStudentWork|Booliano|Indica se esse recurso deve ser copiado para cada envio de alunos para modificação e envio. Obrigatório|
|id|String| ID desse recurso. Somente leitura.|
|recurso|[educationResource](educationresource.md)|Objeto Resource que foi associado a essa atribuição.|

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


