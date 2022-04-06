---
title: Componente Tarefas no microsoft Graph Toolkit
description: O componente Tarefas permite ao usuário exibir, adicionar, remover, concluir ou editar tarefas. Ele funciona com qualquer tarefa Microsoft Planner.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 92d38afc5d0385cde96f0b36b47c5a92de559e78
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64586808"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Componente Tarefas no microsoft Graph Toolkit

O componente Tarefas permite que o usuário exibir, adicionar, remover, concluir ou editar tarefas de Microsoft Planner.  

Além disso, um usuário pode atribuir um único ou vários usuários Graph Microsoft a uma tarefa. Para obter mais detalhes sobre Graph microsoft, consulte [plannerAssignments](/graph/api/resources/plannerassignments).

## <a name="example"></a>Exemplo

O exemplo a seguir exibe as tarefas de Microsoft Planner do usuário Microsoft Planner usando o `mgt-tasks` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a>Propriedades

| Atributo | Propriedade | Descrição |
| -- | -- | -- |
| somente leitura | readOnly | Um Boolean para definir a interface da tarefa a ser lida somente (sem adicionar ou remover tarefas). O padrão é `false`. |
| hide-header | hideHeader | Um Boolean para mostrar ou ocultar o header do componente. O padrão é `false`. |
| hide-options | hideOptions | Um Boolean para mostrar ou ocultar as opções em tarefas. O padrão é `false`.
| initial-id="planner_id/folder_id" | initialId | Uma ID de cadeia de caracteres para definir o planejador ou pasta exibido inicialmente como a ID fornecida. |
| initial-bucket-id="bucket_id" | initialBucketId | Uma ID de cadeia de caracteres para definir o bucket exibido inicialmente (Planner Data-Source Somente) para a ID fornecida. |
| target-id="planner_id/folder_id"| targetId | Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou a ID de pasta fornecida. |
| target-bucket-id="bucket_id" |targetBucketId  | Uma ID de cadeia de caracteres para bloquear a interface de tarefas na ID de bucket fornecida (Planner Data-Source Only). |
| group-id | groupId  | Uma ID de cadeia de caracteres para bloquear a interface de tarefas na ID do grupo. |
| N/D | isNewTaskVisible  | Determina se o novo exibição de tarefa está visível na renderização. |
| N/D | taskFilter  | Uma função opcional para filtrar quais tarefas são mostradas ao usuário. |

O exemplo a seguir mostra apenas tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

O exemplo a seguir mostra como filtrar tarefas que só têm *conjunto de categoria3* .

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

--task-icon-background-completed
--task-icon-background

--task-icon-border-completed
--task-icon-border

--task-icon-color
--task-icon-color-completed

--task-icon-border-radius

--task-icon-alignment: flex-start (default) | center | flex-end
}
````

## <a name="events"></a>Eventos

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`taskAdded` | Dispara quando uma nova tarefa é criada | Tarefa recém-criada que pode ser um [plannerTask](/graph/api/resources/plannertask) nosso [outlookTask](/graph/api/resources/outlooktask) | Não | Não | Sim
`taskChanged` | Dispara quando os metadados da tarefa foram alterados, como a marcação concluída | Tarefa atualizada que pode ser um [plannerTask](/graph/api/resources/plannertask) nosso [outlookTask](/graph/api/resources/outlooktask) | Não | Não | Não
`taskClick` | Dispara quando o usuário clica ou toca em uma tarefa | `task` com o [plannerTask selecionado](/graph/api/resources/plannertask) nosso [outlookTask](/graph/api/resources/outlooktask) | Não | Não | Não
`taskRemoved` | Dispara quando uma tarefa existente foi excluída | `task` com o [plannerTask selecionado](/graph/api/resources/plannertask) nosso [outlookTask](/graph/api/resources/outlooktask) | Não | Não | Não

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

## <a name="templates"></a>Modelos

O `tasks` componente dá suporte a [vários modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e de `data-type` definir o valor como um dos seguintes:

| Tipo de dados     | Contexto de dados              | Descrição                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| tarefa     | tarefa: um objeto de tarefa do planner | substitui toda a tarefa padrão. |
| detalhes da tarefa | tarefa: um objeto de tarefa do planner | template substitui a seção de detalhes da tarefa. |

O exemplo a seguir define um modelo para o componente de tarefas.

```html
    <mgt-tasks>
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

Esse controle usa as seguintes APIs Graph Microsoft e permissões.

| Configuração | Permissão | API |
| ------------- | ---------- | --- |
| `groupId` definir e `dataSource` definir como `TasksSource.planner` | Group.Read.All | [/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?tabs=http) |
| `targetId` definir e `dataSource` definir como `TasksSource.todo` | Tasks.Read | [/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&preserve-view=true&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&preserve-view=true&tabs=http) |
| `targetId` set and `dataSource` set to something else than `TasksSource.todo` | Group.Read.All | [/planner/plans/${planId}](/graph/api/plannerplan-get?tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?tabs=http) |
| `dataSource` set to `TasksSource.planner` | Group.Read.All | [/me/planner/plans](/graph/api/planneruser-list-plans?tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?tabs=http) |
| `dataSource` set to `TasksSource.todo` | Tasks.Read | [/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&preserve-view=true&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&preserve-view=true&tabs=http) |
| `addTask` definir como `true` e `dataSource` definir como `TasksSource.planner` | Group.ReadWrite.All | [/planner/tasks](/graph/api/planner-post-tasks?tabs=http) |
| `addTask` definir como `true` e `dataSource` definir como `TasksSource.todo` | Tasks.ReadWrite | [/me/outlook/taskFolders/${parentFolderId}/tasks](/graph/api/outlookuser-post-tasks?view=graph-rest-beta&preserve-view=true&tabs=csharp) |

Para a Microsoft Planner de dados, buscar e ler tarefas requer a permissão Groups.Read.All. Adicionar, atualizar ou remover tarefas requer a permissão Groups.ReadWrite.All.

## <a name="authentication"></a>Autenticação

O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="cache"></a>Cache

O `mgt-tasks` componente não armazena dados em cache.
