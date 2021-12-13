---
title: Tipo de recurso taskList
description: Representa uma lista criada por um usuário em Microsoft To Do que contém um ou mais recursos task.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 070a427de0531e5ce715e31c91b2ffddd6be4576
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424819"
---
# <a name="tasklist-resource-type"></a>Tipo de recurso taskList

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma lista criada por um usuário em Microsoft To Do que contém um ou mais [recursos task.](./task.md) 

Esse recurso oferece suporte
* Adicionar seus dados a propriedades personalizadas como [extensões abertas](/graph/extensibility-overview)
* Usando [a consulta delta para](/graph/delta-query-overview) rastrear adições incrementais, exclusões e atualizações.

Herda [de baseTaskList](../resources/basetasklist.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar taskLists](../api/tasks-list-lists.md)|[Coleção taskList](../resources/tasklist.md)|Obter uma lista dos objetos [taskList](../resources/tasklist.md) e suas propriedades.|
|[Obter taskList](../api/basetasklist-get.md)|[taskList](../resources/tasklist.md)|Leia as propriedades e as relações de um [objeto taskList.](../resources/tasklist.md)|
|[Atualizar taskList](../api/tasklist-update.md)|[taskList](../resources/tasklist.md)|Atualize as propriedades de um [objeto taskList.](../resources/tasklist.md)|
|[Excluir taskList](../api/tasklist-delete.md)|Nenhum|Exclui um [objeto taskList.](../resources/tasklist.md)|
|[Listar tarefas](../api/basetasklist-list-tasks.md)|[Coleção baseTask](../resources/basetask.md)|Obter os recursos baseTask da propriedade de navegação tarefas.|
|[Criar baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Crie um novo objeto baseTask.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da lista de tarefas. Herdado [de baseTaskList](../resources/basetasklist.md).|
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

