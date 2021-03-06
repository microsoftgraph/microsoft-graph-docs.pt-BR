---
title: tipo de recurso outlookTaskGroup
description: 'Um grupo de pastas (outlookTaskFolder) que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f2ddf43dbbe580b74e69d3f3d85ef226de673a54
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998352"
---
# <a name="outlooktaskgroup-resource-type-deprecated"></a>tipo de recurso outlookTaskGroup (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


Um grupo de pastas ([outlookTaskFolder](outlooktaskfolder.md)) que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ). 

No Outlook, há um grupo de tarefas padrão `My Tasks` que você não pode renomear ou excluir. No entanto, você pode criar grupos de tarefas adicionais. 


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.|
|[Criar outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Criar uma pasta de tarefas do Outlook.|
|[Listar taskFolders](../api/outlooktaskgroup-list-taskfolders.md) |coleção [outlookTaskFolder](outlooktaskfolder.md)| Obter uma coleção de pastas de tarefas do Outlook.|
|[Atualização](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |Atualizar as propriedades graváveis de um grupo de tarefas do Outlook. |
|[Delete](../api/outlooktaskgroup-delete.md) | Nenhum |Excluir o grupo de tarefas do Outlook especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|changeKey|String|A versão do grupo de tarefas.|
|groupKey|Edm.Guid|O identificador exclusivo do GUID do grupo de tarefas.|
|id|String|O identificador exclusivo da cadeia de caracteres do grupo de tarefas. Somente leitura.|
|IsDefault|Boolean|True se o grupo de tarefas é o grupo de tarefas padrão.|
|nome|String|O nome do grupo de tarefas.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|taskFolders|coleção [outlookTaskFolder](outlooktaskfolder.md)| O conjunto de pastas de tarefas no grupo de tarefas. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}-->

```json
{
  "changeKey": "String",
  "groupKey": "Guid",
  "id": "String (identifier)",
  "isDefaultGroup": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


