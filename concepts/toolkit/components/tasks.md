---
title: Componente tarefas no Microsoft Graph Toolkit
description: O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com qualquer tarefa no Microsoft Planner ou no Microsoft to-do.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 3c2017acd7fe054c71a609c8d908e119e12a590b
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242940"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Componente tarefas no Microsoft Graph Toolkit

O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com tarefas no Microsoft Planner ou Microsoft to-do.

## <a name="example"></a>Exemplo

[exemplo de jsfiddle](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a>Propriedades

| Propriedade | Atributo | Descrição |
| -- | -- | -- |
| `dataSource` | `data-source="todo/planner"` | Define a fonte de dados para tarefas-Microsoft a-do ou Microsoft Planner. O padrão é `planner`. |
| `readOnly` | `read-only` | Define a interface de tarefa como somente leitura (sem adicionar ou remover tarefas). O padrão é `false`. |
| `initialId` | `initial-id="planner_id/folder_id"` | Define o planejador ou pasta inicialmente exibido para a ID fornecida. |
| `initialBucketId` | `initial-bucket-id="bucket_id"` | Define o Bucket exibido inicialmente (somente a fonte de dados do Planner) para a ID fornecida. |
| `targetId` | `target-id="planner_id/folder_id"` | Bloqueia a interface de tarefas para o planejador ou ID de pasta fornecido. |
| `targetBucketId` | `target-bucket-id="bucket_id"` | Bloqueia a interface de tarefas para a ID de Bucket fornecida (somente a fonte de dados do Planner). |

Apresentamos um exemplo a seguir.

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

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

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Este controle usa as seguintes APIs e permissões do Microsoft Graph.

| Resource | Permissão/escopo |
| - | - |
| /me/planner/plans | `Group.Read.All` |
| /Planner/Plans/$ {ID} | `Group.Read.All`, `Group.ReadWrite.All` |
| /planner/tasks | `Group.ReadWrite.All` |
| /me/outlook/taskGroups | `Tasks.Read` |
| /me/outlook/taskFolders | `Tasks.Read`, `Tasks.ReadWrite` |
| /me/outlook/tasks | `Tasks.ReadWrite` |

Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All. Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.

Para a fonte de dados do Microsoft todo, a permissão Tasks. Read é necessária para buscar e ler tarefas. Adicionar, atualizar ou remover tarefas requer a permissão Tasks. ReadWrite.

## <a name="authentication"></a>Autenticação

O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).
