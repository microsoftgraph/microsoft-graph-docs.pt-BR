---
title: Tipo de recurso baseTaskList
description: Contém um ou mais recursos de tarefa.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7a0774bf6d51eba2bc55f67c58c2d7de5a0c3312
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424800"
---
# <a name="basetasklist-resource-type"></a>Tipo de recurso baseTaskList

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém um ou mais [recursos de](./basetask.md) tarefa.

Este é o recurso base para os seguintes tipos derivados de listas de tarefas.
* Lista de tarefas in-loco ([recurso wellKnownTaskList)](../resources/wellknowntasklist.md)
* Lista de tarefas criada pelo usuário ([recurso taskList)](../resources/tasklist.md) 

Esse é um tipo abstrato.

## <a name="methods"></a>Métodos
O método a seguir se aplica a qualquer um dos tipos derivados de **baseTaskList** (**wellKnownTaskList**,**taskList**)

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar baseTaskLists](../api/tasks-list-lists.md)|[Coleção baseTaskList](../resources/basetasklist.md)|Obter uma lista dos [objetos baseTaskList](../resources/basetasklist.md) e suas propriedades.|
|[Obter baseTaskList](../api/basetasklist-get.md)|[baseTaskList](../resources/basetasklist.md)|Leia as propriedades e as relações de um [objeto baseTaskList.](../resources/basetasklist.md)|
|[Listar tarefas](../api/basetasklist-list-tasks.md)|[Coleção baseTask](../resources/basetask.md)|Obter os recursos baseTask da propriedade de navegação tarefas.|
|[Criar baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Crie um novo objeto baseTask.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da lista de tarefas.|
|id|String|O identificador da lista de tarefas, exclusivo na caixa de correio do usuário. Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|extensions|Coleção [extension](../resources/extension.md)|A coleção de extensões abertas definidas para a lista de tarefas. Anulável.|
|tarefas|[Coleção baseTask](../resources/basetask.md)|As tarefas nesta lista de tarefas. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.baseTaskList",
  "displayName": "String",
  "id": "String (identifier)"
}
```

