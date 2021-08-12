---
title: tipo de recurso todo
description: Representa os serviços To Do disponíveis para um usuário.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 89bbdd1bd3d91c5114850ffad8afc3aeec90e8bf3bbfb0b65e540444c2022b7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235258"
---
# <a name="todo-resource-type"></a>tipo de recurso todo

Namespace: microsoft.graph

Representa os serviços To Do disponíveis para um usuário.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[List lists](../api/todo-list-lists.md) | Coleção [todoTaskList](todotasklist.md) | Obtenha todas as listas de tarefas na caixa de correio do usuário. |
|[Criar todoTaskList](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Criar uma lista de tarefas To Dona caixa de correio do usuário. |

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|listas|Coleção [todoTaskList](../resources/todotasklist.md)| As listas de tarefas na caixa de correio dos usuários. |

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



