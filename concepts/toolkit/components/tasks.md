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
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8b60e-104">Componente tarefas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="8b60e-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8b60e-105">O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas.</span><span class="sxs-lookup"><span data-stu-id="8b60e-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="8b60e-106">Ele funciona com tarefas no Microsoft Planner ou Microsoft to-do.</span><span class="sxs-lookup"><span data-stu-id="8b60e-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>  

<span data-ttu-id="8b60e-107">Além disso, um usuário pode atribuir um único ou vários usuários do Microsoft Graph a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="8b60e-107">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="8b60e-108">Para obter mais detalhes sobre as atribuições do Microsoft Graph, consulte [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="8b60e-108">For more details about Microsoft Graph assignments, see [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span></span>

## <a name="example"></a><span data-ttu-id="8b60e-109">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b60e-109">Example</span></span>

<span data-ttu-id="8b60e-110">O exemplo a seguir exibe as tarefas do Microsoft Planner do usuário conectado usando o `mgt-tasks` componente.</span><span class="sxs-lookup"><span data-stu-id="8b60e-110">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="8b60e-111">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="8b60e-111">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="8b60e-112">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="8b60e-112">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="8b60e-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b60e-113">Properties</span></span>

| <span data-ttu-id="8b60e-114">Atributo</span><span class="sxs-lookup"><span data-stu-id="8b60e-114">Attribute</span></span> | <span data-ttu-id="8b60e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b60e-115">Property</span></span> | <span data-ttu-id="8b60e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b60e-116">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="8b60e-117">Data-Source = "todo/planejador"</span><span class="sxs-lookup"><span data-stu-id="8b60e-117">data-source="todo/planner"</span></span> | <span data-ttu-id="8b60e-118">dataSource</span><span class="sxs-lookup"><span data-stu-id="8b60e-118">dataSource</span></span> | <span data-ttu-id="8b60e-119">Uma enumeração para configurar a fonte de dados para tarefas-Microsoft to-do ou Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="8b60e-119">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="8b60e-120">O padrão é `planner`.</span><span class="sxs-lookup"><span data-stu-id="8b60e-120">Default is `planner`.</span></span> |
| <span data-ttu-id="8b60e-121">somente leitura</span><span class="sxs-lookup"><span data-stu-id="8b60e-121">read-only</span></span> | <span data-ttu-id="8b60e-122">readOnly</span><span class="sxs-lookup"><span data-stu-id="8b60e-122">readOnly</span></span> | <span data-ttu-id="8b60e-123">Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="8b60e-123">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="8b60e-124">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="8b60e-124">Default is `false`.</span></span> |
| <span data-ttu-id="8b60e-125">Ocultar-cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b60e-125">hide-header</span></span> | <span data-ttu-id="8b60e-126">hideHeader</span><span class="sxs-lookup"><span data-stu-id="8b60e-126">hideHeader</span></span> | <span data-ttu-id="8b60e-127">Um booliano para mostrar ou ocultar o cabeçalho do componente.</span><span class="sxs-lookup"><span data-stu-id="8b60e-127">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="8b60e-128">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="8b60e-128">Default is `false`.</span></span> |
| <span data-ttu-id="8b60e-129">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="8b60e-129">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="8b60e-130">initialid</span><span class="sxs-lookup"><span data-stu-id="8b60e-130">initialId</span></span> | <span data-ttu-id="8b60e-131">Uma ID de cadeia de caracteres para definir o planejador ou pasta inicialmente exibido para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="8b60e-131">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="8b60e-132">Initial-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="8b60e-132">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="8b60e-133">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="8b60e-133">initialBucketId</span></span> | <span data-ttu-id="8b60e-134">Uma ID de cadeia de caracteres para definir o Bucket exibido inicialmente (somente a fonte de dados do Planner) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="8b60e-134">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="8b60e-135">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="8b60e-135">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="8b60e-136">targetId</span><span class="sxs-lookup"><span data-stu-id="8b60e-136">targetId</span></span> | <span data-ttu-id="8b60e-137">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou ID de pasta fornecido.</span><span class="sxs-lookup"><span data-stu-id="8b60e-137">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="8b60e-138">Target-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="8b60e-138">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="8b60e-139">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="8b60e-139">targetBucketId</span></span>  | <span data-ttu-id="8b60e-140">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de Bucket fornecida (somente a fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="8b60e-140">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="8b60e-141">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="8b60e-141">group-id</span></span> | <span data-ttu-id="8b60e-142">groupId</span><span class="sxs-lookup"><span data-stu-id="8b60e-142">groupId</span></span>  | <span data-ttu-id="8b60e-143">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de grupo (somente fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="8b60e-143">A string ID to lock the tasks interface to the group ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="8b60e-144">Não disponível</span><span class="sxs-lookup"><span data-stu-id="8b60e-144">N/A</span></span> | <span data-ttu-id="8b60e-145">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="8b60e-145">isNewTaskVisible</span></span>  | <span data-ttu-id="8b60e-146">Determina se a exibição de nova tarefa é visível no processamento.</span><span class="sxs-lookup"><span data-stu-id="8b60e-146">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="8b60e-147">Não disponível</span><span class="sxs-lookup"><span data-stu-id="8b60e-147">N/A</span></span> | <span data-ttu-id="8b60e-148">taskFilter</span><span class="sxs-lookup"><span data-stu-id="8b60e-148">taskFilter</span></span>  | <span data-ttu-id="8b60e-149">Uma função opcional para filtrar quais tarefas são exibidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="8b60e-149">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="8b60e-150">O exemplo a seguir mostra apenas as tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="8b60e-150">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="8b60e-151">O exemplo a seguir mostra como filtrar tarefas que têm apenas *category3* definido.</span><span class="sxs-lookup"><span data-stu-id="8b60e-151">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="8b60e-152">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="8b60e-152">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="8b60e-153">Eventos</span><span class="sxs-lookup"><span data-stu-id="8b60e-153">Events</span></span>
| <span data-ttu-id="8b60e-154">Evento</span><span class="sxs-lookup"><span data-stu-id="8b60e-154">Event</span></span> | <span data-ttu-id="8b60e-155">Detalhe</span><span class="sxs-lookup"><span data-stu-id="8b60e-155">Detail</span></span> | <span data-ttu-id="8b60e-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b60e-156">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8b60e-157">taskClick</span><span class="sxs-lookup"><span data-stu-id="8b60e-157">taskClick</span></span> | <span data-ttu-id="8b60e-158">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="8b60e-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="8b60e-159">Acionado quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="8b60e-159">Fired when the user clicks or taps on a task.</span></span> |

## <a name="templates"></a><span data-ttu-id="8b60e-160">Modelos</span><span class="sxs-lookup"><span data-stu-id="8b60e-160">Templates</span></span>

<span data-ttu-id="8b60e-161">O `tasks` componente oferece suporte a vários [modelos](../templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="8b60e-161">The `tasks` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="8b60e-162">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina `data-type` o valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="8b60e-162">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="8b60e-163">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="8b60e-163">Data type</span></span>     | <span data-ttu-id="8b60e-164">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="8b60e-164">Data context</span></span>              | <span data-ttu-id="8b60e-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b60e-165">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="8b60e-166">tarefa</span><span class="sxs-lookup"><span data-stu-id="8b60e-166">task</span></span>     | <span data-ttu-id="8b60e-167">tarefa: um planejador ou objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="8b60e-167">task: a planner or to-do task object</span></span> | <span data-ttu-id="8b60e-168">Substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="8b60e-168">replaces the whole default task.</span></span> |
| <span data-ttu-id="8b60e-169">tarefa-detalhes</span><span class="sxs-lookup"><span data-stu-id="8b60e-169">task-details</span></span> | <span data-ttu-id="8b60e-170">tarefa: um planejador ou objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="8b60e-170">task: a planner or to-do task object</span></span> | <span data-ttu-id="8b60e-171">o modelo substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="8b60e-171">template replaces the details section of the task.</span></span> |

<span data-ttu-id="8b60e-172">O exemplo a seguir define um modelo para o componente tarefas.</span><span class="sxs-lookup"><span data-stu-id="8b60e-172">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8b60e-173">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8b60e-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="8b60e-174">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8b60e-174">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="8b60e-175">Resource</span><span class="sxs-lookup"><span data-stu-id="8b60e-175">Resource</span></span> | <span data-ttu-id="8b60e-176">Permissão</span><span class="sxs-lookup"><span data-stu-id="8b60e-176">Permission</span></span> |
| - | - |
| <span data-ttu-id="8b60e-177">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="8b60e-177">/me/planner/plans</span></span> | <span data-ttu-id="8b60e-178">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b60e-178">Group.Read.All</span></span> |
| <span data-ttu-id="8b60e-179">/Planner/Plans/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="8b60e-179">/planner/plans/${id}</span></span> | <span data-ttu-id="8b60e-180">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b60e-180">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8b60e-181">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="8b60e-181">/planner/tasks</span></span> | <span data-ttu-id="8b60e-182">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b60e-182">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8b60e-183">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="8b60e-183">/me/outlook/taskGroups</span></span> | <span data-ttu-id="8b60e-184">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="8b60e-184">Tasks.Read</span></span> |
| <span data-ttu-id="8b60e-185">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="8b60e-185">/me/outlook/taskFolders</span></span> | <span data-ttu-id="8b60e-186">Tarefas. Read, Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b60e-186">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="8b60e-187">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="8b60e-187">/me/outlook/tasks</span></span> | <span data-ttu-id="8b60e-188">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b60e-188">Tasks.ReadWrite</span></span> |
| <span data-ttu-id="8b60e-189">/groups/$ {Group-ID}/Planner/Plans</span><span class="sxs-lookup"><span data-stu-id="8b60e-189">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="8b60e-190">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b60e-190">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="8b60e-191">Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All.</span><span class="sxs-lookup"><span data-stu-id="8b60e-191">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="8b60e-192">Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="8b60e-192">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="8b60e-193">Para a fonte de dados do Microsoft todo, a permissão Tasks. Read é necessária para buscar e ler tarefas.</span><span class="sxs-lookup"><span data-stu-id="8b60e-193">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="8b60e-194">Adicionar, atualizar ou remover tarefas requer a permissão Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="8b60e-194">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="8b60e-195">Autenticação</span><span class="sxs-lookup"><span data-stu-id="8b60e-195">Authentication</span></span>

<span data-ttu-id="8b60e-196">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="8b60e-196">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
