---
title: tipo de recurso tasks
description: Representa o To Do de tarefas disponíveis para um usuário
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a354c71449b5934ae0479eb1833258e394d6987e
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424815"
---
# <a name="tasks-resource-type"></a>tipo de recurso tasks

Namespace: microsoft.graph

Representa os To Do de tarefas disponíveis para um usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List lists](../api/tasks-list-lists.md)|[Coleção baseTaskList](../resources/basetasklist.md)|Obter os recursos baseTaskList da propriedade de navegação listas.|
|[Criar taskList](../api/tasks-post-lists.md)|[taskList](../resources/basetasklist.md)|Crie um novo objeto baseTaskList.|

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|alltasks|[Coleção baseTask](../resources/basetask.md)|Todas as tarefas na caixa de correio dos usuários.|
|listas|[Coleção baseTaskList](../resources/basetasklist.md)|As listas de tarefas na caixa de correio dos usuários.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tasks",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tasks",
  "id": "String (identifier)"
}
```

