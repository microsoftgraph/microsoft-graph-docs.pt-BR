---
title: tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar uma mudança por outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a172737f40572b29358ecdc6fba804db2a8b80e5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951955"
---
# <a name="swapshiftschangerequest-resource-type"></a>tipo de recurso swapShiftsChangeRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de solicitação de mudança para trocar uma [mudança](../resources/shift.md) por outro usuário na [equipe](../resources/team.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/swapshiftschangerequest-list.md) | Coleção de [swapShiftsChangeRequest](swapshiftschangerequest.md) | Listar as propriedades e os relacionamentos dos objetos **swapShiftsChangeRequest** em uma equipe. |
| [Create](../api/swapshiftschangerequest-post.md) | [swapshiftschangerequest](swapshiftschangerequest.md) | Criar uma instância de um objeto swapshiftschangerequest. |
| [Get](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Leia as propriedades e os relacionamentos de um objeto **swapShiftsChangeRequest** . |
|[Aprovar](../api/swapshiftschangerequest-approve.md)|Nenhum|Aprovar um swapshiftschangerequest. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientShiftId|String|ID do destinatário da solicitação de troca. Esse é o usuário com o qual a solicitação deve ser trocada.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest",
  "baseType": ""
}-->

```json
{
  "recipientShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftsChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
