---
title: Componente tarefas no Microsoft Graph Toolkit
description: O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com qualquer tarefa no Microsoft Planner ou no Microsoft to-do.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 80da5522b73051df4d5c264e5289845b9521058f
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639916"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Componente tarefas no Microsoft Graph Toolkit

O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com tarefas no Microsoft Planner ou Microsoft to-do.  

Além disso, um usuário pode atribuir um único ou vários usuários do Microsoft Graph a uma tarefa. Para obter mais detalhes sobre as atribuições do Microsoft Graph, consulte [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).

## <a name="example"></a>Exemplo

O exemplo a seguir exibe as tarefas do Microsoft Planner do usuário conectado usando o `mgt-tasks` componente. Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a>Propriedades

| Atributo | Propriedade | Descrição |
| -- | -- | -- |
| Data-Source = "todo/planejador" | dataSource | Uma enumeração para configurar a fonte de dados para tarefas-Microsoft to-do ou Microsoft Planner. O padrão é `planner`. |
| somente leitura | readOnly | Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas). O padrão é `false`. |
| Ocultar-cabeçalho | hideHeader | Um booliano para mostrar ou ocultar o cabeçalho do componente. O padrão é `false`. |
| Initial-ID = "planner_id/folder_id" | initialid | Uma ID de cadeia de caracteres para definir o planejador ou pasta inicialmente exibido para a ID fornecida. |
| Initial-Bucket-ID = "bucket_id" | initialBucketId | Uma ID de cadeia de caracteres para definir o Bucket exibido inicialmente (somente a fonte de dados do Planner) para a ID fornecida. |
| Target-ID = "planner_id/folder_id"| targetId | Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou ID de pasta fornecido. |
| Target-Bucket-ID = "bucket_id" |targetBucketId  | Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de Bucket fornecida (somente a fonte de dados do Planner). |
| ID de grupo | groupId  | Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de grupo (somente fonte de dados do Planner). |
| Não disponível | isNewTaskVisible  | Determina se a exibição de nova tarefa é visível no processamento. |
| Não disponível | taskFilter  | Uma função opcional para filtrar quais tarefas são exibidas para o usuário. |

O exemplo a seguir mostra apenas as tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

O exemplo a seguir mostra como filtrar tarefas que têm apenas *category3* definido.

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a>Variáveis CSS personalizadas

````css
mgt-tasks {
--tasks-header-padding
--tasks-header-margin 

--tasks-title-padding
--tasks-plan-title-font-size
--tasks-plan-title-padding

--tasks-new-button-width
--tasks-new-button-height
--tasks-new-button-color
--tasks-new-button-background
--tasks-new-button-border
--tasks-new-button-hover-background
--tasks-new-button-active-background

--tasks-new-task-name-margin

--task-margin
--task-box-shadow
--task-background
--task-border

--task-header-color
--task-header-margin

--task-detail-icon-margin

--task-new-margin
--task-new-border
--task-new-line-margin
--tasks-new-line-border
--task-new-input-margin
--task-new-input-padding
--task-new-input-font-size
--task-new-input-active-border
--task-new-select-border

--task-new-add-button-background
--task-new-add-button-disabled-background
--task-new-cancel-button-color

--task-complete-background
--task-complete-border
--task-complete-header-color
--task-complete-detail-color
--task-complete-detail-icon-color
}
````

## <a name="events"></a>Eventos
| Evento | Detalhe | Descrição |
| --- | --- | --- |
| taskClick | O detalhe contém o respectivo `task` objeto | Acionado quando o usuário clica ou toca em uma tarefa. |

## <a name="templates"></a>Modelos

O `tasks` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:

| Tipo de dados     | Contexto de dados              | Descrição                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| tarefa     | tarefa: um planejador ou objeto de tarefa tarefas pendentes | Substitui toda a tarefa padrão. |
| tarefa-detalhes | tarefa: um planejador ou objeto de tarefa tarefas pendentes | o modelo substitui a seção de detalhes da tarefa. |

O exemplo a seguir define um modelo para o componente tarefas.

```html
    <mgt-tasks data-source="todo">
      <template data-type="task-details">
        <div>
          Owner: {{task.owner}}
        </div>
        <div>
          Importance Level: {{task.importance}}
        </div>
      </template>
    </mgt-tasks>
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este controle usa as seguintes APIs e permissões do Microsoft Graph.

| Resource | Permissão |
| - | - |
| /me/planner/plans | Group.Read.All |
| /Planner/Plans/$ {ID} | Group.Read.All, Group.ReadWrite.All |
| /planner/tasks | Group.ReadWrite.All |
| /me/outlook/taskGroups | Tasks.Read |
| /me/outlook/taskFolders | Tarefas. Read, Tasks. ReadWrite |
| /me/outlook/tasks | Tasks.ReadWrite |
| /groups/$ {Group-ID}/Planner/Plans | Group.Read.All, Group.ReadWrite.All |

Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All. Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.

Para a fonte de dados do Microsoft todo, a permissão Tasks. Read é necessária para buscar e ler tarefas. Adicionar, atualizar ou remover tarefas requer a permissão Tasks. ReadWrite.

## <a name="authentication"></a>Autenticação

O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).
