---
title: Componente tarefas no Microsoft Graph Toolkit
description: O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com qualquer tarefa no Microsoft Planner.
localization_priority: Normal
author: benotter
ms.openlocfilehash: 5364491caae4edc9cd3f022937bcd6d809aa924f
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659211"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="4c5ed-104">Componente tarefas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="4c5ed-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="4c5ed-105">O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas do Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks from Microsoft Planner.</span></span>  

<span data-ttu-id="4c5ed-106">Além disso, um usuário pode atribuir um único ou vários usuários do Microsoft Graph a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-106">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="4c5ed-107">Para obter mais detalhes sobre as atribuições do Microsoft Graph, consulte [plannerAssignments](/graph/api/resources/plannerassignments).</span><span class="sxs-lookup"><span data-stu-id="4c5ed-107">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments).</span></span>

## <a name="example"></a><span data-ttu-id="4c5ed-108">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c5ed-108">Example</span></span>

<span data-ttu-id="4c5ed-109">O exemplo a seguir exibe as tarefas do Microsoft Planner do usuário conectado usando o `mgt-tasks` componente.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-109">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="4c5ed-110">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="4c5ed-111">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="4c5ed-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="4c5ed-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c5ed-112">Properties</span></span>

| <span data-ttu-id="4c5ed-113">Atributo</span><span class="sxs-lookup"><span data-stu-id="4c5ed-113">Attribute</span></span> | <span data-ttu-id="4c5ed-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c5ed-114">Property</span></span> | <span data-ttu-id="4c5ed-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c5ed-115">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="4c5ed-116">somente leitura</span><span class="sxs-lookup"><span data-stu-id="4c5ed-116">read-only</span></span> | <span data-ttu-id="4c5ed-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="4c5ed-117">readOnly</span></span> | <span data-ttu-id="4c5ed-118">Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="4c5ed-118">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="4c5ed-119">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-119">Default is `false`.</span></span> |
| <span data-ttu-id="4c5ed-120">Ocultar-cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c5ed-120">hide-header</span></span> | <span data-ttu-id="4c5ed-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="4c5ed-121">hideHeader</span></span> | <span data-ttu-id="4c5ed-122">Um booliano para mostrar ou ocultar o cabeçalho do componente.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-122">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="4c5ed-123">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-123">Default is `false`.</span></span> |
| <span data-ttu-id="4c5ed-124">Hide-opções</span><span class="sxs-lookup"><span data-stu-id="4c5ed-124">hide-options</span></span> | <span data-ttu-id="4c5ed-125">hideoptions</span><span class="sxs-lookup"><span data-stu-id="4c5ed-125">hideOptions</span></span> | <span data-ttu-id="4c5ed-126">Um booliano para mostrar ou ocultar as opções nas tarefas.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-126">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="4c5ed-127">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-127">Default is `false`.</span></span>
| <span data-ttu-id="4c5ed-128">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="4c5ed-128">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="4c5ed-129">initialid</span><span class="sxs-lookup"><span data-stu-id="4c5ed-129">initialId</span></span> | <span data-ttu-id="4c5ed-130">Uma ID de cadeia de caracteres para definir o planejador ou pasta inicialmente exibido para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-130">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="4c5ed-131">Initial-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="4c5ed-131">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="4c5ed-132">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="4c5ed-132">initialBucketId</span></span> | <span data-ttu-id="4c5ed-133">Uma ID de cadeia de caracteres para definir o Bucket exibido inicialmente (planejador Data-Source somente) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="4c5ed-134">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="4c5ed-134">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="4c5ed-135">targetId</span><span class="sxs-lookup"><span data-stu-id="4c5ed-135">targetId</span></span> | <span data-ttu-id="4c5ed-136">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou ID de pasta fornecido.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-136">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="4c5ed-137">Target-Bucket-ID = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="4c5ed-137">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="4c5ed-138">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="4c5ed-138">targetBucketId</span></span>  | <span data-ttu-id="4c5ed-139">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de Bucket fornecida (somente planejador Data-Source).</span><span class="sxs-lookup"><span data-stu-id="4c5ed-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="4c5ed-140">ID de grupo</span><span class="sxs-lookup"><span data-stu-id="4c5ed-140">group-id</span></span> | <span data-ttu-id="4c5ed-141">groupId</span><span class="sxs-lookup"><span data-stu-id="4c5ed-141">groupId</span></span>  | <span data-ttu-id="4c5ed-142">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-142">A string ID to lock the tasks interface to the group ID.</span></span> |
| <span data-ttu-id="4c5ed-143">N/D</span><span class="sxs-lookup"><span data-stu-id="4c5ed-143">N/A</span></span> | <span data-ttu-id="4c5ed-144">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="4c5ed-144">isNewTaskVisible</span></span>  | <span data-ttu-id="4c5ed-145">Determina se a exibição de nova tarefa é visível no processamento.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-145">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="4c5ed-146">N/D</span><span class="sxs-lookup"><span data-stu-id="4c5ed-146">N/A</span></span> | <span data-ttu-id="4c5ed-147">taskFilter</span><span class="sxs-lookup"><span data-stu-id="4c5ed-147">taskFilter</span></span>  | <span data-ttu-id="4c5ed-148">Uma função opcional para filtrar quais tarefas são exibidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-148">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="4c5ed-149">O exemplo a seguir mostra apenas as tarefas do Planner com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-149">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="4c5ed-150">O exemplo a seguir mostra como filtrar tarefas que têm apenas *category3* definido.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-150">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="4c5ed-151">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="4c5ed-151">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="4c5ed-152">Eventos</span><span class="sxs-lookup"><span data-stu-id="4c5ed-152">Events</span></span>
| <span data-ttu-id="4c5ed-153">Evento</span><span class="sxs-lookup"><span data-stu-id="4c5ed-153">Event</span></span> | <span data-ttu-id="4c5ed-154">Detalhe</span><span class="sxs-lookup"><span data-stu-id="4c5ed-154">Detail</span></span> | <span data-ttu-id="4c5ed-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c5ed-155">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="4c5ed-156">taskAdded</span><span class="sxs-lookup"><span data-stu-id="4c5ed-156">taskAdded</span></span> | <span data-ttu-id="4c5ed-157">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="4c5ed-157">The detail contains the respective `task` object</span></span> | <span data-ttu-id="4c5ed-158">Dispara quando uma nova tarefa é criada.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-158">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="4c5ed-159">taskchanged</span><span class="sxs-lookup"><span data-stu-id="4c5ed-159">taskChanged</span></span> | <span data-ttu-id="4c5ed-160">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="4c5ed-160">The detail contains the respective `task` object</span></span> | <span data-ttu-id="4c5ed-161">Dispara quando os metadados da tarefa são alterados, como marcação concluída.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-161">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="4c5ed-162">taskClick</span><span class="sxs-lookup"><span data-stu-id="4c5ed-162">taskClick</span></span> | <span data-ttu-id="4c5ed-163">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="4c5ed-163">The detail contains the respective `task` object</span></span> | <span data-ttu-id="4c5ed-164">Dispara quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-164">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="4c5ed-165">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="4c5ed-165">taskRemoved</span></span> | <span data-ttu-id="4c5ed-166">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="4c5ed-166">The detail contains the respective `task` object</span></span> | <span data-ttu-id="4c5ed-167">Dispara quando uma tarefa existente foi excluída.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-167">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="4c5ed-168">Modelos</span><span class="sxs-lookup"><span data-stu-id="4c5ed-168">Templates</span></span>

<span data-ttu-id="4c5ed-169">O `tasks` componente oferece suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-169">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="4c5ed-170">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="4c5ed-170">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="4c5ed-171">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="4c5ed-171">Data type</span></span>     | <span data-ttu-id="4c5ed-172">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="4c5ed-172">Data context</span></span>              | <span data-ttu-id="4c5ed-173">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c5ed-173">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="4c5ed-174">tarefa</span><span class="sxs-lookup"><span data-stu-id="4c5ed-174">task</span></span>     | <span data-ttu-id="4c5ed-175">tarefa: um objeto de tarefa do Planner</span><span class="sxs-lookup"><span data-stu-id="4c5ed-175">task: a planner task object</span></span> | <span data-ttu-id="4c5ed-176">Substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-176">replaces the whole default task.</span></span> |
| <span data-ttu-id="4c5ed-177">tarefa-detalhes</span><span class="sxs-lookup"><span data-stu-id="4c5ed-177">task-details</span></span> | <span data-ttu-id="4c5ed-178">tarefa: um objeto de tarefa do Planner</span><span class="sxs-lookup"><span data-stu-id="4c5ed-178">task: a planner task object</span></span> | <span data-ttu-id="4c5ed-179">o modelo substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-179">template replaces the details section of the task.</span></span> |

<span data-ttu-id="4c5ed-180">O exemplo a seguir define um modelo para o componente tarefas.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-180">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="4c5ed-181">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4c5ed-181">Microsoft Graph permissions</span></span>

<span data-ttu-id="4c5ed-182">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-182">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="4c5ed-183">Recurso</span><span class="sxs-lookup"><span data-stu-id="4c5ed-183">Resource</span></span> | <span data-ttu-id="4c5ed-184">Permissão</span><span class="sxs-lookup"><span data-stu-id="4c5ed-184">Permission</span></span> |
| - | - |
| <span data-ttu-id="4c5ed-185">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="4c5ed-185">/me/planner/plans</span></span> | <span data-ttu-id="4c5ed-186">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c5ed-186">Group.Read.All</span></span> |
| <span data-ttu-id="4c5ed-187">/Planner/Plans/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="4c5ed-187">/planner/plans/${id}</span></span> | <span data-ttu-id="4c5ed-188">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c5ed-188">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4c5ed-189">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="4c5ed-189">/planner/tasks</span></span> | <span data-ttu-id="4c5ed-190">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c5ed-190">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4c5ed-191">/groups/$ {Group-ID}/Planner/Plans</span><span class="sxs-lookup"><span data-stu-id="4c5ed-191">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="4c5ed-192">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c5ed-192">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="4c5ed-193">Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-193">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="4c5ed-194">Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="4c5ed-194">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="4c5ed-195">Autenticação</span><span class="sxs-lookup"><span data-stu-id="4c5ed-195">Authentication</span></span>

<span data-ttu-id="4c5ed-196">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="4c5ed-196">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>