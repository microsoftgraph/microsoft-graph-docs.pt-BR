---
title: Tipo de recurso educationSubmissionResource
description: Um wrapper em torno de um recurso para uso em um envio.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b24f1ea91691dd66d66848abcdb0069e9a25e4865f18f05b7682d2fb4a8f3d88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141746"
---
# <a name="educationsubmissionresource-resource-type"></a>Tipo de recurso educationSubmissionResource

Namespace: microsoft.graph

Um wrapper em torno de um recurso para uso em um envio. 

O wrapper adiciona um ponteiro ao recurso de atribuição se ele foi copiado da atribuição.  


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter educationSubmissionResource](../api/educationsubmissionresource-get.md) | [educationSubmissionResource](educationsubmissionresource.md) |Leia propriedades e relações de um **objeto educationSubmissionResource.**|
|[Delete](../api/educationsubmissionresource-delete.md) | None |**Exclua um objeto educationSubmissionResource.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignmentResourceUrl|String|Ponteiro para a atribuição da qual esse recurso foi copiado. Se for nulo, o aluno carregará o recurso.|
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


