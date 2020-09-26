---
title: Componente tarefas no Microsoft Graph Toolkit
description: O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com qualquer tarefa no Microsoft Planner ou no Microsoft to-do.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 54e72c5756eb029d7219c07a591c956207a1c0e6
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288557"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="3a4bc-104">Componente tarefas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="3a4bc-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3a4bc-105">O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="3a4bc-106">Ele funciona com tarefas no Microsoft Planner ou Microsoft to-do.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>  

<span data-ttu-id="3a4bc-107">Além disso, um usuário pode atribuir um único ou vários usuários do Microsoft Graph a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-107">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="3a4bc-108">Para obter mais detalhes sobre as atribuições do Microsoft Graph, consulte [plannerAssignments](/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="3a4bc-108">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span></span>

## <a name="example"></a><span data-ttu-id="3a4bc-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a4bc-109">Example</span></span>

<span data-ttu-id="3a4bc-110">O exemplo a seguir exibe as tarefas do Microsoft Planner do usuário conectado usando o `mgt-tasks` componente.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-110">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="3a4bc-111">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-111">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="3a4bc-112">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="3a4bc-112">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="3a4bc-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a4bc-113">Properties</span></span>

| <span data-ttu-id="3a4bc-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="3a4bc-114">Attribute</span></span> | <span data-ttu-id="3a4bc-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a4bc-115">Property</span></span> | <span data-ttu-id="3a4bc-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a4bc-116">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="3a4bc-117">Data-Source = "todo/planejador"</span><span class="sxs-lookup"><span data-stu-id="3a4bc-117">data-source="todo/planner"</span></span> | <span data-ttu-id="3a4bc-118">dataSource</span><span class="sxs-lookup"><span data-stu-id="3a4bc-118">dataSource</span></span> | <span data-ttu-id="3a4bc-119">Uma enumeração para configurar a fonte de dados para tarefas-Microsoft to-do ou Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-119">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="3a4bc-120">O padrão é `planner`.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-120">Default is `planner`.</span></span> |
| <span data-ttu-id="3a4bc-121">somente leitura</span><span class="sxs-lookup"><span data-stu-id="3a4bc-121">read-only</span></span> | <span data-ttu-id="3a4bc-122">readOnly</span><span class="sxs-lookup"><span data-stu-id="3a4bc-122">readOnly</span></span> | <span data-ttu-id="3a4bc-123">Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="3a4bc-123">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="3a4bc-124">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-124">Default is `false`.</span></span> |
| <span data-ttu-id="3a4bc-125">Ocultar-cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a4bc-125">hide-header</span></span> | <span data-ttu-id="3a4bc-126">hideHeader</span><span class="sxs-lookup"><span data-stu-id="3a4bc-126">hideHeader</span></span> | <span data-ttu-id="3a4bc-127">Um booliano para mostrar ou ocultar o cabeçalho do componente.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-127">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="3a4bc-128">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-128">Default is `false`.</span></span> |
| <span data-ttu-id="3a4bc-129">Hide-opções</span><span class="sxs-lookup"><span data-stu-id="3a4bc-129">hide-options</span></span> | <span data-ttu-id="3a4bc-130">hideoptions</span><span class="sxs-lookup"><span data-stu-id="3a4bc-130">hideOptions</span></span> | <span data-ttu-id="3a4bc-131">Um booliano para mostrar ou ocultar as opções nas tarefas.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-131">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="3a4bc-132">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-132">Default is `false`.</span></span>
| <span data-ttu-id="3a4bc-133">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="3a4bc-133">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="3a4bc-134">initialid</span><span class="sxs-lookup"><span data-stu-id="3a4bc-134">initialId</span></span> | <span data-ttu-id="3a4bc-135">Uma ID de cadeia de caracteres para definir o planejador ou pasta inicialmente exibido para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-135">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="3a4bc-136">Initial-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="3a4bc-136">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="3a4bc-137">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="3a4bc-137">initialBucketId</span></span> | <span data-ttu-id="3a4bc-138">Uma ID de cadeia de caracteres para definir o Bucket exibido inicialmente (somente a fonte de dados do Planner) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-138">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="3a4bc-139">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="3a4bc-139">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="3a4bc-140">targetId</span><span class="sxs-lookup"><span data-stu-id="3a4bc-140">targetId</span></span> | <span data-ttu-id="3a4bc-141">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou ID de pasta fornecido.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-141">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="3a4bc-142">Target-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="3a4bc-142">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="3a4bc-143">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="3a4bc-143">targetBucketId</span></span>  | <span data-ttu-id="3a4bc-144">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de Bucket fornecida (somente a fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="3a4bc-144">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="3a4bc-145">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="3a4bc-145">group-id</span></span> | <span data-ttu-id="3a4bc-146">groupId</span><span class="sxs-lookup"><span data-stu-id="3a4bc-146">groupId</span></span>  | <span data-ttu-id="3a4bc-147">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de grupo (somente fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="3a4bc-147">A string ID to lock the tasks interface to the group ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="3a4bc-148">N/D</span><span class="sxs-lookup"><span data-stu-id="3a4bc-148">N/A</span></span> | <span data-ttu-id="3a4bc-149">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="3a4bc-149">isNewTaskVisible</span></span>  | <span data-ttu-id="3a4bc-150">Determina se a exibição de nova tarefa é visível no processamento.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-150">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="3a4bc-151">N/D</span><span class="sxs-lookup"><span data-stu-id="3a4bc-151">N/A</span></span> | <span data-ttu-id="3a4bc-152">taskFilter</span><span class="sxs-lookup"><span data-stu-id="3a4bc-152">taskFilter</span></span>  | <span data-ttu-id="3a4bc-153">Uma função opcional para filtrar quais tarefas são exibidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-153">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="3a4bc-154">O exemplo a seguir mostra apenas as tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-154">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="3a4bc-155">O exemplo a seguir mostra como filtrar tarefas que têm apenas *category3* definido.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-155">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="3a4bc-156">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="3a4bc-156">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="3a4bc-157">Eventos</span><span class="sxs-lookup"><span data-stu-id="3a4bc-157">Events</span></span>
| <span data-ttu-id="3a4bc-158">Evento</span><span class="sxs-lookup"><span data-stu-id="3a4bc-158">Event</span></span> | <span data-ttu-id="3a4bc-159">Detalhe</span><span class="sxs-lookup"><span data-stu-id="3a4bc-159">Detail</span></span> | <span data-ttu-id="3a4bc-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a4bc-160">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="3a4bc-161">taskClick</span><span class="sxs-lookup"><span data-stu-id="3a4bc-161">taskClick</span></span> | <span data-ttu-id="3a4bc-162">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="3a4bc-162">The detail contains the respective `task` object</span></span> | <span data-ttu-id="3a4bc-163">Acionado quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-163">Fired when the user clicks or taps on a task.</span></span> |

## <a name="templates"></a><span data-ttu-id="3a4bc-164">Modelos</span><span class="sxs-lookup"><span data-stu-id="3a4bc-164">Templates</span></span>

<span data-ttu-id="3a4bc-165">O `tasks` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-165">The `tasks` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="3a4bc-166">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="3a4bc-166">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="3a4bc-167">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="3a4bc-167">Data type</span></span>     | <span data-ttu-id="3a4bc-168">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="3a4bc-168">Data context</span></span>              | <span data-ttu-id="3a4bc-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a4bc-169">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="3a4bc-170">tarefa</span><span class="sxs-lookup"><span data-stu-id="3a4bc-170">task</span></span>     | <span data-ttu-id="3a4bc-171">tarefa: um planejador ou objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="3a4bc-171">task: a planner or to-do task object</span></span> | <span data-ttu-id="3a4bc-172">Substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-172">replaces the whole default task.</span></span> |
| <span data-ttu-id="3a4bc-173">tarefa-detalhes</span><span class="sxs-lookup"><span data-stu-id="3a4bc-173">task-details</span></span> | <span data-ttu-id="3a4bc-174">tarefa: um planejador ou objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="3a4bc-174">task: a planner or to-do task object</span></span> | <span data-ttu-id="3a4bc-175">o modelo substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-175">template replaces the details section of the task.</span></span> |

<span data-ttu-id="3a4bc-176">O exemplo a seguir define um modelo para o componente tarefas.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-176">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="3a4bc-177">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3a4bc-177">Microsoft Graph permissions</span></span>

<span data-ttu-id="3a4bc-178">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-178">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="3a4bc-179">Resource</span><span class="sxs-lookup"><span data-stu-id="3a4bc-179">Resource</span></span> | <span data-ttu-id="3a4bc-180">Permissão</span><span class="sxs-lookup"><span data-stu-id="3a4bc-180">Permission</span></span> |
| - | - |
| <span data-ttu-id="3a4bc-181">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="3a4bc-181">/me/planner/plans</span></span> | <span data-ttu-id="3a4bc-182">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a4bc-182">Group.Read.All</span></span> |
| <span data-ttu-id="3a4bc-183">/Planner/Plans/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="3a4bc-183">/planner/plans/${id}</span></span> | <span data-ttu-id="3a4bc-184">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a4bc-184">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3a4bc-185">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="3a4bc-185">/planner/tasks</span></span> | <span data-ttu-id="3a4bc-186">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a4bc-186">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3a4bc-187">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="3a4bc-187">/me/outlook/taskGroups</span></span> | <span data-ttu-id="3a4bc-188">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="3a4bc-188">Tasks.Read</span></span> |
| <span data-ttu-id="3a4bc-189">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="3a4bc-189">/me/outlook/taskFolders</span></span> | <span data-ttu-id="3a4bc-190">Tarefas. Read, Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a4bc-190">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="3a4bc-191">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="3a4bc-191">/me/outlook/tasks</span></span> | <span data-ttu-id="3a4bc-192">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a4bc-192">Tasks.ReadWrite</span></span> |
| <span data-ttu-id="3a4bc-193">/groups/$ {Group-ID}/Planner/Plans</span><span class="sxs-lookup"><span data-stu-id="3a4bc-193">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="3a4bc-194">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a4bc-194">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="3a4bc-195">Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-195">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="3a4bc-196">Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-196">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="3a4bc-197">Para a fonte de dados do Microsoft todo, a permissão Tasks. Read é necessária para buscar e ler tarefas.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-197">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="3a4bc-198">Adicionar, atualizar ou remover tarefas requer a permissão Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="3a4bc-198">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="3a4bc-199">Autenticação</span><span class="sxs-lookup"><span data-stu-id="3a4bc-199">Authentication</span></span>

<span data-ttu-id="3a4bc-200">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="3a4bc-200">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>