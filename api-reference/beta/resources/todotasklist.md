---
title: tipo de recurso todoTaskList
description: Uma lista na Microsoft que contém um ou mais recursos do todoTask.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34f90329fc6ca4d5e12ff2f2b191819b88f895b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849825"
---
# <a name="todotasklist-resource-type"></a>tipo de recurso todoTaskList

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma lista na Microsoft que contém um ou mais recursos do [todoTask](./todotask.md) . 

Em tarefas pendentes, há listas de tarefas internas, como **emails sinalizados** e **tarefas** que não podem ser renomeadas ou excluídas.  No entanto, você pode criar listas de tarefas adicionais.

Este recurso suporta
* Adicionando seus dados às propriedades personalizadas como [extensões abertas](/graph/extensibility-overview)
* Usando a [consulta Delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar listas](../api/todo-list-lists.md) | coleção [todoTaskList](todotasklist.md) | Obtenha todos os [todoTaskList](todotasklist.md) na caixa de correio do usuário. |
|[Criar todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Criar um [todoTaskList](todotasklist.md) na caixa de correio do usuário. |
|[Obter lista de tarefas](../api/todotasklist-get.md)|[todoTaskList](todotasklist.md)|Leia as propriedades e as relações do [todoTaskList](todotasklist.md)especificado.|
|[Atualizar lista de tarefas](../api/todotasklist-update.md)|[todoTaskList](todotasklist.md)| Atualize as propriedades graváveis do [todoTaskList](todotasklist.md)especificado.|
|[Excluir lista de tarefas](../api/todotasklist-delete.md)|Nenhuma| Exclua o [todoTaskList](todotasklist.md) especificado.|
|[Listar tarefas](../api/todotasklist-list-tasks.md)|coleção [todoTask](todotask.md)|Obtenha todos os recursos do [todoTask](todotask.md) na lista especificada.|
|[Criar tarefa](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Criar um [todoTask](todotask.md) na lista de tarefas especificada.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da lista de tarefas.|
|id|String| O identificador da lista de tarefas, exclusivo na caixa de correio do usuário. Somente leitura. Herdado da [entidade](entity.md)|
|IsOwner|Booliano| True se o usuário é proprietário da lista de tarefas determinada.|
|isShared|Booliano| True se a lista de tarefas é compartilhada com outros usuários|
|wellknownListName|wellknownListName| Propriedade que indica o nome da lista conhecido se a lista fornecida é uma lista conhecida. Os valores possíveis são: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|extensions|Coleção [extension](extension.md)| A coleção de extensões abertas definida para a lista de tarefas. Anulável.|
|tarefas|coleção [todoTask](todotask.md)|As tarefas desta lista de tarefas. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTaskList",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "String (identifier)",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
}
```

