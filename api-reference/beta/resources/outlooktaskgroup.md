---
title: tipo de recurso outlookTaskGroup
description: 'Um grupo de pastas (outlookTaskFolder) que contém tarefas do Outlook (coleção de objetos outlookTask). '
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8018863ed7fd142b99e0008f860495a4d13d4e01
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463207"
---
# <a name="outlooktaskgroup-resource-type"></a>tipo de recurso outlookTaskGroup

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um grupo de pastas ([outlookTaskFolder](outlooktaskfolder.md)) que contém tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ). 

No Outlook, há um grupo `My Tasks` de tarefas padrão que você não pode renomear ou excluir. No entanto, você pode criar grupos de tarefas adicionais. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |Obtenha as propriedades e os relacionamentos do grupo de tarefas especificado do Outlook.|
|[Criar outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Criar uma pasta de tarefas do Outlook.|
|[Listar taskFolders](../api/outlooktaskgroup-list-taskfolders.md) |coleção [outlookTaskFolder](outlooktaskfolder.md)| Obter uma coleção de pastas de tarefas do Outlook.|
|[Atualizar](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |Atualizar as propriedades graváveis de um grupo de tarefas do Outlook. |
|[Excluir](../api/outlooktaskgroup-delete.md) | Nenhum |Excluir o grupo de tarefas do Outlook especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|changeKey|String|A versão do grupo de tarefas.|
|groupKey|Edm.Guid|O identificador exclusivo do GUID do grupo de tarefas.|
|id|String|O identificador exclusivo da cadeia de caracteres do grupo de tarefas. Somente leitura.|
|IsDefault|Booliano|True se o grupo de tarefas é o grupo de tarefas padrão.|
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
