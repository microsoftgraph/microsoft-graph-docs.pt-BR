---
title: Tipo de recurso wellKnownTaskList
description: Uma lista de tarefas embutida que não pode ser renomeada ou excluída.
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0594ac7082680096ce17b3780780cc105e30606c
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424809"
---
# <a name="wellknowntasklist-resource-type"></a>Tipo de recurso wellKnownTaskList

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma lista de tarefas embutida que não pode ser renomeada ou excluída. To Do tem duas listas de tarefas e **emails** **sinalizados.**

Esse recurso dá suporte à adição de dados a propriedades personalizadas como [extensões abertas](/graph/extensibility-overview)

Herda [de baseTaskList](../resources/basetasklist.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar wellKnownTaskLists](../api/tasks-list-lists.md)|[Coleção wellKnownTaskList](../resources/wellknowntasklist.md)|Obter uma lista dos [objetos wellKnownTaskList](../resources/wellknowntasklist.md) e suas propriedades.|
|[Obter wellKnownTaskList](../api/basetasklist-get.md)|[wellKnownTaskList](../resources/wellknowntasklist.md)|Leia as propriedades e as relações de um [objeto wellKnownTaskList.](../resources/wellknowntasklist.md)|
|[Listar tarefas](../api/basetasklist-list-tasks.md)|[Coleção baseTask](../resources/basetask.md)|Obter os recursos baseTask da propriedade de navegação tarefas.|
|[Criar baseTask](../api/basetasklist-post-tasks.md)|[baseTask](../resources/basetask.md)|Crie um novo objeto baseTask.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome da lista de tarefas. Herdado [de baseTaskList](../resources/basetasklist.md).|
|id|String|O identificador da lista de tarefas, exclusivo na caixa de correio do usuário. Somente leitura. Herdado [de baseTaskList](../resources/basetasklist.md).|
|wellKnownListName|wellKnownListName_v2|Propriedade indicando o nome da lista se a lista determinada for uma lista conhecida.. Os valores possíveis são: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

### <a name="wellknownlistname-values"></a>valores wellknownListName
|Member|Descrição|
|:---|:---|
|none| Lista criada pelo usuário.|
|defaultList| Lista de tarefas **integrados.**|
|flaggedEmails| Lista de **email sinalizada** embutida. Tarefas de emails sinalizados estão presentes nesta lista.|
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar.|

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

