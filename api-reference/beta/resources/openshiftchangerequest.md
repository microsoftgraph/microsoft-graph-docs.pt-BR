---
title: tipo de recurso openShiftChangeRequest
description: Representa um tipo de solicitação de mudança para declarar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 400444ccccc13d103420cc95c522a6ed0aa1afa6
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895569"
---
# <a name="openshiftchangerequest-resource-type"></a>tipo de recurso openShiftChangeRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de solicitação de mudança para declarar um [openshift](../resources/openshift.md) em um [cronograma](../resources/schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Get](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Leia as propriedades e os relacionamentos de um objeto **openShiftChangeRequest** . |
| [Update](../api/openshiftchangerequest-update.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Atualize um objeto **openShiftChangeRequest** . |
| [Delete](../api/openshiftchangerequest-delete.md) | None | Excluir um objeto **openShiftChangeRequest** . |
|[Aprovar](../api/openshiftchangerequest-approve.md)|Nenhum|Aprovar uma solicitação de alteração de turno aberta.|
|[Aceito](../api/openshiftchangerequest-decline.md)|Nenhum| Recusar uma solicitação de alteração de turno aberto.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|openShiftId|String| ID para o turno aberto.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest",
  "baseType": ""
}-->

```json
{
  "openShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
