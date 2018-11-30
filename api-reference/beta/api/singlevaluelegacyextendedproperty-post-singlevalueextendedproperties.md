---
title: Criar uma propriedade estendida de valor único
description: 'Crie uma ou mais propriedades estendidas de vários valores em uma instância nova ou existente de um recurso. '
ms.openlocfilehash: c55ab01ecde214feb38857e8d77f83eb3bfbabc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035105"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="5a23f-103">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="5a23f-103">Create single-value extended property</span></span>

> <span data-ttu-id="5a23f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a23f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a23f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a23f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a23f-106">Crie uma ou mais propriedades estendidas de vários valores em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="5a23f-106">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="5a23f-107">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="5a23f-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="5a23f-108">calendar</span><span class="sxs-lookup"><span data-stu-id="5a23f-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="5a23f-109">contact</span><span class="sxs-lookup"><span data-stu-id="5a23f-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="5a23f-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5a23f-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="5a23f-111">evento</span><span class="sxs-lookup"><span data-stu-id="5a23f-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="5a23f-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a23f-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="5a23f-113">message</span><span class="sxs-lookup"><span data-stu-id="5a23f-113">message</span></span>](../resources/message.md)
- [<span data-ttu-id="5a23f-114">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="5a23f-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="5a23f-115">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="5a23f-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="5a23f-116">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="5a23f-116">As well as the following group resources:</span></span>

- <span data-ttu-id="5a23f-117">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="5a23f-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="5a23f-118">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="5a23f-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="5a23f-119">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="5a23f-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="5a23f-120">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="5a23f-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a23f-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a23f-121">Permissions</span></span>
<span data-ttu-id="5a23f-122">Dependendo do recurso, você está criando a propriedade estendida no e a permissão digite (delegada ou aplicativos) você solicitação, a permissão especificada na tabela a seguir é o mínimo necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5a23f-122">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="5a23f-123">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a23f-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a23f-124">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-124">Supported resource</span></span> | <span data-ttu-id="5a23f-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a23f-125">Delegated (work or school account)</span></span> | <span data-ttu-id="5a23f-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a23f-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a23f-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a23f-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="5a23f-128">calendar</span><span class="sxs-lookup"><span data-stu-id="5a23f-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="5a23f-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-129">Calendars.ReadWrite</span></span> | <span data-ttu-id="5a23f-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-130">Calendars.ReadWrite</span></span> | <span data-ttu-id="5a23f-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-131">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="5a23f-132">contato</span><span class="sxs-lookup"><span data-stu-id="5a23f-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5a23f-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-133">Contacts.ReadWrite</span></span> | <span data-ttu-id="5a23f-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-134">Contacts.ReadWrite</span></span> | <span data-ttu-id="5a23f-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-135">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="5a23f-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5a23f-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="5a23f-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-137">Contacts.ReadWrite</span></span> | <span data-ttu-id="5a23f-138">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-138">Contacts.ReadWrite</span></span> | <span data-ttu-id="5a23f-139">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-139">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="5a23f-140">evento</span><span class="sxs-lookup"><span data-stu-id="5a23f-140">event</span></span>](../resources/event.md) | <span data-ttu-id="5a23f-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-141">Calendars.ReadWrite</span></span> | <span data-ttu-id="5a23f-142">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-142">Calendars.ReadWrite</span></span> |  <span data-ttu-id="5a23f-143">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-143">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="5a23f-144">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="5a23f-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="5a23f-145">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a23f-145">Group.ReadWrite.All</span></span> | <span data-ttu-id="5a23f-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-146">Not supported</span></span> | <span data-ttu-id="5a23f-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-147">Not supported</span></span> |
| <span data-ttu-id="5a23f-148">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="5a23f-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="5a23f-149">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a23f-149">Group.ReadWrite.All</span></span> | <span data-ttu-id="5a23f-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-150">Not supported</span></span> | <span data-ttu-id="5a23f-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-151">Not supported</span></span> |
| <span data-ttu-id="5a23f-152">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="5a23f-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="5a23f-153">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a23f-153">Group.ReadWrite.All</span></span> | <span data-ttu-id="5a23f-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-154">Not supported</span></span> | <span data-ttu-id="5a23f-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-155">Not supported</span></span> |
| [<span data-ttu-id="5a23f-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5a23f-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="5a23f-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-157">Mail.ReadWrite</span></span> | <span data-ttu-id="5a23f-158">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-158">Mail.ReadWrite</span></span> | <span data-ttu-id="5a23f-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-159">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="5a23f-160">mensagem</span><span class="sxs-lookup"><span data-stu-id="5a23f-160">message</span></span>](../resources/message.md) | <span data-ttu-id="5a23f-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-161">Mail.ReadWrite</span></span> | <span data-ttu-id="5a23f-162">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-162">Mail.ReadWrite</span></span> | <span data-ttu-id="5a23f-163">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-163">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="5a23f-164">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="5a23f-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="5a23f-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="5a23f-166">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-166">Tasks.ReadWrite</span></span> | <span data-ttu-id="5a23f-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-167">Not supported</span></span> |
| [<span data-ttu-id="5a23f-168">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="5a23f-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="5a23f-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="5a23f-170">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a23f-170">Tasks.ReadWrite</span></span> | <span data-ttu-id="5a23f-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5a23f-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="5a23f-172">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a23f-172">HTTP request</span></span>
<span data-ttu-id="5a23f-173">Você pode criar propriedades estendidas em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="5a23f-173">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="5a23f-174">Para criar um ou mais propriedades estendidas em uma _nova_ instância de recurso, use a mesma solicitação REST como criando a instância e inclua as propriedades do novo recurso instância _e a propriedade estendida_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a23f-174">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="5a23f-175">Observe que alguns recursos oferecem suporte a criação de mais de uma forma.</span><span class="sxs-lookup"><span data-stu-id="5a23f-175">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="5a23f-176">Para obter mais informações sobre como criar essas instâncias de recurso, consulte os tópicos correspondentes para a criação de uma [mensagem](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [evento](../api/user-post-events.md), [calendário](../api/user-post-calendars.md), [Contatos](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [, de [tarefa do Outlook](../resources/outlooktask.md) Pasta de tarefas do Outlook](../resources/outlooktaskfolder.md), [eventos de grupo](../api/group-post-events.md)e de [postagem de grupo](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="5a23f-176">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="5a23f-177">Veja a seguir a sintaxe das solicitações.</span><span class="sxs-lookup"><span data-stu-id="5a23f-177">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
POST /me/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks

POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="5a23f-178">Para criar uma ou mais propriedades estendidas em uma instância de recurso existente, especifique essa instância na solicitação e inclua a propriedade estendida no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a23f-178">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="5a23f-179">**Observação** Não é possível criar uma propriedade estendida em uma postagem de grupo existente.</span><span class="sxs-lookup"><span data-stu-id="5a23f-179">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /me/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

PATCH /me/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5a23f-180">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a23f-180">Request headers</span></span>
| <span data-ttu-id="5a23f-181">Nome</span><span class="sxs-lookup"><span data-stu-id="5a23f-181">Name</span></span>       | <span data-ttu-id="5a23f-182">Valor</span><span class="sxs-lookup"><span data-stu-id="5a23f-182">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5a23f-183">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a23f-183">Authorization</span></span> | <span data-ttu-id="5a23f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a23f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a23f-186">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a23f-186">Content-Type</span></span> | <span data-ttu-id="5a23f-187">application/json</span><span class="sxs-lookup"><span data-stu-id="5a23f-187">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a23f-188">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a23f-188">Request body</span></span>

<span data-ttu-id="5a23f-189">Forneça um corpo JSON de cada objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) na propriedade da coleção **singleValueExtendedProperties** da instância do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a23f-189">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="5a23f-190">**.**</span><span class="sxs-lookup"><span data-stu-id="5a23f-190">**Property**</span></span>|<span data-ttu-id="5a23f-191">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="5a23f-191">**Type**</span></span>|<span data-ttu-id="5a23f-192">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5a23f-192">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5a23f-193">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5a23f-193">singleValueExtendedProperties</span></span>|<span data-ttu-id="5a23f-194">Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5a23f-194">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5a23f-195">Uma matriz de uma ou mais propriedades estendidas de valor único.</span><span class="sxs-lookup"><span data-stu-id="5a23f-195">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="5a23f-196">id</span><span class="sxs-lookup"><span data-stu-id="5a23f-196">id</span></span>|<span data-ttu-id="5a23f-197">String</span><span class="sxs-lookup"><span data-stu-id="5a23f-197">String</span></span>|<span data-ttu-id="5a23f-p105">Para cada propriedade na coleção **singleValueExtendedProperties**, especifique isso para identificar a propriedade. Deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a23f-p105">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="5a23f-202">valor</span><span class="sxs-lookup"><span data-stu-id="5a23f-202">value</span></span>|<span data-ttu-id="5a23f-203">string</span><span class="sxs-lookup"><span data-stu-id="5a23f-203">string</span></span>|<span data-ttu-id="5a23f-p106">Para cada propriedade na coleção **singleValueExtendedProperties**, especifique o valor da propriedade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a23f-p106">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="5a23f-206">Ao criar uma propriedade estendida em uma _nova_ instância de recurso, além da nova coleção **singleValueExtendedProperties**, forneça uma representação JSON dessa instância de recurso (ou seja, [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span><span class="sxs-lookup"><span data-stu-id="5a23f-206">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="5a23f-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a23f-207">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="5a23f-208">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="5a23f-208">Response code</span></span>
<span data-ttu-id="5a23f-209">Uma operação bem-sucedida na criação de uma propriedade estendida em uma nova instância de recurso retorna `201 Created`, exceto em uma nova postagem de grupo. Dependendo do método usado, a operação pode retornar `200 OK` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="5a23f-209">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="5a23f-210">Em uma instância de recurso existente, uma operação de criação bem-sucedida retorna `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="5a23f-210">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="5a23f-211">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="5a23f-211">Response body</span></span>

<span data-ttu-id="5a23f-p107">Ao criar uma propriedade estendida, a resposta inclui apenas a instância nova ou existente, mas não a nova propriedade estendida. Para ver a propriedade estendida recém-criada, [obtenha a instância expandida com a propriedade estendida](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="5a23f-p107">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="5a23f-214">Ao criar uma propriedade estendida em uma _nova_ [postagem de grupo](../resources/post.md) respondendo a um thread ou postagem, a resposta inclui um código de resposta, mas não a nova postagem nem a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="5a23f-214">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="5a23f-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a23f-215">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="5a23f-216">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="5a23f-216">Request 1</span></span>

<span data-ttu-id="5a23f-p108">O primeiro exemplo cria um novo evento e uma propriedade de valor único estendida na mesma operação POST. Além das propriedades que você normalmente incluiria para um novo evento, o corpo da solicitação inclui a coleção **singleValueExtendedProperties**, que contém uma propriedade estendida de valor único e as seguintes informações sobre a propriedade:</span><span class="sxs-lookup"><span data-stu-id="5a23f-p108">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="5a23f-219">**id** especifica o tipo de propriedade como `String`, o GUID e a propriedade nomeada `Fun`.</span><span class="sxs-lookup"><span data-stu-id="5a23f-219">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="5a23f-220">**value** especifica `Food` como o valor da propriedade `Fun`.</span><span class="sxs-lookup"><span data-stu-id="5a23f-220">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="5a23f-221">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="5a23f-221">Response 1</span></span>

<span data-ttu-id="5a23f-p109">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 201 Created` e inclui o novo evento em seu corpo, semelhante à resposta da [criação de apenas um evento](../api/user-post-events.md). A resposta não inclui propriedades estendidas recém-criadas.</span><span class="sxs-lookup"><span data-stu-id="5a23f-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="5a23f-224">Para ver a propriedade estendida recém-criada, [obtenha o evento expandido com a propriedade estendida](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="5a23f-224">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="5a23f-225">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="5a23f-225">Request 2</span></span>

<span data-ttu-id="5a23f-p110">O segundo exemplo cria uma propriedade estendido de valor único para a mensagem especificada existente. A propriedade estendida é o único elemento na matriz **singleValueExtendedProperties**. O corpo da solicitação inclui o seguinte para essa propriedade estendida:</span><span class="sxs-lookup"><span data-stu-id="5a23f-p110">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="5a23f-229">**id** especifica o tipo de propriedade como `String`, o GUID e a propriedade nomeada `Color`.</span><span class="sxs-lookup"><span data-stu-id="5a23f-229">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="5a23f-230">**value** especifica `Green` como o valor da propriedade `Color`.</span><span class="sxs-lookup"><span data-stu-id="5a23f-230">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="5a23f-231">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="5a23f-231">Response 2</span></span>

<span data-ttu-id="5a23f-p111">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK` e inclui a mensagem especificada em seu corpo, semelhante à resposta da [atualização de uma mensagem](../api/message-update.md). A resposta não inclui a propriedade estendida recém-criada.</span><span class="sxs-lookup"><span data-stu-id="5a23f-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="5a23f-234">Para ver a propriedade estendida recém-criada, [obtenha a mensagem expandida com a propriedade estendida](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="5a23f-234">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

