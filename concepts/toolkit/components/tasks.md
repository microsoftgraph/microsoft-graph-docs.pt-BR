---
title: Componente Tarefas no microsoft graph Toolkit
description: O componente Tarefas permite ao usuário exibir, adicionar, remover, concluir ou editar tarefas. Ele funciona com qualquer tarefa no Microsoft Planner.
localization_priority: Normal
author: benotter
ms.openlocfilehash: d07db8f1a261f1cff96175a25665f08eff615d67
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266798"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="886c3-104">Componente Tarefas no microsoft graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="886c3-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="886c3-105">O componente Tarefas permite ao usuário exibir, adicionar, remover, concluir ou editar tarefas do Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="886c3-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks from Microsoft Planner.</span></span>  

<span data-ttu-id="886c3-106">Além disso, um usuário pode atribuir um único ou vários usuários do Microsoft Graph a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="886c3-106">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="886c3-107">Para obter mais detalhes sobre as atribuições do Microsoft Graph, consulte [plannerAssignments](/graph/api/resources/plannerassignments).</span><span class="sxs-lookup"><span data-stu-id="886c3-107">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments).</span></span>

## <a name="example"></a><span data-ttu-id="886c3-108">Exemplo</span><span class="sxs-lookup"><span data-stu-id="886c3-108">Example</span></span>

<span data-ttu-id="886c3-109">O exemplo a seguir exibe as tarefas do Microsoft Planner do usuário de logo-in usando o `mgt-tasks` componente.</span><span class="sxs-lookup"><span data-stu-id="886c3-109">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="886c3-110">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="886c3-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="886c3-111">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="886c3-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="886c3-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="886c3-112">Properties</span></span>

| <span data-ttu-id="886c3-113">Atributo</span><span class="sxs-lookup"><span data-stu-id="886c3-113">Attribute</span></span> | <span data-ttu-id="886c3-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="886c3-114">Property</span></span> | <span data-ttu-id="886c3-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="886c3-115">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="886c3-116">somente leitura</span><span class="sxs-lookup"><span data-stu-id="886c3-116">read-only</span></span> | <span data-ttu-id="886c3-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="886c3-117">readOnly</span></span> | <span data-ttu-id="886c3-118">Um Boolean para definir a interface da tarefa a ser lida somente (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="886c3-118">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="886c3-119">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="886c3-119">Default is `false`.</span></span> |
| <span data-ttu-id="886c3-120">hide-header</span><span class="sxs-lookup"><span data-stu-id="886c3-120">hide-header</span></span> | <span data-ttu-id="886c3-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="886c3-121">hideHeader</span></span> | <span data-ttu-id="886c3-122">Um Boolean para mostrar ou ocultar o header do componente.</span><span class="sxs-lookup"><span data-stu-id="886c3-122">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="886c3-123">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="886c3-123">Default is `false`.</span></span> |
| <span data-ttu-id="886c3-124">hide-options</span><span class="sxs-lookup"><span data-stu-id="886c3-124">hide-options</span></span> | <span data-ttu-id="886c3-125">hideOptions</span><span class="sxs-lookup"><span data-stu-id="886c3-125">hideOptions</span></span> | <span data-ttu-id="886c3-126">Um Boolean para mostrar ou ocultar as opções em tarefas.</span><span class="sxs-lookup"><span data-stu-id="886c3-126">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="886c3-127">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="886c3-127">Default is `false`.</span></span>
| <span data-ttu-id="886c3-128">initial-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="886c3-128">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="886c3-129">initialId</span><span class="sxs-lookup"><span data-stu-id="886c3-129">initialId</span></span> | <span data-ttu-id="886c3-130">Uma ID de cadeia de caracteres para definir o planejador ou pasta exibido inicialmente como a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="886c3-130">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="886c3-131">initial-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="886c3-131">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="886c3-132">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="886c3-132">initialBucketId</span></span> | <span data-ttu-id="886c3-133">Uma ID de cadeia de caracteres para definir o bucket exibido inicialmente (Planner Data-Source Somente) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="886c3-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="886c3-134">target-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="886c3-134">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="886c3-135">targetId</span><span class="sxs-lookup"><span data-stu-id="886c3-135">targetId</span></span> | <span data-ttu-id="886c3-136">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou a ID de pasta fornecida.</span><span class="sxs-lookup"><span data-stu-id="886c3-136">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="886c3-137">target-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="886c3-137">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="886c3-138">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="886c3-138">targetBucketId</span></span>  | <span data-ttu-id="886c3-139">Uma ID de cadeia de caracteres para bloquear a interface de tarefas na ID de bucket fornecida (Planner Data-Source Only).</span><span class="sxs-lookup"><span data-stu-id="886c3-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="886c3-140">group-id</span><span class="sxs-lookup"><span data-stu-id="886c3-140">group-id</span></span> | <span data-ttu-id="886c3-141">groupId</span><span class="sxs-lookup"><span data-stu-id="886c3-141">groupId</span></span>  | <span data-ttu-id="886c3-142">Uma ID de cadeia de caracteres para bloquear a interface de tarefas na ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="886c3-142">A string ID to lock the tasks interface to the group ID.</span></span> |
| <span data-ttu-id="886c3-143">N/D</span><span class="sxs-lookup"><span data-stu-id="886c3-143">N/A</span></span> | <span data-ttu-id="886c3-144">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="886c3-144">isNewTaskVisible</span></span>  | <span data-ttu-id="886c3-145">Determina se o novo exibição de tarefa está visível na renderização.</span><span class="sxs-lookup"><span data-stu-id="886c3-145">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="886c3-146">N/D</span><span class="sxs-lookup"><span data-stu-id="886c3-146">N/A</span></span> | <span data-ttu-id="886c3-147">taskFilter</span><span class="sxs-lookup"><span data-stu-id="886c3-147">taskFilter</span></span>  | <span data-ttu-id="886c3-148">Uma função opcional para filtrar quais tarefas são mostradas ao usuário.</span><span class="sxs-lookup"><span data-stu-id="886c3-148">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="886c3-149">O exemplo a seguir mostra apenas tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="886c3-149">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="886c3-150">O exemplo a seguir mostra como filtrar tarefas que só têm *conjunto de categoria3.*</span><span class="sxs-lookup"><span data-stu-id="886c3-150">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="886c3-151">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="886c3-151">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="886c3-152">Eventos</span><span class="sxs-lookup"><span data-stu-id="886c3-152">Events</span></span>
| <span data-ttu-id="886c3-153">Evento</span><span class="sxs-lookup"><span data-stu-id="886c3-153">Event</span></span> | <span data-ttu-id="886c3-154">Detalhe</span><span class="sxs-lookup"><span data-stu-id="886c3-154">Detail</span></span> | <span data-ttu-id="886c3-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="886c3-155">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="886c3-156">taskAdded</span><span class="sxs-lookup"><span data-stu-id="886c3-156">taskAdded</span></span> | <span data-ttu-id="886c3-157">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="886c3-157">The detail contains the respective `task` object</span></span> | <span data-ttu-id="886c3-158">Dispara quando uma nova tarefa é criada.</span><span class="sxs-lookup"><span data-stu-id="886c3-158">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="886c3-159">taskChanged</span><span class="sxs-lookup"><span data-stu-id="886c3-159">taskChanged</span></span> | <span data-ttu-id="886c3-160">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="886c3-160">The detail contains the respective `task` object</span></span> | <span data-ttu-id="886c3-161">Dispara quando os metadados da tarefa foram alterados, como a marcação concluída.</span><span class="sxs-lookup"><span data-stu-id="886c3-161">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="886c3-162">taskClick</span><span class="sxs-lookup"><span data-stu-id="886c3-162">taskClick</span></span> | <span data-ttu-id="886c3-163">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="886c3-163">The detail contains the respective `task` object</span></span> | <span data-ttu-id="886c3-164">Dispara quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="886c3-164">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="886c3-165">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="886c3-165">taskRemoved</span></span> | <span data-ttu-id="886c3-166">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="886c3-166">The detail contains the respective `task` object</span></span> | <span data-ttu-id="886c3-167">Dispara quando uma tarefa existente foi excluída.</span><span class="sxs-lookup"><span data-stu-id="886c3-167">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="886c3-168">Modelos</span><span class="sxs-lookup"><span data-stu-id="886c3-168">Templates</span></span>

<span data-ttu-id="886c3-169">O `tasks` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="886c3-169">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="886c3-170">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes:</span><span class="sxs-lookup"><span data-stu-id="886c3-170">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="886c3-171">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="886c3-171">Data type</span></span>     | <span data-ttu-id="886c3-172">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="886c3-172">Data context</span></span>              | <span data-ttu-id="886c3-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="886c3-173">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="886c3-174">tarefa</span><span class="sxs-lookup"><span data-stu-id="886c3-174">task</span></span>     | <span data-ttu-id="886c3-175">tarefa: um objeto de tarefa do planner</span><span class="sxs-lookup"><span data-stu-id="886c3-175">task: a planner task object</span></span> | <span data-ttu-id="886c3-176">substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="886c3-176">replaces the whole default task.</span></span> |
| <span data-ttu-id="886c3-177">detalhes da tarefa</span><span class="sxs-lookup"><span data-stu-id="886c3-177">task-details</span></span> | <span data-ttu-id="886c3-178">tarefa: um objeto de tarefa do planner</span><span class="sxs-lookup"><span data-stu-id="886c3-178">task: a planner task object</span></span> | <span data-ttu-id="886c3-179">template substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="886c3-179">template replaces the details section of the task.</span></span> |

<span data-ttu-id="886c3-180">O exemplo a seguir define um modelo para o componente de tarefas.</span><span class="sxs-lookup"><span data-stu-id="886c3-180">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="886c3-181">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="886c3-181">Microsoft Graph permissions</span></span>

<span data-ttu-id="886c3-182">Esse controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="886c3-182">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="886c3-183">Recurso</span><span class="sxs-lookup"><span data-stu-id="886c3-183">Resource</span></span> | <span data-ttu-id="886c3-184">Permissão</span><span class="sxs-lookup"><span data-stu-id="886c3-184">Permission</span></span> |
| - | - |
| <span data-ttu-id="886c3-185">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="886c3-185">/me/planner/plans</span></span> | <span data-ttu-id="886c3-186">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="886c3-186">Group.Read.All</span></span> |
| <span data-ttu-id="886c3-187">/planner/plans/${id}</span><span class="sxs-lookup"><span data-stu-id="886c3-187">/planner/plans/${id}</span></span> | <span data-ttu-id="886c3-188">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="886c3-188">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="886c3-189">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="886c3-189">/planner/tasks</span></span> | <span data-ttu-id="886c3-190">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="886c3-190">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="886c3-191">/groups/${group-id}/planner/plans</span><span class="sxs-lookup"><span data-stu-id="886c3-191">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="886c3-192">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="886c3-192">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="886c3-193">Para a fonte de dados do Microsoft Planner, buscar e ler tarefas requer a permissão Groups.Read.All.</span><span class="sxs-lookup"><span data-stu-id="886c3-193">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="886c3-194">Adicionar, atualizar ou remover tarefas requer a permissão Groups.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="886c3-194">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="886c3-195">Autenticação</span><span class="sxs-lookup"><span data-stu-id="886c3-195">Authentication</span></span>

<span data-ttu-id="886c3-196">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="886c3-196">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="886c3-197">Cache</span><span class="sxs-lookup"><span data-stu-id="886c3-197">Cache</span></span>

<span data-ttu-id="886c3-198">O `mgt-tasks` componente não armazena dados em cache.</span><span class="sxs-lookup"><span data-stu-id="886c3-198">The `mgt-tasks` component doesn't cache any data.</span></span>
