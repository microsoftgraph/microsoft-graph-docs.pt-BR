---
title: Visão geral da API do To Do
description: O To Do Oferece uma maneira simples de gerenciar suas tarefas e planejar o seu dia
author: avijityadav
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: f68aa1e4948fdac3ecaed94e75abe750f84db8f4
ms.sourcegitcommit: b6ca83070b6f015c09de215a82cf2b581181c33e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2020
ms.locfileid: "47367226"
---
# <a name="to-do-api-overview-preview"></a><span data-ttu-id="68540-103">Visão geral da API do To Do (visualização)</span><span class="sxs-lookup"><span data-stu-id="68540-103">To Do API overview (preview)</span></span>
<span data-ttu-id="68540-104">O Microsoft To-Do fornece uma maneira simples para as pessoas gerenciarem suas tarefas e planejarem seu dia.</span><span class="sxs-lookup"><span data-stu-id="68540-104">Microsoft To Do provides a simple way for people to manage their tasks and plan their day.</span></span> <span data-ttu-id="68540-105">As tarefas são organizadas em listas de tarefas, que podem ser acessadas através de clientes do To Do, Outlook e Teams a partir de qualquer dispositivo.</span><span class="sxs-lookup"><span data-stu-id="68540-105">Tasks are organized in task lists, which can be accessed across To Do clients, Outlook and Teams from any device.</span></span>

<span data-ttu-id="68540-106">**Aplicativo To Do para Windows**</span><span class="sxs-lookup"><span data-stu-id="68540-106">**To Do Windows app**</span></span>

<span data-ttu-id="68540-107">![Captura de tela de um aplicativo Microsoft To Do para Windows](./images/todo-windows-app.png "Imagem de um aplicativo Microsoft To Do para Windows")</span><span class="sxs-lookup"><span data-stu-id="68540-107">![Screenshot of a Microsoft To Do Windows App](./images/todo-windows-app.png "Image of Microsoft To Do Windows App")</span></span>

## <a name="why-integrate-with-to-do"></a><span data-ttu-id="68540-108">Vantagens da integração no To Do</span><span class="sxs-lookup"><span data-stu-id="68540-108">Why integrate with To Do?</span></span>

### <a name="ease-of-organizing-and-tracking-tasks"></a><span data-ttu-id="68540-109">Facilidade para organizar e acompanhar tarefas</span><span class="sxs-lookup"><span data-stu-id="68540-109">Ease of organizing and tracking tasks</span></span>
<span data-ttu-id="68540-110">O Microsoft To Do ajuda você a criar uma lista para qualquer coisa, desde tarefas de trabalho até projetos caseiros até compras em supermercado.</span><span class="sxs-lookup"><span data-stu-id="68540-110">Microsoft To Do helps you create a list for anything, from work assignments to home projects to groceries.</span></span> <span data-ttu-id="68540-111">Você pode acompanhar os prazos adicionando lembretes, datas de vencimento e anotações.</span><span class="sxs-lookup"><span data-stu-id="68540-111">You can keep track of deadlines by adding reminders, due dates, and notes.</span></span> <span data-ttu-id="68540-112">Você pode acessar suas listas de qualquer lugar com os aplicativos da Microsoft To-Do para iOS, Android, Mac, Windows e para a Web.</span><span class="sxs-lookup"><span data-stu-id="68540-112">You can access your lists from anywhere with the Microsoft To Do apps for iOS, Android, Mac, Windows, and the web.</span></span> 

### <a name="integrate-across-microsoft-365"></a><span data-ttu-id="68540-113">Integração através da Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="68540-113">Integrate across Microsoft 365</span></span>
<span data-ttu-id="68540-114">To Do é o único destino para tarefas pessoais no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="68540-114">To Do is the single destination for personal tasks in Microsoft 365.</span></span> <span data-ttu-id="68540-115">Portanto, está profundamente integrado aos hubs, da Microsoft 365, Outlook e Teams.</span><span class="sxs-lookup"><span data-stu-id="68540-115">So it’s deeply integrated with Microsoft 365 hubs, Outlook, and Teams.</span></span> <span data-ttu-id="68540-116">As tarefas criadas nesses produtos são sincronizadas com o To Do, para que você possa acessá-las e gerenciá-las através de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="68540-116">Tasks created in those products sync with To Do so you can access and manage them across devices.</span></span> <span data-ttu-id="68540-117">A integração do To Do pode ajudá-lo a alcançar milhões de usuários que usam o To Do para reunir tarefas do Outlook e do Teams em uma exibição integrada.</span><span class="sxs-lookup"><span data-stu-id="68540-117">To Do integration can help you reach millions of users who use To Do to gather tasks from Outlook and Teams into one integrated view.</span></span>  

### <a name="support-task-completion-using-linked-resources"></a><span data-ttu-id="68540-118">Dar suporte a conclusão de tarefas usando recursos vinculados</span><span class="sxs-lookup"><span data-stu-id="68540-118">Support task completion using linked resources</span></span>
<span data-ttu-id="68540-119">O Microsoft To Do fornece uma nova entidade chamada _linkedResource_, que você pode usar para criar tarefas que podem ser vinculadas de volta às suas fontes originais.</span><span class="sxs-lookup"><span data-stu-id="68540-119">Microsoft To Do provides a new entity called _linked resource_, which you can use to create tasks that can link back to their original sources.</span></span> <span data-ttu-id="68540-120">Você pode usar isto para integrar perfeitamente ao To Do em seu fluxo de trabalho, criando tarefas que são vinculadas ao seu produto ou serviço.</span><span class="sxs-lookup"><span data-stu-id="68540-120">You can use this to seamlessly integrate To Do in your workflow by creating tasks that link to your product or service.</span></span> 

## <a name="common-to-do-api-operations"></a><span data-ttu-id="68540-121">Operações comuns da API To Do.</span><span class="sxs-lookup"><span data-stu-id="68540-121">Common To Do API operations</span></span>

|<span data-ttu-id="68540-122">Operação</span><span class="sxs-lookup"><span data-stu-id="68540-122">Operation</span></span>|<span data-ttu-id="68540-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68540-123">Request</span></span>|
|:--------|:--|
| <span data-ttu-id="68540-124">Listar todas as listas de tarefas</span><span class="sxs-lookup"><span data-stu-id="68540-124">List all the task lists</span></span> | <span data-ttu-id="68540-125">GET https://graph.microsoft.com/beta/me/todo/lists</span><span class="sxs-lookup"><span data-stu-id="68540-125">GET https://graph.microsoft.com/beta/me/todo/lists</span></span> |
| <span data-ttu-id="68540-126">Lista de todas as tarefas em uma lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="68540-126">List all tasks in a task list</span></span> | <span data-ttu-id="68540-127">GET https://graph.microsoft.com/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="68540-127">GET https://graph.microsoft.com/me/todo/lists/{todoTaskListId}/tasks</span></span> |
| <span data-ttu-id="68540-128">Criar uma nova tarefa</span><span class="sxs-lookup"><span data-stu-id="68540-128">Create a new task</span></span> | <span data-ttu-id="68540-129">POST https://graph.microsoft.com/beta/me/todo/lists/{todoTaskListId}/tasks</span><span class="sxs-lookup"><span data-stu-id="68540-129">POST https://graph.microsoft.com/beta/me/todo/lists/{todoTaskListId}/tasks</span></span> |
| <span data-ttu-id="68540-130">Atualizar uma tarefa</span><span class="sxs-lookup"><span data-stu-id="68540-130">Update a task</span></span> | <span data-ttu-id="68540-131">PATCH https://graph.microsoft.com/beta/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span><span class="sxs-lookup"><span data-stu-id="68540-131">PATCH https://graph.microsoft.com/beta/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span></span> |
| <span data-ttu-id="68540-132">Excluir uma tarefa</span><span class="sxs-lookup"><span data-stu-id="68540-132">Delete a task</span></span> | <span data-ttu-id="68540-133">DELETE https://graph.microsoft.com/beta/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span><span class="sxs-lookup"><span data-stu-id="68540-133">DELETE https://graph.microsoft.com/beta/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}</span></span> |

## <a name="api-reference"></a><span data-ttu-id="68540-134">Referência da API</span><span class="sxs-lookup"><span data-stu-id="68540-134">API reference</span></span>
<span data-ttu-id="68540-135">Está procurando a referência de API para esse serviço?</span><span class="sxs-lookup"><span data-stu-id="68540-135">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="68540-136">API do To Do no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="68540-136">To Do API in Microsoft Graph</span></span>](/graph/api/resources/todo-overview?view=graph-rest-beta)
