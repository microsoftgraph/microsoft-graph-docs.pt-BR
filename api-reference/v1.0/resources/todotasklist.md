---
title: Tipo de recurso todoTaskList
description: Uma lista em Microsoft To Do que contém um ou mais recursos todoTask.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 24d98f5fa351db7aed56a637eee2d606d42fb504
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134287"
---
# <a name="todotasklist-resource-type"></a>Tipo de recurso todoTaskList

Namespace: microsoft.graph

Uma lista em Microsoft To Do que contém um ou mais [recursos todoTask.](./todotask.md) 

No To Do, há listas de tarefas internos,  como emails sinalizados e **Tarefas** que não podem ser renomeadas ou excluídas.  No entanto, você pode criar listas de tarefas adicionais.

Esse recurso oferece suporte
* Adicionar seus dados a propriedades personalizadas como [extensões abertas](/graph/extensibility-overview)
* Usando [a consulta delta para](/graph/delta-query-overview) rastrear adições incrementais, exclusões e atualizações.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List lists](../api/todo-list-lists.md) | Coleção [todoTaskList](todotasklist.md) | Obter todas as [todoTaskList](todotasklist.md) na caixa de correio do usuário. |
|[Criar todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Crie um [todoTaskList](todotasklist.md) na caixa de correio do usuário. |
|[Obter lista de tarefas](../api/todotasklist-get.md)|[todoTaskList](todotasklist.md)|Leia as propriedades e as relações do [todoTaskList especificado.](todotasklist.md)|
|[Atualizar lista de tarefas](../api/todotasklist-update.md)|[todoTaskList](todotasklist.md)| Atualize as propriedades writable do [todoTaskList especificado.](todotasklist.md)|
|[Excluir lista de tarefas](../api/todotasklist-delete.md)|Nenhum(a)| Exclua [todoTaskList especificado.](todotasklist.md)|
|[Listar tarefas](../api/todotasklist-list-tasks.md)|Coleção [todoTask](todotask.md)|Obtenha todos os recursos [todoTask](todotask.md) na lista especificada.|
|[Criar tarefa](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Crie um [todoTask](todotask.md) na lista de tarefas especificada.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da lista de tarefas.|
|id|String| O identificador da lista de tarefas, exclusivo na caixa de correio do usuário. Somente leitura. Herdado da [entidade](entity.md)|
|isOwner|Boolean| True se o usuário for proprietário da lista de tarefas determinada.|
|isShared|Booliano| True se a lista de tarefas for compartilhada com outros usuários|
|wellknownListName|wellknownListName| Propriedade indicando o nome da lista se a lista determinada for uma lista conhecida. Os valores possíveis são: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

### <a name="wellknownlistname-values"></a>valores wellknownListName
|Member|Descrição|
|:---|:---|
|Nenhuma| Lista criada pelo usuário.|
|defaultList| Lista de **tarefas** integrados.|
|flaggedEmails| Lista de **email sinalizada** embutida. Tarefas de emails sinalizados estão presentes nesta lista.|
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|extensions|[extension](extension.md) collection| A coleção de extensões abertas definidas para a lista de tarefas. Anulável.|
|tarefas|Coleção [todoTask](todotask.md)|As tarefas nesta lista de tarefas. Somente leitura. Anulável.|

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



