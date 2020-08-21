---
title: tipo de recurso todo
description: Representa os serviços de tarefas pendentes disponíveis para um usuário.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99b2936cf84c5cfdc25a39ff6f0e35518658d0ff
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849828"
---
# <a name="todo-resource-type"></a>tipo de recurso todo

Namespace: microsoft.graph

Representa os serviços de tarefas pendentes disponíveis para um usuário.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar listas](../api/todo-list-lists.md) | coleção [todoTaskList](todotasklist.md) | Obtenha todas as listas de tarefas na caixa de correio do usuário. |
|[Criar todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Criar uma lista de tarefas pendentes na caixa de correio do usuário. |

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|listas|coleção [todoTaskList](../resources/todotasklist.md)| As listas de tarefas na caixa de correio dos usuários. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todo",
  "id": "String"
}
```

