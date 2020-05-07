---
title: tipo de recurso openShift
description: Representa um turno aberto não atribuído em um cronograma.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2051dddb78121341d22dc9e3cd20b13178cb81c9
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154988"
---
# <a name="openshift-resource-type"></a>tipo de recurso openShift

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um turno não atribuído e aberto em um [cronograma](../resources/schedule.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List](../api/openshift-list.md) | Coleção de [openShift](openshift.md) | Listar as propriedades e os relacionamentos dos objetos **openShift** em uma equipe.|
| [Create](../api/openshift-post.md) | [openShift](openshift.md) | Criar uma instância de um objeto **openShift** . |
| [Get](../api/openshift-get.md) | [openShift](openshift.md) | Leia as propriedades e os relacionamentos de um objeto **openShift** . |
| [Update](../api/openshift-update.md) | [openShift](openshift.md) | Atualize um objeto **openShift** . |
| [Delete](../api/openshift-delete.md) | None | Excluir um objeto **openShift** . |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|draftOpenShift|[openShiftItem](openshiftitem.md)|Um turno aberto não publicado.|
|schedulingGroupId|Cadeia de caracteres|ID do grupo de agendamento ao qual o turno aberto pertence.|
|sharedOpenShift|[openShiftItem](openshiftitem.md)|Um turno aberto publicado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShift",
  "baseType": ""
}-->

```json
{
  "draftOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"},
  "schedulingGroupId": "String",
  "sharedOpenShift": {"@odata.type": "microsoft.graph.openShiftItem"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
