---
title: Componente tarefas pendentes no Microsoft Graph Toolkit
description: O componente tarefas pendentes permite ao usuário exibir, adicionar, remover, concluir ou editar tarefas pendentes. Ele funciona com qualquer tarefa no Microsoft to-do.
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 1a00d045da55dc14da47770b0e56522590f4b5bc
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659159"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f5990-104">Componente tarefas pendentes no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="f5990-104">To Do component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f5990-105">O componente tarefas pendentes é usado para permitir que o usuário conectado exiba, adicione, remova, conclua e/ou edite tarefas da Microsoft para usar a API tarefas pendentes no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f5990-105">The To Do component is used to enable the signed-in user to view, add, remove, complete, and/or edit tasks from Microsoft To Do using the To Do API in Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="f5990-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5990-106">Example</span></span>

<span data-ttu-id="f5990-107">O exemplo a seguir exibe as tarefas do usuário conectado da Microsoft usando o `mgt-todo` componente.</span><span class="sxs-lookup"><span data-stu-id="f5990-107">The following example displays the signed-in user's Microsoft To Do tasks using the `mgt-todo` component.</span></span> <span data-ttu-id="f5990-108">Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.</span><span class="sxs-lookup"><span data-stu-id="f5990-108">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="f5990-109">Abra este exemplo em gerenciamento de. dev</span><span class="sxs-lookup"><span data-stu-id="f5990-109">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="f5990-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5990-110">Properties</span></span>

<span data-ttu-id="f5990-111">Você pode usar os seguintes atributos e propriedades para personalizar o componente.</span><span class="sxs-lookup"><span data-stu-id="f5990-111">You can use the following attributes and properties to customize the component.</span></span>

| <span data-ttu-id="f5990-112">Atributo</span><span class="sxs-lookup"><span data-stu-id="f5990-112">Attribute</span></span> | <span data-ttu-id="f5990-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5990-113">Property</span></span> | <span data-ttu-id="f5990-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5990-114">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="f5990-115">somente leitura</span><span class="sxs-lookup"><span data-stu-id="f5990-115">read-only</span></span> | <span data-ttu-id="f5990-116">readOnly</span><span class="sxs-lookup"><span data-stu-id="f5990-116">readOnly</span></span> | <span data-ttu-id="f5990-117">Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="f5990-117">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="f5990-118">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="f5990-118">Default is `false`.</span></span> |
| <span data-ttu-id="f5990-119">Ocultar-cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5990-119">hide-header</span></span> | <span data-ttu-id="f5990-120">hideHeader</span><span class="sxs-lookup"><span data-stu-id="f5990-120">hideHeader</span></span> | <span data-ttu-id="f5990-121">Um booliano para mostrar ou ocultar o cabeçalho do componente.</span><span class="sxs-lookup"><span data-stu-id="f5990-121">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="f5990-122">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="f5990-122">Default is `false`.</span></span> |
| <span data-ttu-id="f5990-123">Hide-opções</span><span class="sxs-lookup"><span data-stu-id="f5990-123">hide-options</span></span> | <span data-ttu-id="f5990-124">hideoptions</span><span class="sxs-lookup"><span data-stu-id="f5990-124">hideOptions</span></span> | <span data-ttu-id="f5990-125">Um booliano para mostrar ou ocultar as opções nas tarefas.</span><span class="sxs-lookup"><span data-stu-id="f5990-125">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="f5990-126">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="f5990-126">Default is `false`.</span></span>
| <span data-ttu-id="f5990-127">Initial-ID = "folder_id"</span><span class="sxs-lookup"><span data-stu-id="f5990-127">initial-id="folder_id"</span></span> | <span data-ttu-id="f5990-128">initialid</span><span class="sxs-lookup"><span data-stu-id="f5990-128">initialId</span></span> | <span data-ttu-id="f5990-129">Uma ID de cadeia de caracteres para definir a pasta exibida inicialmente com a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="f5990-129">A string ID to set the initially displayed folder to the provided ID.</span></span> |
| <span data-ttu-id="f5990-130">Target-ID = "folder_id"</span><span class="sxs-lookup"><span data-stu-id="f5990-130">target-id="folder_id"</span></span>| <span data-ttu-id="f5990-131">targetId</span><span class="sxs-lookup"><span data-stu-id="f5990-131">targetId</span></span> | <span data-ttu-id="f5990-132">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de pasta fornecida.</span><span class="sxs-lookup"><span data-stu-id="f5990-132">A string ID to lock the tasks interface to the provided folder ID.</span></span> |
| <span data-ttu-id="f5990-133">N/D</span><span class="sxs-lookup"><span data-stu-id="f5990-133">N/A</span></span> | <span data-ttu-id="f5990-134">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="f5990-134">isNewTaskVisible</span></span>  | <span data-ttu-id="f5990-135">Determina se a exibição de nova tarefa é visível no processamento.</span><span class="sxs-lookup"><span data-stu-id="f5990-135">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="f5990-136">N/D</span><span class="sxs-lookup"><span data-stu-id="f5990-136">N/A</span></span> | <span data-ttu-id="f5990-137">taskFilter</span><span class="sxs-lookup"><span data-stu-id="f5990-137">taskFilter</span></span>  | <span data-ttu-id="f5990-138">Uma função opcional para filtrar quais tarefas são exibidas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="f5990-138">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="f5990-139">O exemplo a seguir mostra apenas as tarefas da pasta com a ID *12345* e não permite que o usuário crie novas tarefas.</span><span class="sxs-lookup"><span data-stu-id="f5990-139">The following example shows only tasks from the folder with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a><span data-ttu-id="f5990-140">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="f5990-140">Custom CSS variables</span></span>

<span data-ttu-id="f5990-141">O `mgt-todo` componente define as seguintes propriedades personalizadas de CSS.</span><span class="sxs-lookup"><span data-stu-id="f5990-141">The `mgt-todo` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="f5990-142">Para saber mais, confira [estilos de componentes](https://docs.microsoft.com/graph/toolkit/style.md).</span><span class="sxs-lookup"><span data-stu-id="f5990-142">To learn more, see [styling components](https://docs.microsoft.com/graph/toolkit/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="f5990-143">Eventos</span><span class="sxs-lookup"><span data-stu-id="f5990-143">Events</span></span>

<span data-ttu-id="f5990-144">Os eventos a seguir são acionados do componente.</span><span class="sxs-lookup"><span data-stu-id="f5990-144">The following events are fired from the component.</span></span>

| <span data-ttu-id="f5990-145">Evento</span><span class="sxs-lookup"><span data-stu-id="f5990-145">Event</span></span> | <span data-ttu-id="f5990-146">Detalhe</span><span class="sxs-lookup"><span data-stu-id="f5990-146">Detail</span></span> | <span data-ttu-id="f5990-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5990-147">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f5990-148">taskAdded</span><span class="sxs-lookup"><span data-stu-id="f5990-148">taskAdded</span></span> | <span data-ttu-id="f5990-149">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="f5990-149">The detail contains the respective `task` object</span></span> | <span data-ttu-id="f5990-150">Dispara quando uma nova tarefa é criada.</span><span class="sxs-lookup"><span data-stu-id="f5990-150">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="f5990-151">taskchanged</span><span class="sxs-lookup"><span data-stu-id="f5990-151">taskChanged</span></span> | <span data-ttu-id="f5990-152">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="f5990-152">The detail contains the respective `task` object</span></span> | <span data-ttu-id="f5990-153">Dispara quando os metadados da tarefa são alterados, como marcação concluída.</span><span class="sxs-lookup"><span data-stu-id="f5990-153">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="f5990-154">taskClick</span><span class="sxs-lookup"><span data-stu-id="f5990-154">taskClick</span></span> | <span data-ttu-id="f5990-155">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="f5990-155">The detail contains the respective `task` object</span></span> | <span data-ttu-id="f5990-156">Dispara quando o usuário clica ou toca em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f5990-156">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="f5990-157">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="f5990-157">taskRemoved</span></span> | <span data-ttu-id="f5990-158">O detalhe contém o respectivo `task` objeto</span><span class="sxs-lookup"><span data-stu-id="f5990-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="f5990-159">Dispara quando uma tarefa existente foi excluída.</span><span class="sxs-lookup"><span data-stu-id="f5990-159">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="f5990-160">Modelos</span><span class="sxs-lookup"><span data-stu-id="f5990-160">Templates</span></span>

<span data-ttu-id="f5990-161">O `tasks` componente oferece suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente.</span><span class="sxs-lookup"><span data-stu-id="f5990-161">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="f5990-162">Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.</span><span class="sxs-lookup"><span data-stu-id="f5990-162">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="f5990-163">Tipo de dados</span><span class="sxs-lookup"><span data-stu-id="f5990-163">Data type</span></span>     | <span data-ttu-id="f5990-164">Contexto de dados</span><span class="sxs-lookup"><span data-stu-id="f5990-164">Data context</span></span>              | <span data-ttu-id="f5990-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5990-165">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="f5990-166">tarefa</span><span class="sxs-lookup"><span data-stu-id="f5990-166">task</span></span>     | <span data-ttu-id="f5990-167">tarefa: um objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="f5990-167">task: a to-do task object</span></span> | <span data-ttu-id="f5990-168">Substitui toda a tarefa padrão.</span><span class="sxs-lookup"><span data-stu-id="f5990-168">Replaces the whole default task.</span></span> |
| <span data-ttu-id="f5990-169">tarefa-detalhes</span><span class="sxs-lookup"><span data-stu-id="f5990-169">task-details</span></span> | <span data-ttu-id="f5990-170">tarefa: um objeto de tarefa tarefas pendentes</span><span class="sxs-lookup"><span data-stu-id="f5990-170">task: a to-do task object</span></span> | <span data-ttu-id="f5990-171">O modelo substitui a seção de detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="f5990-171">Template replaces the details section of the task.</span></span> |

<span data-ttu-id="f5990-172">O exemplo a seguir define um modelo para o componente tarefas.</span><span class="sxs-lookup"><span data-stu-id="f5990-172">The following example defines a template for the tasks component.</span></span>

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f5990-173">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f5990-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="f5990-174">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f5990-174">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="f5990-175">Recurso</span><span class="sxs-lookup"><span data-stu-id="f5990-175">Resource</span></span> | <span data-ttu-id="f5990-176">Permissão</span><span class="sxs-lookup"><span data-stu-id="f5990-176">Permission</span></span> |
| - | - |
| [<span data-ttu-id="f5990-177">/me/todo/lists/</span><span class="sxs-lookup"><span data-stu-id="f5990-177">/me/todo/lists/</span></span>](/graph/api/todo-list-lists) | <span data-ttu-id="f5990-178">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5990-178">Tasks.ReadWrite</span></span> |
| [<span data-ttu-id="f5990-179">/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="f5990-179">/me/todo/lists/{todoTaskListId}/tasks</span></span>](/graph/api/todotasklist-list-tasks) | <span data-ttu-id="f5990-180">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5990-180">Tasks.ReadWrite</span></span> |
| [<span data-ttu-id="f5990-181">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span><span class="sxs-lookup"><span data-stu-id="f5990-181">/me/todo/lists/{todoTaskListId}/tasks/{taskId}</span></span>](/graph/api/todotask-get) | <span data-ttu-id="f5990-182">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5990-182">Tasks.ReadWrite</span></span> |

## <a name="authentication"></a><span data-ttu-id="f5990-183">Autenticação</span><span class="sxs-lookup"><span data-stu-id="f5990-183">Authentication</span></span>

<span data-ttu-id="f5990-184">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="f5990-184">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>
