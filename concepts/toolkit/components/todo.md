---
title: To Do componente no microsoft Graph Toolkit
description: O To Do componente permite ao usuário exibir, adicionar, remover, concluir ou editar todas as tarefas. Ele funciona com qualquer tarefa no Microsoft To-Do.
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 3eb91bc23f1159e08749b6e6b073939bacca0c5c
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780999"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="51e2e-104">To Do componente no microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="51e2e-104">To Do component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="51e2e-105">O componente To Do é usado para permitir que o usuário inscreveu para exibir, adicionar, remover, concluir e/ou editar tarefas do Microsoft To Do usando a API To Do no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="51e2e-105">The To Do component is used to enable the signed-in user to view, add, remove, complete, and/or edit tasks from Microsoft To Do using the To Do API in Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="51e2e-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51e2e-106">Example</span></span>

<span data-ttu-id="51e2e-107">O exemplo a seguir exibe as tarefas de Microsoft To Do do usuário Microsoft To Do usando o `mgt-todo` componente.</span><span class="sxs-lookup"><span data-stu-id="51e2e-107">The following example displays the signed-in user's Microsoft To Do tasks using the `mgt-todo` component.</span></span> <span data-ttu-id="51e2e-108">Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="51e2e-108">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="51e2e-109">Abra este exemplo em mgt.dev</span><span class="sxs-lookup"><span data-stu-id="51e2e-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="51e2e-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51e2e-110">Properties</span></span>

<span data-ttu-id="51e2e-111">Você pode usar os seguintes atributos e propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="51e2e-111">You can use the following attributes and properties to customize the component.</span></span>

| <span data-ttu-id="51e2e-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="51e2e-112">Attribute</span></span> | <span data-ttu-id="51e2e-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51e2e-113">Property</span></span> | <span data-ttu-id="51e2e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e2e-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="51e2e-115">somente leitura</span><span class="sxs-lookup"><span data-stu-id="51e2e-115">read-only</span></span> | <span data-ttu-id="51e2e-116">readOnly</span><span class="sxs-lookup"><span data-stu-id="51e2e-116">readOnly</span></span> | <span data-ttu-id="51e2e-117">Um Boolean para definir a interface da tarefa a ser lida somente (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="51e2e-117">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="51e2e-118">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-118">Default is `false`.</span></span> |
| <span data-ttu-id="51e2e-119">hide-header</span><span class="sxs-lookup"><span data-stu-id="51e2e-119">hide-header</span></span> | <span data-ttu-id="51e2e-120">hideHeader</span><span class="sxs-lookup"><span data-stu-id="51e2e-120">hideHeader</span></span> | <span data-ttu-id="51e2e-121">Um Boolean para mostrar ou ocultar o header do componente.</span><span class="sxs-lookup"><span data-stu-id="51e2e-121">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="51e2e-122">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-122">Default is `false`.</span></span> |
| <span data-ttu-id="51e2e-123">hide-options</span><span class="sxs-lookup"><span data-stu-id="51e2e-123">hide-options</span></span> | <span data-ttu-id="51e2e-124">hideOptions</span><span class="sxs-lookup"><span data-stu-id="51e2e-124">hideOptions</span></span> | <span data-ttu-id="51e2e-125">Um Boolean para mostrar ou ocultar as opções em tarefas.</span><span class="sxs-lookup"><span data-stu-id="51e2e-125">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="51e2e-126">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="51e2e-126">Default is `false`.</span></span>
| <span data-ttu-id="51e2e-127">initial-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="51e2e-127">initial-id="folder_id"</span></span> | <span data-ttu-id="51e2e-128">initialId</span><span class="sxs-lookup"><span data-stu-id="51e2e-128">initialId</span></span> | <span data-ttu-id="51e2e-129">Uma ID de cadeia de caracteres para definir a pasta inicialmente exibida como a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="51e2e-129">A string ID to set the initially displayed folder to the provided ID.</span></span> |
| <span data-ttu-id="51e2e-130">target-id="folder_id"</span><span class="sxs-lookup"><span data-stu-id="51e2e-130">target-id="folder_id"</span></span>| <span data-ttu-id="51e2e-131">targetId</span><span class="sxs-lookup"><span data-stu-id="51e2e-131">targetId</span></span> | <span data-ttu-id="51e2e-132">Uma ID de cadeia de caracteres para bloquear a interface de tarefas na ID da pasta fornecida.</span><span class="sxs-lookup"><span data-stu-id="51e2e-132">A string ID to lock the tasks interface to the provided folder ID.</span></span> |
| <span data-ttu-id="51e2e-133">N/A</span><span class="sxs-lookup"><span data-stu-id="51e2e-133">N/A</span></span> | <span data-ttu-id="51e2e-134">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="51e2e-134">isNewTaskVisible</span></span>  | <span data-ttu-id="51e2e-135">Determina se o novo exibição de tarefa está visível na renderização.</span><span class="sxs-lookup"><span data-stu-id="51e2e-135">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="51e2e-136">N/A</span><span class="sxs-lookup"><span data-stu-id="51e2e-136">N/A</span></span> | <span data-ttu-id="51e2e-137">taskFilter</span><span class="sxs-lookup"><span data-stu-id="51e2e-137">taskFilter</span></span>  | <span data-ttu-id="51e2e-138">Uma função opcional para filtrar quais tarefas são mostradas ao usuário.</span><span class="sxs-lookup"><span data-stu-id="51e2e-138">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="51e2e-139">O exemplo a seguir mostra apenas tarefas da pasta com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="51e2e-139">The following example shows only tasks from the folder with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a><span data-ttu-id="51e2e-140">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="51e2e-140">Custom CSS variables</span></span>

<span data-ttu-id="51e2e-141">O `mgt-todo` componente define as seguintes propriedades personalizadas CSS.</span><span class="sxs-lookup"><span data-stu-id="51e2e-141">The `mgt-todo` component defines the following CSS custom properties.</span></span>

````css
mgt-todo {
  --tasks-background-color
  --tasks-header-padding
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

  --task-margin
  --task-background
  --task-border
  --task-header-color
  --task-header-margin

  --task-new-margin
  --task-new-border
  --task-new-input-margin
  --task-new-input-padding
  --task-new-input-font-size
  --task-new-select-border

  --task-new-add-button-background
  --task-new-add-button-disabled-background
  --task-new-cancel-button-color

  --task-complete-background
  --task-complete-border

  --task-icon-alignment: flex-start (default) | center | flex-end
  --task-icon-background
  --task-icon-background-completed
  --task-icon-border
  --task-icon-border-completed
  --task-icon-border-radius
  --task-icon-color
  --task-icon-color-completed
}
````

<span data-ttu-id="51e2e-142">Para saber mais, confira [componentes de estilo](https://docs.microsoft.com/graph/toolkit/style.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-142">To learn more, see [styling components](https://docs.microsoft.com/graph/toolkit/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="51e2e-143">Eventos</span><span class="sxs-lookup"><span data-stu-id="51e2e-143">Events</span></span>

<span data-ttu-id="51e2e-144">Os eventos a seguir são disparados do componente.</span><span class="sxs-lookup"><span data-stu-id="51e2e-144">The following events are fired from the component.</span></span>

| <span data-ttu-id="51e2e-145">Evento</span><span class="sxs-lookup"><span data-stu-id="51e2e-145">Event</span></span> | <span data-ttu-id="51e2e-146">Detalhe</span><span class="sxs-lookup"><span data-stu-id="51e2e-146">Detail</span></span> | <span data-ttu-id="51e2e-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e2e-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="51e2e-148">taskAdded</span><span class="sxs-lookup"><span data-stu-id="51e2e-148">taskAdded</span></span> | <span data-ttu-id="51e2e-149">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="51e2e-149">The detail contains the respective `task` object</span></span> | <span data-ttu-id="51e2e-150">Dispara quando uma nova tarefa é criada.</span><span class="sxs-lookup"><span data-stu-id="51e2e-150">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="51e2e-151">taskChanged</span><span class="sxs-lookup"><span data-stu-id="51e2e-151">taskChanged</span></span> | <span data-ttu-id="51e2e-152">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="51e2e-152">The detail contains the respective `task` object</span></span> | <span data-ttu-id="51e2e-153">Dispara quando os metadados da tarefa foram alterados, como a marcação concluída.</span><span class="sxs-lookup"><span data-stu-id="51e2e-153">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="51e2e-154">taskClick</span><span class="sxs-lookup"><span data-stu-id="51e2e-154">taskClick</span></span> | <span data-ttu-id="51e2e-155">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="51e2e-155">The detail contains the respective `task` object</span></span> | <span data-ttu-id="51e2e-156">Dispara quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="51e2e-156">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="51e2e-157">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="51e2e-157">taskRemoved</span></span> | <span data-ttu-id="51e2e-158">O detalhe contém o objeto `task` respectivo</span><span class="sxs-lookup"><span data-stu-id="51e2e-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="51e2e-159">Dispara quando uma tarefa existente foi excluída.</span><span class="sxs-lookup"><span data-stu-id="51e2e-159">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="51e2e-160">Modelos</span><span class="sxs-lookup"><span data-stu-id="51e2e-160">Templates</span></span>

<span data-ttu-id="51e2e-161">O `tasks` componente dá suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="51e2e-161">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="51e2e-162">Para especificar um modelo, inclua um elemento dentro de um componente e de definir o `<template>` valor como um dos `data-type` seguintes.</span><span class="sxs-lookup"><span data-stu-id="51e2e-162">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="51e2e-163">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="51e2e-163">Data type</span></span>     | <span data-ttu-id="51e2e-164">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="51e2e-164">Data context</span></span>              | <span data-ttu-id="51e2e-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e2e-165">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="51e2e-166">tarefa</span><span class="sxs-lookup"><span data-stu-id="51e2e-166">task</span></span>     | <span data-ttu-id="51e2e-167">tarefa: um objeto de tarefa a ser usado</span><span class="sxs-lookup"><span data-stu-id="51e2e-167">task: a to-do task object</span></span> | <span data-ttu-id="51e2e-168">Substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="51e2e-168">Replaces the whole default task.</span></span> |
| <span data-ttu-id="51e2e-169">detalhes da tarefa</span><span class="sxs-lookup"><span data-stu-id="51e2e-169">task-details</span></span> | <span data-ttu-id="51e2e-170">tarefa: um objeto de tarefa a ser usado</span><span class="sxs-lookup"><span data-stu-id="51e2e-170">task: a to-do task object</span></span> | <span data-ttu-id="51e2e-171">O modelo substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="51e2e-171">Template replaces the details section of the task.</span></span> |

<span data-ttu-id="51e2e-172">O exemplo a seguir define um modelo para o componente de tarefas.</span><span class="sxs-lookup"><span data-stu-id="51e2e-172">The following example defines a template for the tasks component.</span></span>

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="51e2e-173">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="51e2e-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="51e2e-174">Esse controle usa as seguintes APIs Graph Microsoft e permissões.</span><span class="sxs-lookup"><span data-stu-id="51e2e-174">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="51e2e-175">Configuração</span><span class="sxs-lookup"><span data-stu-id="51e2e-175">Configuration</span></span> | <span data-ttu-id="51e2e-176">Permissão</span><span class="sxs-lookup"><span data-stu-id="51e2e-176">Permission</span></span> | <span data-ttu-id="51e2e-177">API</span><span class="sxs-lookup"><span data-stu-id="51e2e-177">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="51e2e-178">`targetId` set</span><span class="sxs-lookup"><span data-stu-id="51e2e-178">`targetId` set</span></span> | <span data-ttu-id="51e2e-179">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="51e2e-179">Tasks.Read</span></span> | <span data-ttu-id="51e2e-180">[/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span><span class="sxs-lookup"><span data-stu-id="51e2e-180">[/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span></span> |
| <span data-ttu-id="51e2e-181">`targetId` não definido</span><span class="sxs-lookup"><span data-stu-id="51e2e-181">`targetId` not set</span></span> | <span data-ttu-id="51e2e-182">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="51e2e-182">Tasks.Read</span></span> | <span data-ttu-id="51e2e-183">[/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span><span class="sxs-lookup"><span data-stu-id="51e2e-183">[/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks)</span></span> |
| <span data-ttu-id="51e2e-184">criar, atualizar ou excluir tarefa</span><span class="sxs-lookup"><span data-stu-id="51e2e-184">create, update or delete task</span></span> | <span data-ttu-id="51e2e-185">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e2e-185">Tasks.ReadWrite</span></span> | [<span data-ttu-id="51e2e-186">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span><span class="sxs-lookup"><span data-stu-id="51e2e-186">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span></span>](/graph/api/todotask-get) |

## <a name="authentication"></a><span data-ttu-id="51e2e-187">Autenticação</span><span class="sxs-lookup"><span data-stu-id="51e2e-187">Authentication</span></span>

<span data-ttu-id="51e2e-188">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="51e2e-188">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="51e2e-189">Cache</span><span class="sxs-lookup"><span data-stu-id="51e2e-189">Cache</span></span>

<span data-ttu-id="51e2e-190">O `mgt-todo` componente não armazena dados em cache.</span><span class="sxs-lookup"><span data-stu-id="51e2e-190">The `mgt-todo` component doesn't cache any data.</span></span>
