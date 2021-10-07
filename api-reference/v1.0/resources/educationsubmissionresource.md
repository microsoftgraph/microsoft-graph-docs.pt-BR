---
title: Tipo de recurso educationSubmissionResource
description: Um wrapper em torno de um recurso para uso em um envio.
author: sharad-sharma-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0663fb168100d3dcded42dcd621650899d8b72a9
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220749"
---
# <a name="educationsubmissionresource-resource-type"></a>Tipo de recurso educationSubmissionResource

Namespace: microsoft.graph

Um wrapper em torno de um recurso para uso em um envio. 

O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.  


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar recursos](../api/educationsubmission-list-resources.md) | [objetos educationSubmissionResource](educationsubmissionresource.md) |Retorna uma lista de **objetos educationSubmissionResource.**|
|[Obter educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |Leia propriedades e relações de um **objeto educationSubmissionResource.**|
|[Excluir](../api/educationsubmissionresource-delete.md) | Nenhum |**Exclua um objeto educationSubmissionResource.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignmentResourceUrl|Cadeia de caracteres|Ponteiro para a atribuição da qual esse recurso foi copiado. Se for nulo, o aluno carregará o recurso.|
|id|String| Somente leitura.|
|recurso|[educationResource](educationresource.md)|Objeto Resource.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


