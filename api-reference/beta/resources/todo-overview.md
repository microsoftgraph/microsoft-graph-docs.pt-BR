---
title: Usar a API do Microsoft To Do
description: Você pode usar a API do Microsoft Graph para criar um aplicativo que se conecta com tarefas no Microsoft To Do.
author: avijityadav
localization_priority: Priority
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 76dc89caeb0a39d9dd0f40c1bcf046ffe9fe3f9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973514"
---
# <a name="use-the-microsoft-to-do-api"></a><span data-ttu-id="15798-103">Usar a API do Microsoft To Do</span><span class="sxs-lookup"><span data-stu-id="15798-103">Use the Microsoft To Do API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15798-104">Use a API To Do no Microsoft Graph para criar um aplicativo que se conecta com tarefas através do Microsoft To Do.</span><span class="sxs-lookup"><span data-stu-id="15798-104">Use the Microsoft Graph To Do API to create an app that connects with tasks across Microsoft To Do clients.</span></span> <span data-ttu-id="15798-105">Compilar uma variedade de experiências com tarefas, tais como as seguintes:</span><span class="sxs-lookup"><span data-stu-id="15798-105">Build a variety of experiences with tasks, such as the following:</span></span>

* <span data-ttu-id="15798-106">Crie tarefas a partir do fluxo de trabalho do seu aplicativo, por exemplo, por email ou notificações, e salve-as no To Do.</span><span class="sxs-lookup"><span data-stu-id="15798-106">Create tasks from your app’s workflow, for example, from email or notifications, and save them in To Do.</span></span> <span data-ttu-id="15798-107">Use a entidade [linkedResource](linkedresource.md) para armazenar o link de volta ao seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15798-107">Use the [linkedResource](linkedresource.md) entity to store the link back to your app.</span></span>
* <span data-ttu-id="15798-108">Sincronize as tarefas existentes de seu aplicativo com o To Do e crie uma única exibição de tarefa para melhor priorização e gerenciabilidade.</span><span class="sxs-lookup"><span data-stu-id="15798-108">Sync your app’s existing tasks with To Do and create a single task view for better prioritization and manageability.</span></span>
* <span data-ttu-id="15798-109">Gerenciar tarefas To Do em aplicações comerciais personalizadas.</span><span class="sxs-lookup"><span data-stu-id="15798-109">Manage To Do tasks in a custom business application.</span></span>

<span data-ttu-id="15798-110">Atualmente, a API suporta apenas as permissões delegadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="15798-110">Currently, the API supports only permissions delegated by the signed-in user.</span></span>
 
<span data-ttu-id="15798-111">Antes de começar com a API To Do, dê uma olhada nos recursos e como eles se relacionam entre si.</span><span class="sxs-lookup"><span data-stu-id="15798-111">Before starting with the To Do API, take a look at the resources and how they relate to one another.</span></span>

![Entidades da API To Do](/graph/images/todo-api-entities.png)

## <a name="task-list"></a><span data-ttu-id="15798-113">Lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="15798-113">Task list</span></span>

<span data-ttu-id="15798-114">O [todoTaskList](./todotasklist.md) representa um contêiner lógico dos recursos [todoTask](./todotask.md).</span><span class="sxs-lookup"><span data-stu-id="15798-114">A [todoTaskList](./todotasklist.md) represents a logical container of [todoTask](./todotask.md) resources.</span></span> <span data-ttu-id="15798-115">Atualmente, você só pode criar tarefas em uma lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="15798-115">You can currently create tasks only in a task list.</span></span> <span data-ttu-id="15798-116">Para [obter todas as suas listas de tarefas](../api/todotasklist-get.md), faça a seguinte solicitação HTTP:</span><span class="sxs-lookup"><span data-stu-id="15798-116">To [get all your task lists](../api/todotasklist-get.md), make the following HTTP request:</span></span>

``` http
GET /me/todo/lists
```

## <a name="task"></a><span data-ttu-id="15798-117">Tarefas</span><span class="sxs-lookup"><span data-stu-id="15798-117">Task</span></span>

<span data-ttu-id="15798-118">O [todoTask](./todotask.md) representa uma tarefa, ou seja, um trabalho ou um item pessoal que pode ser acompanhado e concluído.</span><span class="sxs-lookup"><span data-stu-id="15798-118">A [todoTask](./todotask.md) represents a task, i.e. a piece of work or personal item that can be tracked and completed.</span></span> <span data-ttu-id="15798-119">Para obter suas tarefas de uma lista de tarefas, faça a seguinte solicitação HTTP:</span><span class="sxs-lookup"><span data-stu-id="15798-119">To get your tasks from a task list, make the following HTTP request:</span></span>
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
```

## <a name="linked-resource"></a><span data-ttu-id="15798-120">Recurso vinculado</span><span class="sxs-lookup"><span data-stu-id="15798-120">Linked resource</span></span>

<span data-ttu-id="15798-121">O [linkedResource](linkedresource.md) representa qualquer item de um aplicativo de parceiro relacionado à tarefa, por exemplo, um item como o email de onde uma tarefa foi criada.</span><span class="sxs-lookup"><span data-stu-id="15798-121">A [linkedResource](linkedresource.md) represents any item from a partner application related to the task, e.g. an item like email from where a task was created.</span></span> <span data-ttu-id="15798-122">Você pode usá-la para armazenar informações e o link de volta para o item relacionado em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15798-122">You can use it to store information and the link back to the related item in your app.</span></span> <span data-ttu-id="15798-123">Para obter um recurso vinculado de uma tarefa, faça a seguinte solicitação HTTP:</span><span class="sxs-lookup"><span data-stu-id="15798-123">To get a linked resource from a task, make the following HTTP request:</span></span>
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/linkedresources/{linkedResourceId}
```

## <a name="track-changes-using-delta-query"></a><span data-ttu-id="15798-124">Acompanhar alterações usando a consulta delta</span><span class="sxs-lookup"><span data-stu-id="15798-124">Track changes using delta query</span></span>

<span data-ttu-id="15798-125">Por motivos de desempenho, talvez você queira manter um cache local de objetos e sincronizar periodicamente o cache local com o servidor, usando uma [consulta delta](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="15798-125">For performance reasons, you may want to maintain a local cache of objects, and periodically synchronize the local cache with the server, using [delta query](/graph/delta-query-overview).</span></span> 

<span data-ttu-id="15798-126">Os seguintes recursos da API To Do oferecem suporte à consulta delta:</span><span class="sxs-lookup"><span data-stu-id="15798-126">The following To Do API resources support delta query:</span></span>
* <span data-ttu-id="15798-127">Coleção [toTask](./todotask.md) em uma lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="15798-127">[todoTask](./todotask.md) collection in a task list</span></span>
* [<span data-ttu-id="15798-128">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="15798-128">todoTaskList</span></span>](./todotasklist.md)

## <a name="whats-new"></a><span data-ttu-id="15798-129">O que há de novo</span><span class="sxs-lookup"><span data-stu-id="15798-129">What's new</span></span>
<span data-ttu-id="15798-130">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="15798-130">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

