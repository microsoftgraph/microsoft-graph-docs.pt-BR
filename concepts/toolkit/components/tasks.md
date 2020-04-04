---
title: Componente tarefas no Microsoft Graph Toolkit
description: O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com qualquer tarefa no Microsoft Planner ou no Microsoft to-do.
localization_priority: Normal
author: benotter
ms.openlocfilehash: cfd248ca7cb240cd724b8df863383b308121db4b
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144272"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1d3c9-104">Componente tarefas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1d3c9-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1d3c9-105">O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="1d3c9-106">Ele funciona com tarefas no Microsoft Planner ou Microsoft to-do.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>  

<span data-ttu-id="1d3c9-107">Além disso, um usuário pode atribuir um único ou vários usuários do Microsoft Graph a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-107">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="1d3c9-108">Para obter mais detalhes sobre as atribuições do Microsoft Graph, consulte [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="1d3c9-108">For more details about Microsoft Graph assignments, see [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span></span>

## <a name="example"></a><span data-ttu-id="1d3c9-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d3c9-109">Example</span></span>

<span data-ttu-id="1d3c9-110">O exemplo a seguir exibe as tarefas do Microsoft Planner do usuário conectado usando o `mgt-tasks` componente.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-110">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="1d3c9-111">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-111">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="1d3c9-112">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="1d3c9-112">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="1d3c9-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d3c9-113">Properties</span></span>

| <span data-ttu-id="1d3c9-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="1d3c9-114">Attribute</span></span> | <span data-ttu-id="1d3c9-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d3c9-115">Property</span></span> | <span data-ttu-id="1d3c9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d3c9-116">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="1d3c9-117">Data-Source = "todo/planejador"</span><span class="sxs-lookup"><span data-stu-id="1d3c9-117">data-source="todo/planner"</span></span> | <span data-ttu-id="1d3c9-118">dataSource</span><span class="sxs-lookup"><span data-stu-id="1d3c9-118">dataSource</span></span> | <span data-ttu-id="1d3c9-119">Uma enumeração para configurar a fonte de dados para tarefas-Microsoft to-do ou Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-119">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="1d3c9-120">O padrão é `planner`.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-120">Default is `planner`.</span></span> |
| <span data-ttu-id="1d3c9-121">somente leitura</span><span class="sxs-lookup"><span data-stu-id="1d3c9-121">read-only</span></span> | <span data-ttu-id="1d3c9-122">readOnly</span><span class="sxs-lookup"><span data-stu-id="1d3c9-122">readOnly</span></span> | <span data-ttu-id="1d3c9-123">Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="1d3c9-123">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="1d3c9-124">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-124">Default is `false`.</span></span> |
| <span data-ttu-id="1d3c9-125">Ocultar-cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d3c9-125">hide-header</span></span> | <span data-ttu-id="1d3c9-126">hideHeader</span><span class="sxs-lookup"><span data-stu-id="1d3c9-126">hideHeader</span></span> | <span data-ttu-id="1d3c9-127">Um booliano para mostrar ou ocultar o cabeçalho do componente.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-127">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="1d3c9-128">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-128">Default is `false`.</span></span> |
| <span data-ttu-id="1d3c9-129">Hide-opções</span><span class="sxs-lookup"><span data-stu-id="1d3c9-129">hide-options</span></span> | <span data-ttu-id="1d3c9-130">hideoptions</span><span class="sxs-lookup"><span data-stu-id="1d3c9-130">hideOptions</span></span> | <span data-ttu-id="1d3c9-131">Um booliano para mostrar ou ocultar as opções nas tarefas.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-131">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="1d3c9-132">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-132">Default is `false`.</span></span>
| <span data-ttu-id="1d3c9-133">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="1d3c9-133">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="1d3c9-134">initialid</span><span class="sxs-lookup"><span data-stu-id="1d3c9-134">initialId</span></span> | <span data-ttu-id="1d3c9-135">Uma ID de cadeia de caracteres para definir o planejador ou pasta inicialmente exibido para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-135">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="1d3c9-136">Initial-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="1d3c9-136">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="1d3c9-137">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="1d3c9-137">initialBucketId</span></span> | <span data-ttu-id="1d3c9-138">Uma ID de cadeia de caracteres para definir o Bucket exibido inicialmente (somente a fonte de dados do Planner) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-138">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="1d3c9-139">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="1d3c9-139">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="1d3c9-140">targetId</span><span class="sxs-lookup"><span data-stu-id="1d3c9-140">targetId</span></span> | <span data-ttu-id="1d3c9-141">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou ID de pasta fornecido.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-141">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="1d3c9-142">Target-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="1d3c9-142">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="1d3c9-143">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="1d3c9-143">targetBucketId</span></span>  | <span data-ttu-id="1d3c9-144">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de Bucket fornecida (somente a fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="1d3c9-144">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="1d3c9-145">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="1d3c9-145">group-id</span></span> | <span data-ttu-id="1d3c9-146">groupId</span><span class="sxs-lookup"><span data-stu-id="1d3c9-146">groupId</span></span>  | <span data-ttu-id="1d3c9-147">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de grupo (somente fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="1d3c9-147">A string ID to lock the tasks interface to the group ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="1d3c9-148">Não disponível</span><span class="sxs-lookup"><span data-stu-id="1d3c9-148">N/A</span></span> | <span data-ttu-id="1d3c9-149">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="1d3c9-149">isNewTaskVisible</span></span>  | <span data-ttu-id="1d3c9-150">Determina se a exibição de nova tarefa é visível no processamento.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-150">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="1d3c9-151">Não disponível</span><span class="sxs-lookup"><span data-stu-id="1d3c9-151">N/A</span></span> | <span data-ttu-id="1d3c9-152">taskFilter</span><span class="sxs-lookup"><span data-stu-id="1d3c9-152">taskFilter</span></span>  | <span data-ttu-id="1d3c9-153">Uma função opcional para filtrar quais tarefas são exibidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-153">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="1d3c9-154">O exemplo a seguir mostra apenas as tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-154">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="1d3c9-155">O exemplo a seguir mostra como filtrar tarefas que têm apenas *category3* definido.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-155">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="1d3c9-156">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="1d3c9-156">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="1d3c9-157">Eventos</span><span class="sxs-lookup"><span data-stu-id="1d3c9-157">Events</span></span>
| <span data-ttu-id="1d3c9-158">Evento</span><span class="sxs-lookup"><span data-stu-id="1d3c9-158">Event</span></span> | <span data-ttu-id="1d3c9-159">Detalhe</span><span class="sxs-lookup"><span data-stu-id="1d3c9-159">Detail</span></span> | <span data-ttu-id="1d3c9-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d3c9-160">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1d3c9-161">taskClick</span><span class="sxs-lookup"><span data-stu-id="1d3c9-161">taskClick</span></span> | <span data-ttu-id="1d3c9-162">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="1d3c9-162">The detail contains the respective `task` object</span></span> | <span data-ttu-id="1d3c9-163">Acionado quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-163">Fired when the user clicks or taps on a task.</span></span> |

## <a name="templates"></a><span data-ttu-id="1d3c9-164">Modelos</span><span class="sxs-lookup"><span data-stu-id="1d3c9-164">Templates</span></span>

<span data-ttu-id="1d3c9-165">O `tasks` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-165">The `tasks` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="1d3c9-166">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="1d3c9-166">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="1d3c9-167">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="1d3c9-167">Data type</span></span>     | <span data-ttu-id="1d3c9-168">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="1d3c9-168">Data context</span></span>              | <span data-ttu-id="1d3c9-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d3c9-169">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="1d3c9-170">tarefa</span><span class="sxs-lookup"><span data-stu-id="1d3c9-170">task</span></span>     | <span data-ttu-id="1d3c9-171">tarefa: um planejador ou objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="1d3c9-171">task: a planner or to-do task object</span></span> | <span data-ttu-id="1d3c9-172">Substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-172">replaces the whole default task.</span></span> |
| <span data-ttu-id="1d3c9-173">tarefa-detalhes</span><span class="sxs-lookup"><span data-stu-id="1d3c9-173">task-details</span></span> | <span data-ttu-id="1d3c9-174">tarefa: um planejador ou objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="1d3c9-174">task: a planner or to-do task object</span></span> | <span data-ttu-id="1d3c9-175">o modelo substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-175">template replaces the details section of the task.</span></span> |

<span data-ttu-id="1d3c9-176">O exemplo a seguir define um modelo para o componente tarefas.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-176">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="1d3c9-177">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1d3c9-177">Microsoft Graph permissions</span></span>

<span data-ttu-id="1d3c9-178">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-178">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="1d3c9-179">Resource</span><span class="sxs-lookup"><span data-stu-id="1d3c9-179">Resource</span></span> | <span data-ttu-id="1d3c9-180">Permissão</span><span class="sxs-lookup"><span data-stu-id="1d3c9-180">Permission</span></span> |
| - | - |
| <span data-ttu-id="1d3c9-181">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="1d3c9-181">/me/planner/plans</span></span> | <span data-ttu-id="1d3c9-182">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d3c9-182">Group.Read.All</span></span> |
| <span data-ttu-id="1d3c9-183">/Planner/Plans/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="1d3c9-183">/planner/plans/${id}</span></span> | <span data-ttu-id="1d3c9-184">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d3c9-184">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1d3c9-185">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="1d3c9-185">/planner/tasks</span></span> | <span data-ttu-id="1d3c9-186">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d3c9-186">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1d3c9-187">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="1d3c9-187">/me/outlook/taskGroups</span></span> | <span data-ttu-id="1d3c9-188">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1d3c9-188">Tasks.Read</span></span> |
| <span data-ttu-id="1d3c9-189">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="1d3c9-189">/me/outlook/taskFolders</span></span> | <span data-ttu-id="1d3c9-190">Tarefas. Read, Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d3c9-190">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="1d3c9-191">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="1d3c9-191">/me/outlook/tasks</span></span> | <span data-ttu-id="1d3c9-192">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d3c9-192">Tasks.ReadWrite</span></span> |
| <span data-ttu-id="1d3c9-193">/groups/$ {Group-ID}/Planner/Plans</span><span class="sxs-lookup"><span data-stu-id="1d3c9-193">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="1d3c9-194">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d3c9-194">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="1d3c9-195">Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-195">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="1d3c9-196">Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-196">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="1d3c9-197">Para a fonte de dados do Microsoft todo, a permissão Tasks. Read é necessária para buscar e ler tarefas.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-197">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="1d3c9-198">Adicionar, atualizar ou remover tarefas requer a permissão Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="1d3c9-198">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="1d3c9-199">Autenticação</span><span class="sxs-lookup"><span data-stu-id="1d3c9-199">Authentication</span></span>

<span data-ttu-id="1d3c9-200">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="1d3c9-200">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
