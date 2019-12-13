---
title: Componente tarefas no Microsoft Graph Toolkit
description: O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com qualquer tarefa no Microsoft Planner ou no Microsoft to-do.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 19faf3dec1c61680250cacf3cfaf5837b8bc4cee
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955845"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1b268-104">Componente tarefas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1b268-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1b268-105">O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas.</span><span class="sxs-lookup"><span data-stu-id="1b268-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="1b268-106">Ele funciona com tarefas no Microsoft Planner ou Microsoft to-do.</span><span class="sxs-lookup"><span data-stu-id="1b268-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>  

<span data-ttu-id="1b268-107">Além disso, um usuário pode atribuir um único ou vários usuários do Microsoft Graph a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="1b268-107">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="1b268-108">Para obter mais detalhes sobre as atribuições do Microsoft Graph, consulte [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="1b268-108">For more details about Microsoft Graph assignments, see [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span></span>

## <a name="example"></a><span data-ttu-id="1b268-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b268-109">Example</span></span>

[<span data-ttu-id="1b268-110">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="1b268-110">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="1b268-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b268-111">Properties</span></span>

| <span data-ttu-id="1b268-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="1b268-112">Attribute</span></span> | <span data-ttu-id="1b268-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b268-113">Property</span></span> | <span data-ttu-id="1b268-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b268-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="1b268-115">Data-Source = "todo/planejador"</span><span class="sxs-lookup"><span data-stu-id="1b268-115">data-source="todo/planner"</span></span> | <span data-ttu-id="1b268-116">dataSource</span><span class="sxs-lookup"><span data-stu-id="1b268-116">dataSource</span></span> | <span data-ttu-id="1b268-117">Uma enumeração para configurar a fonte de dados para tarefas-Microsoft to-do ou Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="1b268-117">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="1b268-118">O padrão é `planner`.</span><span class="sxs-lookup"><span data-stu-id="1b268-118">Default is `planner`.</span></span> |
| <span data-ttu-id="1b268-119">somente leitura</span><span class="sxs-lookup"><span data-stu-id="1b268-119">read-only</span></span> | <span data-ttu-id="1b268-120">readOnly</span><span class="sxs-lookup"><span data-stu-id="1b268-120">readOnly</span></span> | <span data-ttu-id="1b268-121">Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="1b268-121">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="1b268-122">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="1b268-122">Default is `false`.</span></span> |
| <span data-ttu-id="1b268-123">Ocultar-cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b268-123">hide-header</span></span> | <span data-ttu-id="1b268-124">hideHeader</span><span class="sxs-lookup"><span data-stu-id="1b268-124">hideHeader</span></span> | <span data-ttu-id="1b268-125">Um booliano para mostrar ou ocultar o cabeçalho do componente.</span><span class="sxs-lookup"><span data-stu-id="1b268-125">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="1b268-126">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="1b268-126">Default is `false`.</span></span> |
| <span data-ttu-id="1b268-127">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="1b268-127">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="1b268-128">initialid</span><span class="sxs-lookup"><span data-stu-id="1b268-128">initialId</span></span> | <span data-ttu-id="1b268-129">Uma ID de cadeia de caracteres para definir o planejador ou pasta inicialmente exibido para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="1b268-129">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="1b268-130">Initial-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="1b268-130">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="1b268-131">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="1b268-131">initialBucketId</span></span> | <span data-ttu-id="1b268-132">Uma ID de cadeia de caracteres para definir o Bucket exibido inicialmente (somente a fonte de dados do Planner) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="1b268-132">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="1b268-133">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="1b268-133">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="1b268-134">targetId</span><span class="sxs-lookup"><span data-stu-id="1b268-134">targetId</span></span> | <span data-ttu-id="1b268-135">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou ID de pasta fornecido.</span><span class="sxs-lookup"><span data-stu-id="1b268-135">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="1b268-136">Target-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="1b268-136">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="1b268-137">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="1b268-137">targetBucketId</span></span>  | <span data-ttu-id="1b268-138">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de Bucket fornecida (somente a fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="1b268-138">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="1b268-139">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="1b268-139">group-id</span></span> | <span data-ttu-id="1b268-140">groupId</span><span class="sxs-lookup"><span data-stu-id="1b268-140">groupId</span></span>  | <span data-ttu-id="1b268-141">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de grupo (somente fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="1b268-141">A string ID to lock the tasks interface to the group ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="1b268-142">Não disponível</span><span class="sxs-lookup"><span data-stu-id="1b268-142">N/A</span></span> | <span data-ttu-id="1b268-143">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="1b268-143">isNewTaskVisible</span></span>  | <span data-ttu-id="1b268-144">Determina se a exibição de nova tarefa é visível no processamento.</span><span class="sxs-lookup"><span data-stu-id="1b268-144">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="1b268-145">Não disponível</span><span class="sxs-lookup"><span data-stu-id="1b268-145">N/A</span></span> | <span data-ttu-id="1b268-146">taskFilter</span><span class="sxs-lookup"><span data-stu-id="1b268-146">taskFilter</span></span>  | <span data-ttu-id="1b268-147">Uma função opcional para filtrar quais tarefas são exibidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1b268-147">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="1b268-148">O exemplo a seguir mostra apenas as tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="1b268-148">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="1b268-149">O exemplo a seguir mostra como filtrar tarefas que têm apenas *category3* definido.</span><span class="sxs-lookup"><span data-stu-id="1b268-149">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="1b268-150">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="1b268-150">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="1b268-151">Eventos</span><span class="sxs-lookup"><span data-stu-id="1b268-151">Events</span></span>
| <span data-ttu-id="1b268-152">Evento</span><span class="sxs-lookup"><span data-stu-id="1b268-152">Event</span></span> | <span data-ttu-id="1b268-153">Detalhe</span><span class="sxs-lookup"><span data-stu-id="1b268-153">Detail</span></span> | <span data-ttu-id="1b268-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b268-154">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1b268-155">taskClick</span><span class="sxs-lookup"><span data-stu-id="1b268-155">taskClick</span></span> | <span data-ttu-id="1b268-156">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="1b268-156">The detail contains the respective `task` object</span></span> | <span data-ttu-id="1b268-157">Acionado quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="1b268-157">Fired when the user clicks or taps on a task.</span></span> |

## <a name="templates"></a><span data-ttu-id="1b268-158">Modelos</span><span class="sxs-lookup"><span data-stu-id="1b268-158">Templates</span></span>

<span data-ttu-id="1b268-159">O `tasks` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="1b268-159">The `tasks` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="1b268-160">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="1b268-160">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="1b268-161">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="1b268-161">Data type</span></span>     | <span data-ttu-id="1b268-162">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="1b268-162">Data context</span></span>              | <span data-ttu-id="1b268-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b268-163">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="1b268-164">tarefa</span><span class="sxs-lookup"><span data-stu-id="1b268-164">task</span></span>     | <span data-ttu-id="1b268-165">tarefa: um planejador ou objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="1b268-165">task: a planner or to-do task object</span></span> | <span data-ttu-id="1b268-166">Substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="1b268-166">replaces the whole default task.</span></span> |
| <span data-ttu-id="1b268-167">tarefa-detalhes</span><span class="sxs-lookup"><span data-stu-id="1b268-167">task-details</span></span> | <span data-ttu-id="1b268-168">tarefa: um planejador ou objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="1b268-168">task: a planner or to-do task object</span></span> | <span data-ttu-id="1b268-169">o modelo substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="1b268-169">template replaces the details section of the task.</span></span> |

<span data-ttu-id="1b268-170">O exemplo a seguir define um modelo para o componente tarefas.</span><span class="sxs-lookup"><span data-stu-id="1b268-170">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="1b268-171">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1b268-171">Microsoft Graph permissions</span></span>

<span data-ttu-id="1b268-172">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1b268-172">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="1b268-173">Resource</span><span class="sxs-lookup"><span data-stu-id="1b268-173">Resource</span></span> | <span data-ttu-id="1b268-174">Permissão</span><span class="sxs-lookup"><span data-stu-id="1b268-174">Permission</span></span> |
| - | - |
| <span data-ttu-id="1b268-175">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="1b268-175">/me/planner/plans</span></span> | <span data-ttu-id="1b268-176">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b268-176">Group.Read.All</span></span> |
| <span data-ttu-id="1b268-177">/Planner/Plans/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="1b268-177">/planner/plans/${id}</span></span> | <span data-ttu-id="1b268-178">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b268-178">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1b268-179">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="1b268-179">/planner/tasks</span></span> | <span data-ttu-id="1b268-180">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b268-180">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1b268-181">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="1b268-181">/me/outlook/taskGroups</span></span> | <span data-ttu-id="1b268-182">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1b268-182">Tasks.Read</span></span> |
| <span data-ttu-id="1b268-183">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="1b268-183">/me/outlook/taskFolders</span></span> | <span data-ttu-id="1b268-184">Tarefas. Read, Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b268-184">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="1b268-185">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="1b268-185">/me/outlook/tasks</span></span> | <span data-ttu-id="1b268-186">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b268-186">Tasks.ReadWrite</span></span> |
| <span data-ttu-id="1b268-187">/groups/$ {Group-ID}/Planner/Plans</span><span class="sxs-lookup"><span data-stu-id="1b268-187">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="1b268-188">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b268-188">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="1b268-189">Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All.</span><span class="sxs-lookup"><span data-stu-id="1b268-189">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="1b268-190">Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="1b268-190">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="1b268-191">Para a fonte de dados do Microsoft todo, a permissão Tasks. Read é necessária para buscar e ler tarefas.</span><span class="sxs-lookup"><span data-stu-id="1b268-191">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="1b268-192">Adicionar, atualizar ou remover tarefas requer a permissão Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="1b268-192">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="1b268-193">Autenticação</span><span class="sxs-lookup"><span data-stu-id="1b268-193">Authentication</span></span>

<span data-ttu-id="1b268-194">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="1b268-194">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
