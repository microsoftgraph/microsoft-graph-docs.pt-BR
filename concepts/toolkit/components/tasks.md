---
title: Componente tarefas no Microsoft Graph Toolkit
description: O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas. Ele funciona com qualquer tarefa no Microsoft Planner ou no Microsoft to-do.
localization_priority: Normal
author: benotter
ms.openlocfilehash: f8366842be9319e8c89d05fa23bc488cde49359a
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275819"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="94f39-104">Componente tarefas no Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="94f39-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="94f39-105">O componente tarefas permite que o usuário exiba, adicione, remova, conclua ou edite tarefas.</span><span class="sxs-lookup"><span data-stu-id="94f39-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="94f39-106">Ele funciona com tarefas no Microsoft Planner ou Microsoft to-do.</span><span class="sxs-lookup"><span data-stu-id="94f39-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>

## <a name="example"></a><span data-ttu-id="94f39-107">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94f39-107">Example</span></span>

[<span data-ttu-id="94f39-108">exemplo de jsfiddle</span><span class="sxs-lookup"><span data-stu-id="94f39-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="94f39-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94f39-109">Properties</span></span>

| <span data-ttu-id="94f39-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94f39-110">Property</span></span> | <span data-ttu-id="94f39-111">Atributo</span><span class="sxs-lookup"><span data-stu-id="94f39-111">Attribute</span></span> | <span data-ttu-id="94f39-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="94f39-112">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="94f39-113">dataSource</span><span class="sxs-lookup"><span data-stu-id="94f39-113">dataSource</span></span> | <span data-ttu-id="94f39-114">Data-Source = "todo/planejador"</span><span class="sxs-lookup"><span data-stu-id="94f39-114">data-source="todo/planner"</span></span> | <span data-ttu-id="94f39-115">Uma enumeração para configurar a fonte de dados para tarefas-Microsoft to-do ou Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="94f39-115">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="94f39-116">O padrão é `planner`.</span><span class="sxs-lookup"><span data-stu-id="94f39-116">Default is `planner`.</span></span> |
| <span data-ttu-id="94f39-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="94f39-117">readOnly</span></span> | <span data-ttu-id="94f39-118">somente leitura</span><span class="sxs-lookup"><span data-stu-id="94f39-118">read-only</span></span> | <span data-ttu-id="94f39-119">Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas).</span><span class="sxs-lookup"><span data-stu-id="94f39-119">A boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="94f39-120">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="94f39-120">Default is `false`.</span></span> |
| <span data-ttu-id="94f39-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="94f39-121">hideHeader</span></span> | <span data-ttu-id="94f39-122">Ocultar-cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94f39-122">hide-header</span></span> | <span data-ttu-id="94f39-123">Um booliano para mostrar ou ocultar o cabeçalho do componente.</span><span class="sxs-lookup"><span data-stu-id="94f39-123">A boolean to show or hide the header of the component.</span></span> <span data-ttu-id="94f39-124">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="94f39-124">Default is `false`.</span></span> |
| <span data-ttu-id="94f39-125">initialid</span><span class="sxs-lookup"><span data-stu-id="94f39-125">initialId</span></span> | <span data-ttu-id="94f39-126">Initial-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="94f39-126">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="94f39-127">Uma ID de cadeia de caracteres para definir o planejador ou pasta inicialmente exibido para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="94f39-127">A string id to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="94f39-128">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="94f39-128">initialBucketId</span></span> | <span data-ttu-id="94f39-129">Initial-Bucket-ID = "BUCKET_ID"</span><span class="sxs-lookup"><span data-stu-id="94f39-129">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="94f39-130">Uma ID de cadeia de caracteres para definir o Bucket exibido inicialmente (somente a fonte de dados do Planner) para a ID fornecida.</span><span class="sxs-lookup"><span data-stu-id="94f39-130">A string id to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="94f39-131">targetId</span><span class="sxs-lookup"><span data-stu-id="94f39-131">targetId</span></span> | <span data-ttu-id="94f39-132">Target-ID = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="94f39-132">target-id="planner_id/folder_id"</span></span> | <span data-ttu-id="94f39-133">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para o planejador ou ID de pasta fornecido.</span><span class="sxs-lookup"><span data-stu-id="94f39-133">A string id to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="94f39-134">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="94f39-134">targetBucketId</span></span> | <span data-ttu-id="94f39-135">Target-Bucket-ID = "BUCKET_ID"</span><span class="sxs-lookup"><span data-stu-id="94f39-135">target-bucket-id="bucket_id"</span></span> | <span data-ttu-id="94f39-136">Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de Bucket fornecida (somente a fonte de dados do Planner).</span><span class="sxs-lookup"><span data-stu-id="94f39-136">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |

<span data-ttu-id="94f39-137">Apresentamos um exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="94f39-137">The following is an example.</span></span>

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a><span data-ttu-id="94f39-138">Variáveis CSS personalizadas</span><span class="sxs-lookup"><span data-stu-id="94f39-138">Custom CSS variables</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="94f39-139">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="94f39-139">Microsoft Graph permissions</span></span>

<span data-ttu-id="94f39-140">Este controle usa as seguintes APIs e permissões do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="94f39-140">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="94f39-141">Resource</span><span class="sxs-lookup"><span data-stu-id="94f39-141">Resource</span></span> | <span data-ttu-id="94f39-142">Permissão</span><span class="sxs-lookup"><span data-stu-id="94f39-142">Permission</span></span> |
| - | - |
| <span data-ttu-id="94f39-143">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="94f39-143">/me/planner/plans</span></span> | <span data-ttu-id="94f39-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="94f39-144">Group.Read.All</span></span> |
| <span data-ttu-id="94f39-145">/Planner/Plans/$ {ID}</span><span class="sxs-lookup"><span data-stu-id="94f39-145">/planner/plans/${id}</span></span> | <span data-ttu-id="94f39-146">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f39-146">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="94f39-147">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="94f39-147">/planner/tasks</span></span> | <span data-ttu-id="94f39-148">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f39-148">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="94f39-149">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="94f39-149">/me/outlook/taskGroups</span></span> | <span data-ttu-id="94f39-150">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="94f39-150">Tasks.Read</span></span> |
| <span data-ttu-id="94f39-151">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="94f39-151">/me/outlook/taskFolders</span></span> | <span data-ttu-id="94f39-152">Tarefas. Read, Tasks. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94f39-152">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="94f39-153">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="94f39-153">/me/outlook/tasks</span></span> | <span data-ttu-id="94f39-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94f39-154">Tasks.ReadWrite</span></span> |

<span data-ttu-id="94f39-155">Para a fonte de dados do Microsoft Planner, as tarefas de busca e leitura exigem a permissão groups. Read. All.</span><span class="sxs-lookup"><span data-stu-id="94f39-155">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="94f39-156">Adicionar, atualizar ou remover tarefas requer a permissão groups. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="94f39-156">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="94f39-157">Para a fonte de dados do Microsoft todo, a permissão Tasks. Read é necessária para buscar e ler tarefas.</span><span class="sxs-lookup"><span data-stu-id="94f39-157">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="94f39-158">Adicionar, atualizar ou remover tarefas requer a permissão Tasks. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="94f39-158">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="94f39-159">Autenticação</span><span class="sxs-lookup"><span data-stu-id="94f39-159">Authentication</span></span>

<span data-ttu-id="94f39-160">O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="94f39-160">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
