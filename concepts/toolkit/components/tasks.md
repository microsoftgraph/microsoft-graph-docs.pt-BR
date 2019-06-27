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
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ca252-104">Componente tarefas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="ca252-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ca252-105">O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas.</span><span class="sxs-lookup"><span data-stu-id="ca252-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="ca252-106">Ele funciona com tarefas no Microsoft Planner ou Microsoft to-do.</span><span class="sxs-lookup"><span data-stu-id="ca252-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>

## <a name="example"></a><span data-ttu-id="ca252-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca252-107">Example</span></span>

[<span data-ttu-id="ca252-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="ca252-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="ca252-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca252-109">Properties</span></span>

| <span data-ttu-id="ca252-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca252-110">Property</span></span> | <span data-ttu-id="ca252-111">Atributo</span><span class="sxs-lookup"><span data-stu-id="ca252-111">Attribute</span></span> | <span data-ttu-id="ca252-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca252-112">Description</span></span> |
| -- | -- | -- |
| `dataSource` | `data-source="todo/planner"` | <span data-ttu-id="ca252-113">Define a fonte de dados para tarefas-Microsoft a-do ou Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="ca252-113">Sets the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="ca252-114">O padrão é `planner`.</span><span class="sxs-lookup"><span data-stu-id="ca252-114">Default is `planner`.</span></span> |
| `readOnly` | `read-only` | <span data-ttu-id="ca252-115">Define a interface de tarefa como somente leitura (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="ca252-115">Sets the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="ca252-116">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="ca252-116">Default is `false`.</span></span> |
| `initialId` | `initial-id="planner_id/folder_id"` | <span data-ttu-id="ca252-117">Define o planejador ou pasta inicialmente exibido para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="ca252-117">Sets the initially displayed planner or folder to the provided ID.</span></span> |
| `initialBucketId` | `initial-bucket-id="bucket_id"` | <span data-ttu-id="ca252-118">Define o Bucket exibido inicialmente (somente a fonte de dados do Planner) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="ca252-118">Sets the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| `targetId` | `target-id="planner_id/folder_id"` | <span data-ttu-id="ca252-119">Bloqueia a interface de tarefas para o planejador ou ID de pasta fornecido.</span><span class="sxs-lookup"><span data-stu-id="ca252-119">Locks the tasks interface to the provided planner or folder ID.</span></span> |
| `targetBucketId` | `target-bucket-id="bucket_id"` | <span data-ttu-id="ca252-120">Bloqueia a interface de tarefas para a ID de Bucket fornecida (somente a fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="ca252-120">Locks the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |

<span data-ttu-id="ca252-121">Apresentamos um exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="ca252-121">The following is an example.</span></span>

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a><span data-ttu-id="ca252-122">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="ca252-122">Custom CSS variables</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ca252-123">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ca252-123">Microsoft Graph permissions</span></span>

<span data-ttu-id="ca252-124">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ca252-124">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="ca252-125">Resource</span><span class="sxs-lookup"><span data-stu-id="ca252-125">Resource</span></span> | <span data-ttu-id="ca252-126">Permissão/escopo</span><span class="sxs-lookup"><span data-stu-id="ca252-126">Permission/scope</span></span> |
| - | - |
| <span data-ttu-id="ca252-127">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="ca252-127">/me/planner/plans</span></span> | `Group.Read.All` |
| <span data-ttu-id="ca252-128">/Planner/Plans/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="ca252-128">/planner/plans/${id}</span></span> | <span data-ttu-id="ca252-129">`Group.Read.All`, `Group.ReadWrite.All`</span><span class="sxs-lookup"><span data-stu-id="ca252-129"></span></span> |
| <span data-ttu-id="ca252-130">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="ca252-130">/planner/tasks</span></span> | `Group.ReadWrite.All` |
| <span data-ttu-id="ca252-131">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="ca252-131">/me/outlook/taskGroups</span></span> | `Tasks.Read` |
| <span data-ttu-id="ca252-132">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="ca252-132">/me/outlook/taskFolders</span></span> | <span data-ttu-id="ca252-133">`Tasks.Read`, `Tasks.ReadWrite`</span><span class="sxs-lookup"><span data-stu-id="ca252-133"></span></span> |
| <span data-ttu-id="ca252-134">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="ca252-134">/me/outlook/tasks</span></span> | `Tasks.ReadWrite` |

<span data-ttu-id="ca252-135">Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All.</span><span class="sxs-lookup"><span data-stu-id="ca252-135">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="ca252-136">Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="ca252-136">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="ca252-137">Para a fonte de dados do Microsoft todo, a permissão Tasks. Read é necessária para buscar e ler tarefas.</span><span class="sxs-lookup"><span data-stu-id="ca252-137">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="ca252-138">Adicionar, atualizar ou remover tarefas requer a permissão Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="ca252-138">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="ca252-139">Autenticação</span><span class="sxs-lookup"><span data-stu-id="ca252-139">Authentication</span></span>

<span data-ttu-id="ca252-140">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="ca252-140">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
