---
title: Tipo de recurso addLargeGalleryViewOperation
description: Descreve o formato de resposta para uma operação que adiciona o modo de exibição de galeria grande.
author: navali-msft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 312f3ea1d9c924e142e6b192a7f6542cc6e0cd19
ms.sourcegitcommit: 4ff6e89e89178cbd5aef8aa019e714d95817fae4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2022
ms.locfileid: "65017030"
---
# <a name="addlargegalleryviewoperation-resource-type"></a>Tipo de recurso addLargeGalleryViewOperation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o formato de resposta para uma operação que adiciona o modo de exibição de galeria grande.

Herda de [commsOperation](commsoperation.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-|:-|:-|
| [Obter addLargeGalleryViewOperation](../api/addlargegalleryviewoperation-get.md) | [addLargeGalleryViewOperation](addlargegalleryviewoperation.md) | Obtenha o status de uma operação que adiciona o modo de exibição de galeria grande a uma chamada. |

## <a name="properties"></a>Propriedades

| Propriedade                       | Tipo                        | Descrição                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | Cadeia de caracteres                      | O contexto do cliente.                                                                                                                               |
| id                             | Cadeia de caracteres                      | A ID da operação do servidor. Somente leitura.                                                                                             |
| resultInfo                     | [resultInfo](resultinfo.md) | As informações de resultado.  Somente leitura.                                                                                             |
| status                         | operationStatus             | O status da operação. Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`. Somente leitura.                                                 |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addLargeGalleryViewOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addLargeGalleryViewOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


