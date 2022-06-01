---
title: Tipo de recurso taskList
description: Representa uma lista criada por um usuário no Microsoft To Do que contém um ou mais recursos de tarefa.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bee831640d6ba392f359a1ad1dbd70b088733141
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819353"
---
# <a name="tasklist-resource-type-deprecated"></a>Tipo de recurso taskList (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Representa uma lista criada por um usuário no Microsoft To Do que contém um ou mais recursos [de](./task.md) tarefa. 

Esse recurso dá suporte ao seguinte:
* Adicionando seus dados a propriedades [personalizadas como extensões abertas](/graph/extensibility-overview)
* Usando [a consulta delta para](/graph/delta-query-overview) acompanhar adições incrementais, exclusões e atualizações.

O **recurso taskList** herda de [baseTaskList](../resources/basetasklist.md).
Seu conteúdo, do tipo **de recurso** de tarefa, herda de [baseTask](../resources/basetask.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar taskLists](../api/tasks-list-lists.md)|[coleção taskList](../resources/tasklist.md)|Obtenha uma lista dos objetos [taskList](../resources/tasklist.md) e suas propriedades.|
|[Obter taskList](../api/basetasklist-get.md)|[Tasklist](../resources/tasklist.md)|Leia as propriedades e as relações de um [objeto taskList](../resources/tasklist.md) .|
|[Atualizar taskList](../api/tasklist-update.md)|[Tasklist](../resources/tasklist.md)|Atualize as propriedades de um [objeto taskList](../resources/tasklist.md) .|
|[Excluir taskList](../api/tasklist-delete.md)|Nenhum|Exclui um objeto [taskList](../resources/tasklist.md) .|
|[Listar tarefas](../api/basetasklist-list-tasks.md)|[Coleção baseTask](../resources/basetask.md)|Obtenha os recursos baseTask da propriedade de navegação de tarefas.|
|[Criar baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Crie um novo objeto baseTask.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome da lista de tarefas. Herdado [de baseTaskList](../resources/basetasklist.md).|
|id|String|O identificador da lista de tarefas, exclusivo na caixa de correio do usuário. Somente leitura. Herdado [de baseTaskList](../resources/basetasklist.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|extensions|Coleção [extension](../resources/extension.md)|A coleção de extensões abertas definidas para a lista de tarefas. Anulável. Herdado [de baseTaskList](../resources/basetasklist.md)|
|tarefas|[Coleção baseTask](../resources/basetask.md)|As tarefas nesta lista de tarefas. Somente leitura. Anulável. Herdado [de baseTaskList](../resources/basetasklist.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taskList",
  "baseType": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taskList",
  "displayName": "String",
  "id": "String (identifier)"
}
```

