---
title: Componente Tarefas no microsoft Graph Toolkit
description: O componente Tarefas permite ao usuário exibir, adicionar, remover, concluir ou editar tarefas. Ele funciona com qualquer tarefa no Microsoft Planner.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 3b3476751798dd5569218ec6acc6d09a91112fe6
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082031"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="aca0e-104">Componente Tarefas no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="aca0e-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="aca0e-105">O componente Tarefas permite ao usuário exibir, adicionar, remover, concluir ou editar tarefas do Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="aca0e-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks from Microsoft Planner.</span></span>  

<span data-ttu-id="aca0e-106">Além disso, um usuário pode atribuir um único ou vários usuários Graph Microsoft a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="aca0e-106">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="aca0e-107">Para obter mais detalhes sobre Graph microsoft, consulte [plannerAssignments](/graph/api/resources/plannerassignments).</span><span class="sxs-lookup"><span data-stu-id="aca0e-107">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments).</span></span>

## <a name="example"></a><span data-ttu-id="aca0e-108">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aca0e-108">Example</span></span>

<span data-ttu-id="aca0e-109">O exemplo a seguir exibe as tarefas do Microsoft Planner do usuário de logo-in usando o `mgt-tasks` componente.</span><span class="sxs-lookup"><span data-stu-id="aca0e-109">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="aca0e-110">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="aca0e-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="aca0e-111">Abrir este exemplo no mgt.dev</span><span class="sxs-lookup"><span data-stu-id="aca0e-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="aca0e-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aca0e-112">Properties</span></span>

| <span data-ttu-id="aca0e-113">Atributo</span><span class="sxs-lookup"><span data-stu-id="aca0e-113">Attribute</span></span> | <span data-ttu-id="aca0e-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aca0e-114">Property</span></span> | <span data-ttu-id="aca0e-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca0e-115">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="aca0e-116">somente leitura</span><span class="sxs-lookup"><span data-stu-id="aca0e-116">read-only</span></span> | <span data-ttu-id="aca0e-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="aca0e-117">readOnly</span></span> | <span data-ttu-id="aca0e-118">Um Boolean para definir a interface da tarefa a ser lida somente (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="aca0e-118">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="aca0e-119">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="aca0e-119">Default is `false`.</span></span> |
| <span data-ttu-id="aca0e-120">hide-header</span><span class="sxs-lookup"><span data-stu-id="aca0e-120">hide-header</span></span> | <span data-ttu-id="aca0e-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="aca0e-121">hideHeader</span></span> | <span data-ttu-id="aca0e-122">Um Boolean para mostrar ou ocultar o header do componente.</span><span class="sxs-lookup"><span data-stu-id="aca0e-122">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="aca0e-123">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="aca0e-123">Default is `false`.</span></span> |
| <span data-ttu-id="aca0e-124">hide-options</span><span class="sxs-lookup"><span data-stu-id="aca0e-124">hide-options</span></span> | <span data-ttu-id="aca0e-125">hideOptions</span><span class="sxs-lookup"><span data-stu-id="aca0e-125">hideOptions</span></span> | <span data-ttu-id="aca0e-126">Um Boolean para mostrar ou ocultar as opções em tarefas.</span><span class="sxs-lookup"><span data-stu-id="aca0e-126">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="aca0e-127">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="aca0e-127">Default is `false`.</span></span>
| <span data-ttu-id="aca0e-128">initial-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="aca0e-128">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="aca0e-129">initialId</span><span class="sxs-lookup"><span data-stu-id="aca0e-129">initialId</span></span> | <span data-ttu-id="aca0e-130">Uma ID de cadeia de caracteres para definir o planejador ou pasta exibido inicialmente como a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="aca0e-130">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="aca0e-131">initial-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="aca0e-131">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="aca0e-132">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="aca0e-132">initialBucketId</span></span> | <span data-ttu-id="aca0e-133">Uma ID de cadeia de caracteres para definir o bucket exibido inicialmente (Planner Data-Source Somente) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="aca0e-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="aca0e-134">target-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="aca0e-134">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="aca0e-135">targetId</span><span class="sxs-lookup"><span data-stu-id="aca0e-135">targetId</span></span> | <span data-ttu-id="aca0e-136">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou a ID de pasta fornecida.</span><span class="sxs-lookup"><span data-stu-id="aca0e-136">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="aca0e-137">target-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="aca0e-137">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="aca0e-138">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="aca0e-138">targetBucketId</span></span>  | <span data-ttu-id="aca0e-139">Uma ID de cadeia de caracteres para bloquear a interface de tarefas na ID de bucket fornecida (Planner Data-Source Only).</span><span class="sxs-lookup"><span data-stu-id="aca0e-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="aca0e-140">group-id</span><span class="sxs-lookup"><span data-stu-id="aca0e-140">group-id</span></span> | <span data-ttu-id="aca0e-141">groupId</span><span class="sxs-lookup"><span data-stu-id="aca0e-141">groupId</span></span>  | <span data-ttu-id="aca0e-142">Uma ID de cadeia de caracteres para bloquear a interface de tarefas na ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="aca0e-142">A string ID to lock the tasks interface to the group ID.</span></span> |
| <span data-ttu-id="aca0e-143">N/A</span><span class="sxs-lookup"><span data-stu-id="aca0e-143">N/A</span></span> | <span data-ttu-id="aca0e-144">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="aca0e-144">isNewTaskVisible</span></span>  | <span data-ttu-id="aca0e-145">Determina se o novo exibição de tarefa está visível na renderização.</span><span class="sxs-lookup"><span data-stu-id="aca0e-145">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="aca0e-146">N/A</span><span class="sxs-lookup"><span data-stu-id="aca0e-146">N/A</span></span> | <span data-ttu-id="aca0e-147">taskFilter</span><span class="sxs-lookup"><span data-stu-id="aca0e-147">taskFilter</span></span>  | <span data-ttu-id="aca0e-148">Uma função opcional para filtrar quais tarefas são mostradas ao usuário.</span><span class="sxs-lookup"><span data-stu-id="aca0e-148">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="aca0e-149">O exemplo a seguir mostra apenas tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="aca0e-149">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="aca0e-150">O exemplo a seguir mostra como filtrar tarefas que só têm *conjunto de categoria3.*</span><span class="sxs-lookup"><span data-stu-id="aca0e-150">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="aca0e-151">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="aca0e-151">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="aca0e-152">Eventos</span><span class="sxs-lookup"><span data-stu-id="aca0e-152">Events</span></span>

| <span data-ttu-id="aca0e-153">Event</span><span class="sxs-lookup"><span data-stu-id="aca0e-153">Event</span></span> | <span data-ttu-id="aca0e-154">Detalhe</span><span class="sxs-lookup"><span data-stu-id="aca0e-154">Detail</span></span> | <span data-ttu-id="aca0e-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca0e-155">Description</span></span> |
| --- | --- | --- |
| `taskAdded` | <span data-ttu-id="aca0e-156">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="aca0e-156">The detail contains the respective `task` object</span></span> | <span data-ttu-id="aca0e-157">Dispara quando uma nova tarefa é criada.</span><span class="sxs-lookup"><span data-stu-id="aca0e-157">Fires when a new task has been created.</span></span> |
| `taskChanged` | <span data-ttu-id="aca0e-158">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="aca0e-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="aca0e-159">Dispara quando os metadados da tarefa foram alterados, como a marcação concluída.</span><span class="sxs-lookup"><span data-stu-id="aca0e-159">Fires when task metadata has been changed, such as marking completed.</span></span> |
| `taskClick` | <span data-ttu-id="aca0e-160">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="aca0e-160">The detail contains the respective `task` object</span></span> | <span data-ttu-id="aca0e-161">Dispara quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="aca0e-161">Fires when the user clicks or taps on a task.</span></span> |
| `taskRemoved` | <span data-ttu-id="aca0e-162">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="aca0e-162">The detail contains the respective `task` object</span></span> | <span data-ttu-id="aca0e-163">Dispara quando uma tarefa existente foi excluída.</span><span class="sxs-lookup"><span data-stu-id="aca0e-163">Fires when an existing task has been deleted.</span></span> |

<span data-ttu-id="aca0e-164">Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).</span><span class="sxs-lookup"><span data-stu-id="aca0e-164">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="aca0e-165">Modelos</span><span class="sxs-lookup"><span data-stu-id="aca0e-165">Templates</span></span>

<span data-ttu-id="aca0e-166">O `tasks` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="aca0e-166">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="aca0e-167">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes:</span><span class="sxs-lookup"><span data-stu-id="aca0e-167">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="aca0e-168">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="aca0e-168">Data type</span></span>     | <span data-ttu-id="aca0e-169">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="aca0e-169">Data context</span></span>              | <span data-ttu-id="aca0e-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="aca0e-170">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="aca0e-171">tarefa</span><span class="sxs-lookup"><span data-stu-id="aca0e-171">task</span></span>     | <span data-ttu-id="aca0e-172">tarefa: um objeto de tarefa do planner</span><span class="sxs-lookup"><span data-stu-id="aca0e-172">task: a planner task object</span></span> | <span data-ttu-id="aca0e-173">substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="aca0e-173">replaces the whole default task.</span></span> |
| <span data-ttu-id="aca0e-174">detalhes da tarefa</span><span class="sxs-lookup"><span data-stu-id="aca0e-174">task-details</span></span> | <span data-ttu-id="aca0e-175">tarefa: um objeto de tarefa do planner</span><span class="sxs-lookup"><span data-stu-id="aca0e-175">task: a planner task object</span></span> | <span data-ttu-id="aca0e-176">template substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="aca0e-176">template replaces the details section of the task.</span></span> |

<span data-ttu-id="aca0e-177">O exemplo a seguir define um modelo para o componente de tarefas.</span><span class="sxs-lookup"><span data-stu-id="aca0e-177">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="aca0e-178">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aca0e-178">Microsoft Graph permissions</span></span>

<span data-ttu-id="aca0e-179">Esse controle usa as seguintes APIs Graph Microsoft e permissões.</span><span class="sxs-lookup"><span data-stu-id="aca0e-179">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="aca0e-180">Configuração</span><span class="sxs-lookup"><span data-stu-id="aca0e-180">Configuration</span></span> | <span data-ttu-id="aca0e-181">Permissão</span><span class="sxs-lookup"><span data-stu-id="aca0e-181">Permission</span></span> | <span data-ttu-id="aca0e-182">API</span><span class="sxs-lookup"><span data-stu-id="aca0e-182">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="aca0e-183">`groupId` definir e `dataSource` definir como `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="aca0e-183">`groupId` set and `dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="aca0e-184">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="aca0e-184">Group.Read.All</span></span> | <span data-ttu-id="aca0e-185">[/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="aca0e-185">[/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="aca0e-186">`targetId` definir e `dataSource` definir como `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="aca0e-186">`targetId` set and `dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="aca0e-187">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="aca0e-187">Tasks.Read</span></span> | <span data-ttu-id="aca0e-188">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="aca0e-188">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span></span> |
| <span data-ttu-id="aca0e-189">`targetId` set and `dataSource` set to something else than `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="aca0e-189">`targetId` set and `dataSource` set to something else than `TasksSource.todo`</span></span> | <span data-ttu-id="aca0e-190">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="aca0e-190">Group.Read.All</span></span> | <span data-ttu-id="aca0e-191">[/planner/plans/${planId}](/graph/api/plannerplan-get?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="aca0e-191">[/planner/plans/${planId}](/graph/api/plannerplan-get?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="aca0e-192">`dataSource` set to `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="aca0e-192">`dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="aca0e-193">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="aca0e-193">Group.Read.All</span></span> | <span data-ttu-id="aca0e-194">[/me/planner/plans](/graph/api/planneruser-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="aca0e-194">[/me/planner/plans](/graph/api/planneruser-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="aca0e-195">`dataSource` set to `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="aca0e-195">`dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="aca0e-196">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="aca0e-196">Tasks.Read</span></span> | <span data-ttu-id="aca0e-197">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="aca0e-197">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span></span> |
| <span data-ttu-id="aca0e-198">`addTask` definir como `true` e `dataSource` definir como `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="aca0e-198">`addTask` set to `true` and `dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="aca0e-199">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aca0e-199">Group.ReadWrite.All</span></span> | [<span data-ttu-id="aca0e-200">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="aca0e-200">/planner/tasks</span></span>](/graph/api/planner-post-tasks?view=graph-rest-1.0&tabs=http) |
| <span data-ttu-id="aca0e-201">`addTask` definir como `true` e `dataSource` definir como `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="aca0e-201">`addTask` set to `true` and `dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="aca0e-202">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aca0e-202">Tasks.ReadWrite</span></span> | [<span data-ttu-id="aca0e-203">/me/outlook/taskFolders/${parentFolderId}/tasks</span><span class="sxs-lookup"><span data-stu-id="aca0e-203">/me/outlook/taskFolders/${parentFolderId}/tasks</span></span>](/graph/api/outlookuser-post-tasks?view=graph-rest-beta&tabs=csharp) |

<span data-ttu-id="aca0e-204">Para a fonte de dados do Microsoft Planner, buscar e ler tarefas requer a permissão Groups.Read.All.</span><span class="sxs-lookup"><span data-stu-id="aca0e-204">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="aca0e-205">Adicionar, atualizar ou remover tarefas requer a permissão Groups.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="aca0e-205">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="aca0e-206">Autenticação</span><span class="sxs-lookup"><span data-stu-id="aca0e-206">Authentication</span></span>

<span data-ttu-id="aca0e-207">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="aca0e-207">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="aca0e-208">Cache</span><span class="sxs-lookup"><span data-stu-id="aca0e-208">Cache</span></span>

<span data-ttu-id="aca0e-209">O `mgt-tasks` componente não armazena dados em cache.</span><span class="sxs-lookup"><span data-stu-id="aca0e-209">The `mgt-tasks` component doesn't cache any data.</span></span>
