---
title: tipo de recurso de outlookTaskGroup
description: 'Um grupo de pastas (outlookTaskFolder) que contêm tarefas do Outlook (coleção de objetos outlookTask). '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d1392e07f76d508fe30307294a54429a692f34e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923905"
---
# <a name="outlooktaskgroup-resource-type"></a>tipo de recurso de outlookTaskGroup

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um grupo de pastas ([outlookTaskFolder](outlooktaskfolder.md)) que contêm tarefas do Outlook (coleção de objetos [outlookTask](outlooktask.md) ). 

No Outlook, há um grupo de tarefas padrão `My Tasks` que não é possível renomear ou excluir. No entanto, você pode criar grupos de tarefas adicionais. 


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter outlookTaskGroup](../api/outlooktaskgroup-get.md) | [outlookTaskGroup](outlooktaskgroup.md) |Obtenha as propriedades e relacionamentos do grupo de tarefas especificado do Outlook.|
|[Criar outlookTaskFolder](../api/outlooktaskgroup-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Crie uma pasta de tarefas do Outlook.|
|[Lista taskFolders](../api/outlooktaskgroup-list-taskfolders.md) |coleção [outlookTaskFolder](outlooktaskfolder.md)| Obtenha uma coleção de pastas de tarefas do Outlook.|
|[Update](../api/outlooktaskgroup-update.md) | [outlookTaskGroup](outlooktaskgroup.md)  |Atualize as propriedades graváveis de um grupo de tarefa do Outlook. |
|[Delete](../api/outlooktaskgroup-delete.md) | Nenhum |Exclua o grupo de tarefas do Outlook especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|changeKey|Cadeia de caracteres|A versão do grupo de tarefas.|
|groupKey|Edm.Guid|O identificador GUID exclusivo para o grupo de tarefa.|
|id|Cadeia de caracteres|O identificador de cadeia de caracteres exclusiva do grupo de tarefas. Somente leitura.|
|isDefaultGroup|Booliano|True se o grupo de tarefa é o grupo de tarefas padrão.|
|name|Cadeia de caracteres|O nome do grupo de tarefas.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|taskFolders|coleção [outlookTaskFolder](outlooktaskfolder.md)| A coleção de pastas de tarefa no grupo de tarefas. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTaskGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
