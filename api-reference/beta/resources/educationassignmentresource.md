---
title: tipo de recurso de educationAssignmentResource
description: Um objeto wrapper que armazena os recursos associados a uma atribuição. O wrapper adiciona a propriedade **distributeForStudentWork** e indica as datas que este recurso será
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb0879737d0375bf2463268fe29f2c98f2b6ed51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991346"
---
# <a name="educationassignmentresource-resource-type"></a>tipo de recurso de educationAssignmentResource

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
|id|Cadeia de caracteres| Identificação desse recurso. Somente leitura.|
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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
