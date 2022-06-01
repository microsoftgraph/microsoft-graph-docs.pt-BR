---
title: Tipo de recurso wellKnownTaskList
description: Uma lista de tarefas interna que não pode ser renomeada ou excluída.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0391983a88f91255779b994221fed195ad890c7e
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821194"
---
# <a name="wellknowntasklist-resource-type-deprecated"></a>Tipo de recurso wellKnownTaskList (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

Uma lista de tarefas interna que não pode ser renomeada ou excluída. To Do tem duas listas internas, email **sinalizado e** **lista de** tarefas.

Esse recurso dá suporte à adição de dados a propriedades [personalizadas como extensões abertas](/graph/extensibility-overview)

Herda de [baseTaskList](../resources/basetasklist.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar wellKnownTaskLists](../api/tasks-list-lists.md)|[coleção wellKnownTaskList](../resources/wellknowntasklist.md)|Obtenha uma lista dos [objetos wellKnownTaskList](../resources/wellknowntasklist.md) e suas propriedades.|
|[Obter wellKnownTaskList](../api/basetasklist-get.md)|[wellKnownTaskList](../resources/wellknowntasklist.md)|Leia as propriedades e as relações de um [objeto wellKnownTaskList](../resources/wellknowntasklist.md) .|
|[Listar tarefas](../api/basetasklist-list-tasks.md)|[Coleção baseTask](../resources/basetask.md)|Obtenha os recursos baseTask da propriedade de navegação de tarefas.|
|[Criar baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Crie um novo objeto baseTask.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome da lista de tarefas. Herdado [de baseTaskList](../resources/basetasklist.md).|
|id|Cadeia de caracteres|O identificador da lista de tarefas, exclusivo na caixa de correio do usuário. Somente leitura. Herdado [de baseTaskList](../resources/basetasklist.md).|
|wellKnownListName|wellKnownListName_v2|Propriedade que indica o nome da lista se a lista fornecida for uma lista conhecida.. Os valores possíveis são: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

### <a name="wellknownlistname-values"></a>Valores wellknownListName
|Member|Descrição|
|:---|:---|
|none| Lista criada pelo usuário.|
|defaultList| Lista de tarefas **internas** .|
|flaggedEmails| Lista de **email sinalizada interna** . As tarefas de emails sinalizados estão presentes nesta lista.|
|unknownFutureValue| Valor de sentinel de enumeração evolvável. Não usar.|

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
  "@odata.type": "microsoft.graph.wellKnownTaskList",
  "baseType": "microsoft.graph.baseTaskList",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.wellKnownTaskList",
  "displayName": "String",
  "id": "String (identifier)",
  "wellKnownListName": "String"
}
```

