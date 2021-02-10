---
title: Tipo de recurso swapShiftsChangeRequest
description: Representa o tipo de solicitação de turno para trocar de turno com outro usuário na equipe.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5f5d1bb7a520d5d7f64640725a846ef5bc76a0b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154730"
---
# <a name="swapshiftschangerequest-resource-type"></a>Tipo de recurso swapShiftsChangeRequest

Namespace: microsoft.graph

Representa um tipo de solicitação de turno para trocar uma [mudança](../resources/shift.md) com outro usuário na [equipe.](../resources/team.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/swapshiftschangerequest-list.md) | Coleção de [swapShiftsChangeRequest](swapshiftschangerequest.md) | Listar as propriedades e os relacionamentos dos **objetos swapShiftsChangeRequest** em uma equipe. |
| [Criar](../api/swapshiftschangerequest-post.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Crie uma instância de um **objeto swapShiftsChangeRequest.** |
| [Get](../api/swapshiftschangerequest-get.md) | [swapShiftsChangeRequest](swapshiftschangerequest.md) | Leia as propriedades e os relacionamentos de um **objeto swapShiftsChangeRequest.** |
|[Aprovar](../api/swapshiftschangerequest-approve.md)|Nenhum|Aprovar um **swapShiftsChangeRequest**. |
|[Recusar](../api/swapshiftschangerequest-decline.md)|Nenhum|Recusar um **swapShiftsChangeRequest**.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recipientShiftId|Cadeia de caracteres|ShiftId para o usuário do destinatário com o qual a solicitação deve ser trocada.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
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

