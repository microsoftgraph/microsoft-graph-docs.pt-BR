---
title: tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar uma mudança por outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3a18b3627aec777bf95ece65cd26a170d6f98ad7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056440"
---
# <a name="swapshiftschangerequest-resource-type"></a>tipo de recurso swapShiftsChangeRequest

Namespace: microsoft.graph

Representa um tipo de solicitação de mudança para trocar uma [mudança](../resources/shift.md) por outro usuário na [equipe](../resources/team.md).

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/swapshiftschangerequest-list.md) | Coleção de [swapShiftsChangeRequest](swapshiftschangerequest.md) | Listar as propriedades e os relacionamentos dos objetos **swapShiftsChangeRequest** em uma equipe. |
| [Create](../api/swapshiftschangerequest-post.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Criar uma instância de um objeto **swapShiftsChangeRequest** . |
| [Get](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Leia as propriedades e os relacionamentos de um objeto **swapShiftsChangeRequest** . |
|[Aprovar](../api/swapshiftschangerequest-approve.md)|Nenhum|Aprovar um **swapShiftsChangeRequest**. |
|[Aceito](../api/swapshiftschangerequest-decline.md)|Nenhum|Recusar um **swapShiftsChangeRequest**.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientShiftId|String|ShiftID do usuário do destinatário com o qual a solicitação deve ser trocada.|

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

