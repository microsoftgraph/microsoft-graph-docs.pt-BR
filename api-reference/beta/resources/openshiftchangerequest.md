---
title: Tipo de recurso openShiftChangeRequest
description: Representa um tipo de solicitação de turno para reivindicar um turno aberto em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e141dcb6657c9efc7d751b1713aa8b53d79c9264
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161415"
---
# <a name="openshiftchangerequest-resource-type"></a>Tipo de recurso openShiftChangeRequest

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de solicitação de turno para [reivindicar uma abertura](../resources/openshift.md) em um [cronograma.](../resources/schedule.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar](../api/openshiftchangerequest-post.md) | [openshiftchangerequest](openshiftchangerequest.md) | Crie uma instância de um objeto openshiftchangerequest. |
| [Lista](../api/openshiftchangerequest-list.md) | Coleção de [openshiftchangerequest](openshiftchangerequest.md) | Listar as propriedades e os relacionamentos dos **objetos openShiftChangeRequest** em uma equipe. |
| [Get](../api/openshiftchangerequest-get.md) | [openShiftChangeRequest](openshiftchangerequest.md) | Leia as propriedades e os relacionamentos de um **objeto openShiftChangeRequest.** |
|[Aprovar](../api/openshiftchangerequest-approve.md)|Nenhum(a)|Aprovar uma solicitação de alteração de turno aberto.|
|[Recusar](../api/openshiftchangerequest-decline.md)|Nenhum(a)| Recusar uma solicitação de alteração de turno aberto.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|openShiftId|String| ID do turno aberto.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
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


