---
title: Tipo de recurso educationFeedbackResourceOutcome
description: Representa comentários sobre um objeto educationOutcome na forma de um documento.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0cad7a6e8c2f0527dd89ce624fac5652c6ac544b
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900539"
---
# <a name="educationfeedbackresourceoutcome-resource-type"></a>Tipo de recurso educationFeedbackResourceOutcome

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa comentários sobre [um objeto educationOutcome](educationoutcome.md) na forma de um documento.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar educationFeedbackResourceOutcome](../api/educationfeedbackresourceoutcome-post-outcomes.md) | [educationOutcome](educationoutcome.md) | Crie um novo [recurso de comentários](../resources/educationfeedbackresourceoutcome.md) para um envio. |
| [Excluir educationFeedbackResourceOutcome](../api/educationfeedbackresourceoutcome-delete.md) | Nenhum | Exclua [um recurso de comentários](../resources/educationfeedbackresourceoutcome.md) de um envio. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|feedbackResource|[educationResource](educationresource.md)|O recurso de comentários real.|
|id|String|Identificador exclusivo para **educationFeedbackResourceOutcome**.|
|resourceStatus|educationFeedbackResourceOutcomeStatus|O status do recurso de comentários. Os valores possíveis são: `notPublished`, `pendingPublish`, `published`, `failedPublish`e `unknownFutureValue`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackResourceOutcome",
  "keyProperty": "id"
}-->

```json
{
  "feedbackResource": {"@odata.type": "microsoft.graph.educationResource"},
  "id": "String (identifier)",
  "resourceStatus": {"@odata.type": "microsoft.graph.educationFeedbackResourceOutcomeStatus"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2022-05-05 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackResourceOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
