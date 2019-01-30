---
title: Criar uma propriedade estendida de valor único
description: 'Crie uma ou mais propriedades estendidas de vários valores em uma instância nova ou existente de um recurso. '
localization_priority: Normal
ms.openlocfilehash: 3b122eb1a02ddd9e413f5c58bf840b912dd8365f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641390"
---
# <a name="create-single-value-extended-property"></a><span data-ttu-id="aabe1-103">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="aabe1-103">Create single-value extended property</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aabe1-104">Crie uma ou mais propriedades estendidas de vários valores em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="aabe1-104">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="aabe1-105">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="aabe1-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="aabe1-106">calendar</span><span class="sxs-lookup"><span data-stu-id="aabe1-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="aabe1-107">contact</span><span class="sxs-lookup"><span data-stu-id="aabe1-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="aabe1-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="aabe1-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="aabe1-109">evento</span><span class="sxs-lookup"><span data-stu-id="aabe1-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="aabe1-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="aabe1-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="aabe1-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="aabe1-111">message</span></span>](../resources/message.md)
- [<span data-ttu-id="aabe1-112">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="aabe1-112">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="aabe1-113">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="aabe1-113">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="aabe1-114">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="aabe1-114">As well as the following group resources:</span></span>

- <span data-ttu-id="aabe1-115">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="aabe1-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="aabe1-116">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="aabe1-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="aabe1-117">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="aabe1-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="aabe1-118">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="aabe1-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="aabe1-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="aabe1-119">Permissions</span></span>
<span data-ttu-id="aabe1-120">Dependendo do recurso, você está criando a propriedade estendida no e a permissão digite (delegada ou aplicativos) você solicitação, a permissão especificada na tabela a seguir é o mínimo necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="aabe1-120">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="aabe1-121">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aabe1-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aabe1-122">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-122">Supported resource</span></span> | <span data-ttu-id="aabe1-123">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aabe1-123">Delegated (work or school account)</span></span> | <span data-ttu-id="aabe1-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aabe1-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aabe1-125">Application</span><span class="sxs-lookup"><span data-stu-id="aabe1-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="aabe1-126">calendar</span><span class="sxs-lookup"><span data-stu-id="aabe1-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="aabe1-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-127">Calendars.ReadWrite</span></span> | <span data-ttu-id="aabe1-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-128">Calendars.ReadWrite</span></span> | <span data-ttu-id="aabe1-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-129">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="aabe1-130">contato</span><span class="sxs-lookup"><span data-stu-id="aabe1-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="aabe1-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="aabe1-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="aabe1-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="aabe1-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="aabe1-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="aabe1-135">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-135">Contacts.ReadWrite</span></span> | <span data-ttu-id="aabe1-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-136">Contacts.ReadWrite</span></span> | <span data-ttu-id="aabe1-137">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-137">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="aabe1-138">evento</span><span class="sxs-lookup"><span data-stu-id="aabe1-138">event</span></span>](../resources/event.md) | <span data-ttu-id="aabe1-139">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-139">Calendars.ReadWrite</span></span> | <span data-ttu-id="aabe1-140">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-140">Calendars.ReadWrite</span></span> |  <span data-ttu-id="aabe1-141">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-141">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="aabe1-142">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="aabe1-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="aabe1-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aabe1-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="aabe1-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-144">Not supported</span></span> | <span data-ttu-id="aabe1-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-145">Not supported</span></span> |
| <span data-ttu-id="aabe1-146">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="aabe1-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="aabe1-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aabe1-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="aabe1-148">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-148">Not supported</span></span> | <span data-ttu-id="aabe1-149">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-149">Not supported</span></span> |
| <span data-ttu-id="aabe1-150">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="aabe1-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="aabe1-151">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aabe1-151">Group.ReadWrite.All</span></span> | <span data-ttu-id="aabe1-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-152">Not supported</span></span> | <span data-ttu-id="aabe1-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-153">Not supported</span></span> |
| [<span data-ttu-id="aabe1-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="aabe1-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="aabe1-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-155">Mail.ReadWrite</span></span> | <span data-ttu-id="aabe1-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-156">Mail.ReadWrite</span></span> | <span data-ttu-id="aabe1-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-157">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="aabe1-158">mensagem</span><span class="sxs-lookup"><span data-stu-id="aabe1-158">message</span></span>](../resources/message.md) | <span data-ttu-id="aabe1-159">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-159">Mail.ReadWrite</span></span> | <span data-ttu-id="aabe1-160">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-160">Mail.ReadWrite</span></span> | <span data-ttu-id="aabe1-161">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-161">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="aabe1-162">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="aabe1-162">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="aabe1-163">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-163">Tasks.ReadWrite</span></span> | <span data-ttu-id="aabe1-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="aabe1-165">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-165">Not supported</span></span> |
| [<span data-ttu-id="aabe1-166">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="aabe1-166">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="aabe1-167">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-167">Tasks.ReadWrite</span></span> | <span data-ttu-id="aabe1-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aabe1-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="aabe1-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="aabe1-169">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="aabe1-170">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aabe1-170">HTTP request</span></span>
<span data-ttu-id="aabe1-171">Você pode criar propriedades estendidas em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="aabe1-171">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="aabe1-172">Para criar um ou mais propriedades estendidas em uma _nova_ instância de recurso, use a mesma solicitação REST como criando a instância e inclua as propriedades do novo recurso instância _e a propriedade estendida_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aabe1-172">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body.</span></span>
<span data-ttu-id="aabe1-173">Observe que alguns recursos oferecem suporte a criação de mais de uma forma.</span><span class="sxs-lookup"><span data-stu-id="aabe1-173">Note that some resources support creation in more than one way.</span></span> <span data-ttu-id="aabe1-174">Para obter mais informações sobre como criar essas instâncias de recurso, consulte os tópicos correspondentes para a criação de uma [mensagem](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [evento](../api/user-post-events.md), [calendário](../api/user-post-calendars.md), [Contatos](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [, de [tarefa do Outlook](../resources/outlooktask.md) Pasta de tarefas do Outlook](../resources/outlooktaskfolder.md), [eventos de grupo](../api/group-post-events.md)e de [postagem de grupo](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="aabe1-174">For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [event](../api/user-post-events.md), [calendar](../api/user-post-calendars.md), [contact](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), [group event](../api/group-post-events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="aabe1-175">Veja a seguir a sintaxe das solicitações.</span><span class="sxs-lookup"><span data-stu-id="aabe1-175">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="aabe1-176">Para criar uma ou mais propriedades estendidas em uma instância de recurso existente, especifique essa instância na solicitação e inclua a propriedade estendida no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aabe1-176">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="aabe1-177">**Observação** Não é possível criar uma propriedade estendida em uma postagem de grupo existente.</span><span class="sxs-lookup"><span data-stu-id="aabe1-177">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="aabe1-178">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aabe1-178">Request headers</span></span>
| <span data-ttu-id="aabe1-179">Nome</span><span class="sxs-lookup"><span data-stu-id="aabe1-179">Name</span></span>       | <span data-ttu-id="aabe1-180">Valor</span><span class="sxs-lookup"><span data-stu-id="aabe1-180">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="aabe1-181">Autorização</span><span class="sxs-lookup"><span data-stu-id="aabe1-181">Authorization</span></span> | <span data-ttu-id="aabe1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aabe1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aabe1-184">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aabe1-184">Content-Type</span></span> | <span data-ttu-id="aabe1-185">application/json</span><span class="sxs-lookup"><span data-stu-id="aabe1-185">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="aabe1-186">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aabe1-186">Request body</span></span>

<span data-ttu-id="aabe1-187">Forneça um corpo JSON de cada objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) na propriedade da coleção **singleValueExtendedProperties** da instância do recurso.</span><span class="sxs-lookup"><span data-stu-id="aabe1-187">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="aabe1-188">**Propriedade**</span><span class="sxs-lookup"><span data-stu-id="aabe1-188">**Property**</span></span>|<span data-ttu-id="aabe1-189">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="aabe1-189">**Type**</span></span>|<span data-ttu-id="aabe1-190">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aabe1-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="aabe1-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="aabe1-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="aabe1-192">Coleção [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="aabe1-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="aabe1-193">Uma matriz de uma ou mais propriedades estendidas de valor único.</span><span class="sxs-lookup"><span data-stu-id="aabe1-193">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="aabe1-194">id</span><span class="sxs-lookup"><span data-stu-id="aabe1-194">id</span></span>|<span data-ttu-id="aabe1-195">String</span><span class="sxs-lookup"><span data-stu-id="aabe1-195">String</span></span>|<span data-ttu-id="aabe1-p104">Para cada propriedade na coleção **singleValueExtendedProperties**, especifique isso para identificar a propriedade. Deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aabe1-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="aabe1-200">valor</span><span class="sxs-lookup"><span data-stu-id="aabe1-200">value</span></span>|<span data-ttu-id="aabe1-201">string</span><span class="sxs-lookup"><span data-stu-id="aabe1-201">string</span></span>|<span data-ttu-id="aabe1-p105">Para cada propriedade na coleção **singleValueExtendedProperties**, especifique o valor da propriedade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aabe1-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="aabe1-204">Ao criar uma propriedade estendida em uma _nova_ instância de recurso, além da nova coleção **singleValueExtendedProperties**, forneça uma representação JSON dessa instância de recurso (ou seja, [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span><span class="sxs-lookup"><span data-stu-id="aabe1-204">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="aabe1-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="aabe1-205">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="aabe1-206">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="aabe1-206">Response code</span></span>
<span data-ttu-id="aabe1-207">Uma operação bem-sucedida na criação de uma propriedade estendida em uma nova instância de recurso retorna `201 Created`, exceto em uma nova postagem de grupo. Dependendo do método usado, a operação pode retornar `200 OK` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="aabe1-207">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="aabe1-208">Em uma instância de recurso existente, uma operação de criação bem-sucedida retorna `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="aabe1-208">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="aabe1-209">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="aabe1-209">Response body</span></span>

<span data-ttu-id="aabe1-p106">Ao criar uma propriedade estendida, a resposta inclui apenas a instância nova ou existente, mas não a nova propriedade estendida. Para ver a propriedade estendida recém-criada, [obtenha a instância expandida com a propriedade estendida](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="aabe1-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<span data-ttu-id="aabe1-212">Ao criar uma propriedade estendida em uma _nova_ [postagem de grupo](../resources/post.md) respondendo a um thread ou postagem, a resposta inclui um código de resposta, mas não a nova postagem nem a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="aabe1-212">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="aabe1-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aabe1-213">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="aabe1-214">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="aabe1-214">Request 1</span></span>

<span data-ttu-id="aabe1-p107">O primeiro exemplo cria um novo evento e uma propriedade de valor único estendida na mesma operação POST. Além das propriedades que você normalmente incluiria para um novo evento, o corpo da solicitação inclui a coleção **singleValueExtendedProperties**, que contém uma propriedade estendida de valor único e as seguintes informações sobre a propriedade:</span><span class="sxs-lookup"><span data-stu-id="aabe1-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>

- <span data-ttu-id="aabe1-217">**id** especifica o tipo de propriedade como `String`, o GUID e a propriedade nomeada `Fun`.</span><span class="sxs-lookup"><span data-stu-id="aabe1-217">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="aabe1-218">**value** especifica `Food` como o valor da propriedade `Fun`.</span><span class="sxs-lookup"><span data-stu-id="aabe1-218">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

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

##### <a name="response-1"></a><span data-ttu-id="aabe1-219">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="aabe1-219">Response 1</span></span>

<span data-ttu-id="aabe1-p108">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 201 Created` e inclui o novo evento em seu corpo, semelhante à resposta da [criação de apenas um evento](../api/user-post-events.md). A resposta não inclui propriedades estendidas recém-criadas.</span><span class="sxs-lookup"><span data-stu-id="aabe1-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user-post-events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="aabe1-222">Para ver a propriedade estendida recém-criada, [obtenha o evento expandido com a propriedade estendida](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="aabe1-222">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="aabe1-223">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="aabe1-223">Request 2</span></span>

<span data-ttu-id="aabe1-p109">O segundo exemplo cria uma propriedade estendido de valor único para a mensagem especificada existente. A propriedade estendida é o único elemento na matriz **singleValueExtendedProperties**. O corpo da solicitação inclui o seguinte para essa propriedade estendida:</span><span class="sxs-lookup"><span data-stu-id="aabe1-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="aabe1-227">**id** especifica o tipo de propriedade como `String`, o GUID e a propriedade nomeada `Color`.</span><span class="sxs-lookup"><span data-stu-id="aabe1-227">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="aabe1-228">**value** especifica `Green` como o valor da propriedade `Color`.</span><span class="sxs-lookup"><span data-stu-id="aabe1-228">**value** specifies `Green` as the value of the `Color` property.</span></span>

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

##### <a name="response-2"></a><span data-ttu-id="aabe1-229">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="aabe1-229">Response 2</span></span>

<span data-ttu-id="aabe1-p110">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK` e inclui a mensagem especificada em seu corpo, semelhante à resposta da [atualização de uma mensagem](../api/message-update.md). A resposta não inclui a propriedade estendida recém-criada.</span><span class="sxs-lookup"><span data-stu-id="aabe1-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message-update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="aabe1-232">Para ver a propriedade estendida recém-criada, [obtenha a mensagem expandida com a propriedade estendida](../api/singlevaluelegacyextendedproperty-get.md).</span><span class="sxs-lookup"><span data-stu-id="aabe1-232">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty-get.md).</span></span>

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

