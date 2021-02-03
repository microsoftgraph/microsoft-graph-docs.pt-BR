---
title: Obter extensão aberta
description: Obtenha uma extensão aberta (objeto openTypeExtension) identificada por nome ou nome totalmente qualificado.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 2071e8e6520cfc1145b0e88faabf3a0969f9ac96
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092705"
---
# <a name="get-open-extension"></a><span data-ttu-id="89d89-103">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="89d89-103">Get open extension</span></span>

<span data-ttu-id="89d89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89d89-105">Obtenha uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) identificada por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="89d89-105">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="89d89-106">A tabela na seção [Permissões lista os](#permissions) recursos que suportam extensões abertas.</span><span class="sxs-lookup"><span data-stu-id="89d89-106">The table in the [Permissions](#permissions) section lists the resources that support open extensions.</span></span>

<span data-ttu-id="89d89-107">A tabela a seguir lista os três cenários em que é possível obter uma extensão aberta de uma instância de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="89d89-107">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="89d89-108">**Cenário GET**</span><span class="sxs-lookup"><span data-stu-id="89d89-108">**GET scenario**</span></span>|<span data-ttu-id="89d89-109">**Recursos com suporte**</span><span class="sxs-lookup"><span data-stu-id="89d89-109">**Supported resources**</span></span>|<span data-ttu-id="89d89-110">**Corpo da resposta**</span><span class="sxs-lookup"><span data-stu-id="89d89-110">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="89d89-111">Obtenha uma extensão específica de uma instância de recurso conhecida.</span><span class="sxs-lookup"><span data-stu-id="89d89-111">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="89d89-112">[Unidade administrativa](../resources/administrativeunit.md), [dispositivo](../resources/device.md), [evento](../resources/event.md), [grupo](../resources/group.md) [,](../resources/event.md)evento de grupo , [postagem](../resources/post.md)de [grupo](../resources/message.md) [,](../resources/organization.md)mensagem , organização , [contato](../resources/contact.md)pessoal , [usuário](../resources/user.md), [tarefa](../resources/todotask.md), lista [de tarefas](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="89d89-112">[Administrative unit](../resources/administrativeunit.md), [device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md), [task](../resources/todotask.md), [tasklist](../resources/todotasklist.md)</span></span>  | <span data-ttu-id="89d89-113">Somente extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="89d89-113">Open extension only.</span></span>|
|<span data-ttu-id="89d89-114">Obtenha uma instância de recurso conhecida, expandida com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="89d89-114">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="89d89-115">Unidade administrativa, dispositivo, evento, grupo, evento de grupo, postagem de grupo, mensagem, organização, contato pessoal, usuário, tarefa, lista de tarefas.</span><span class="sxs-lookup"><span data-stu-id="89d89-115">Administrative unit, device, event, group, group event, group post, message, organization, personal contact, user, task, task list.</span></span> |<span data-ttu-id="89d89-116">Uma instância de recurso expandida com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="89d89-116">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="89d89-117">Encontre e expanda instâncias de recursos com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="89d89-117">Find and expand resource instances with a specific extension.</span></span> | <span data-ttu-id="89d89-118">Evento, evento de grupo, postagem de grupo, mensagem, contato pessoal, tarefa, lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="89d89-118">Event, group event, group post, message, personal contact, task, task list</span></span> |<span data-ttu-id="89d89-119">Instâncias de recursos expandidas com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="89d89-119">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="89d89-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="89d89-120">Permissions</span></span>

<span data-ttu-id="89d89-121">Dependendo do recurso que contém a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="89d89-121">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="89d89-122">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher permissões mais privilegiadas, procure as seguintes permissões em [Permissões.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="89d89-122">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89d89-123">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="89d89-123">Supported resource</span></span> | <span data-ttu-id="89d89-124">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89d89-124">Delegated (work or school account)</span></span> | <span data-ttu-id="89d89-125">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89d89-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89d89-126">Application</span><span class="sxs-lookup"><span data-stu-id="89d89-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="89d89-127">device</span><span class="sxs-lookup"><span data-stu-id="89d89-127">device</span></span>](../resources/device.md) | <span data-ttu-id="89d89-128">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d89-128">Directory.Read.All</span></span> | <span data-ttu-id="89d89-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89d89-129">Not supported</span></span> | <span data-ttu-id="89d89-130">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d89-130">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="89d89-131">evento</span><span class="sxs-lookup"><span data-stu-id="89d89-131">event</span></span>](../resources/event.md) | <span data-ttu-id="89d89-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-132">Calendars.Read</span></span> | <span data-ttu-id="89d89-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-133">Calendars.Read</span></span> | <span data-ttu-id="89d89-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-134">Calendars.Read</span></span> |
| [<span data-ttu-id="89d89-135">grupo</span><span class="sxs-lookup"><span data-stu-id="89d89-135">group</span></span>](../resources/group.md) | <span data-ttu-id="89d89-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d89-136">Group.Read.All</span></span> | <span data-ttu-id="89d89-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89d89-137">Not supported</span></span> | <span data-ttu-id="89d89-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d89-138">Group.Read.All</span></span> |
| [<span data-ttu-id="89d89-139">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="89d89-139">group event</span></span>](../resources/event.md) | <span data-ttu-id="89d89-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d89-140">Group.Read.All</span></span> | <span data-ttu-id="89d89-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89d89-141">Not supported</span></span> | <span data-ttu-id="89d89-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89d89-142">Not supported</span></span> |
| [<span data-ttu-id="89d89-143">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="89d89-143">group post</span></span>](../resources/post.md) | <span data-ttu-id="89d89-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d89-144">Group.Read.All</span></span> | <span data-ttu-id="89d89-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="89d89-145">Not supported</span></span> | <span data-ttu-id="89d89-146">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d89-146">Group.Read.All</span></span> |
| [<span data-ttu-id="89d89-147">message</span><span class="sxs-lookup"><span data-stu-id="89d89-147">message</span></span>](../resources/message.md) | <span data-ttu-id="89d89-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-148">Mail.Read</span></span> | <span data-ttu-id="89d89-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-149">Mail.Read</span></span> | <span data-ttu-id="89d89-150">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-150">Mail.Read</span></span> | 
| [<span data-ttu-id="89d89-151">organização</span><span class="sxs-lookup"><span data-stu-id="89d89-151">organization</span></span>](../resources/organization.md) | <span data-ttu-id="89d89-152">User.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-152">User.Read</span></span> | <span data-ttu-id="89d89-153">Incompatível</span><span class="sxs-lookup"><span data-stu-id="89d89-153">Not supported</span></span> | <span data-ttu-id="89d89-154">Organization.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d89-154">Organization.Read.All</span></span> |
| [<span data-ttu-id="89d89-155">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="89d89-155">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="89d89-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-156">Contacts.Read</span></span> | <span data-ttu-id="89d89-157">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-157">Contacts.Read</span></span> | <span data-ttu-id="89d89-158">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-158">Contacts.Read</span></span> |
| [<span data-ttu-id="89d89-159">usuário</span><span class="sxs-lookup"><span data-stu-id="89d89-159">user</span></span>](../resources/user.md) | <span data-ttu-id="89d89-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-160">User.Read</span></span> | <span data-ttu-id="89d89-161">User.Read</span><span class="sxs-lookup"><span data-stu-id="89d89-161">User.Read</span></span> | <span data-ttu-id="89d89-162">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="89d89-162">User.Read.All</span></span> |
| [<span data-ttu-id="89d89-163">task</span><span class="sxs-lookup"><span data-stu-id="89d89-163">task</span></span>](../resources/todotask.md) | <span data-ttu-id="89d89-164">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89d89-164">Tasks.ReadWrite</span></span> | <span data-ttu-id="89d89-165">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89d89-165">Tasks.ReadWrite</span></span> | <span data-ttu-id="89d89-166">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d89-166">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="89d89-167">tasklist</span><span class="sxs-lookup"><span data-stu-id="89d89-167">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="89d89-168">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89d89-168">Tasks.ReadWrite</span></span> | <span data-ttu-id="89d89-169">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89d89-169">Tasks.ReadWrite</span></span> | <span data-ttu-id="89d89-170">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d89-170">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89d89-171">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89d89-171">HTTP request</span></span>

<span data-ttu-id="89d89-172">Esta seção lista a sintaxe de cada um dos três cenários `GET` descritos acima</span><span class="sxs-lookup"><span data-stu-id="89d89-172">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="89d89-173">Obtenha uma extensão específica em uma instância de recurso conhecida</span><span class="sxs-lookup"><span data-stu-id="89d89-173">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="89d89-174">Use a mesma solicitação REST obtendo a instância do recurso e identifique a extensão usando a propriedade de navegação **extensions** dessa instância.</span><span class="sxs-lookup"><span data-stu-id="89d89-174">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{Id}/extensions/{extensionId}
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/extensions/{extensionId}
```

### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="89d89-175">Obtenha uma instância de recurso conhecida, expandida com uma extensão correspondente.</span><span class="sxs-lookup"><span data-stu-id="89d89-175">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="89d89-176">Para o evento, evento de grupo, postagem de grupo, mensagem, contato pessoal, tarefa, tipos de recurso de lista de tarefas, você pode usar a mesma solicitação REST como obter a instância do recurso, procurar uma extensão que corresponde a um filtro em sua propriedade **de ID** e expandir a instância com a extensão.</span><span class="sxs-lookup"><span data-stu-id="89d89-176">For the event, group event, group post, message, personal contact, task, task list resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension.</span></span> <span data-ttu-id="89d89-177">A resposta inclui a maioria das propriedades do recurso.</span><span class="sxs-lookup"><span data-stu-id="89d89-177">The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/todo/lists/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="89d89-178">Para os tipos de recurso de dispositivo, grupo, organização e usuário, você também deve usar um parâmetro `$select` para incluir a propriedade **id** e quaisquer outras propriedades que você deseja na instância do recurso:</span><span class="sxs-lookup"><span data-stu-id="89d89-178">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```


### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="89d89-179">Filtrar as instâncias do recurso expandidas com uma extensão correspondente</span><span class="sxs-lookup"><span data-stu-id="89d89-179">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="89d89-180">Use a mesma solicitação REST para obter uma coleção do recurso suportado, filtre a coleção para instâncias que contêm uma extensão com uma propriedade **id** correspondente e expanda essas instâncias com a extensão.</span><span class="sxs-lookup"><span data-stu-id="89d89-180">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="89d89-181">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso ou coleção, para obter uma extensão dela.</span><span class="sxs-lookup"><span data-stu-id="89d89-181">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it.</span></span> <span data-ttu-id="89d89-182">Todas as outras sintaxes que permitem identificar essas instâncias de recursos ou coleções dão suporte à obtenção de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="89d89-182">All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="89d89-183">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="89d89-183">Path parameters</span></span>
|<span data-ttu-id="89d89-184">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="89d89-184">**Parameter**</span></span>|<span data-ttu-id="89d89-185">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="89d89-185">**Type**</span></span>|<span data-ttu-id="89d89-186">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89d89-186">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="89d89-187">Id</span><span class="sxs-lookup"><span data-stu-id="89d89-187">Id</span></span>|<span data-ttu-id="89d89-188">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89d89-188">string</span></span>|<span data-ttu-id="89d89-p104">Espaço reservado para um identificador exclusivo de um objeto na coleção correspondente, como mensagens, contatos e eventos. Obrigatório. Não deve ser confundido com a propriedade **id** de uma **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="89d89-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="89d89-192">extensionId</span><span class="sxs-lookup"><span data-stu-id="89d89-192">extensionId</span></span>|<span data-ttu-id="89d89-193">string</span><span class="sxs-lookup"><span data-stu-id="89d89-193">string</span></span>|<span data-ttu-id="89d89-p105">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para um a uma extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade **id** quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89d89-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="89d89-197">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89d89-197">Optional query parameters</span></span>

<span data-ttu-id="89d89-198">Verifique se aplicou a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de caracteres `$filter`.</span><span class="sxs-lookup"><span data-stu-id="89d89-198">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="89d89-199">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="89d89-199">Parameter</span></span>|<span data-ttu-id="89d89-200">Descrição</span><span class="sxs-lookup"><span data-stu-id="89d89-200">Description</span></span>|<span data-ttu-id="89d89-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89d89-201">Example</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="89d89-202">$filter</span><span class="sxs-lookup"><span data-stu-id="89d89-202">$filter</span></span>|<span data-ttu-id="89d89-203">Retorna uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="89d89-203">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="89d89-204">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="89d89-204">Request 3</span></span>](#request-3)|
|<span data-ttu-id="89d89-205">$filter com o operador **any**</span><span class="sxs-lookup"><span data-stu-id="89d89-205">$filter with **any** operator</span></span>|<span data-ttu-id="89d89-206">Retorna instâncias de uma coleção de recursos que contêm uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="89d89-206">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="89d89-207">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="89d89-207">Request 5</span></span>](#request-5)|
|<span data-ttu-id="89d89-208">$expand</span><span class="sxs-lookup"><span data-stu-id="89d89-208">$expand</span></span>|<span data-ttu-id="89d89-209">Expande uma instância de recurso para incluir uma extensão.</span><span class="sxs-lookup"><span data-stu-id="89d89-209">Expands a resource instance to include an extension.</span></span> |<span data-ttu-id="89d89-210">[Solicitação 3](#request-3) e [solicitação 5](#request-5)</span><span class="sxs-lookup"><span data-stu-id="89d89-210">[Request 3](#request-3) and [request 5](#request-5)</span></span>|

## <a name="request-headers"></a><span data-ttu-id="89d89-211">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89d89-211">Request headers</span></span>
| <span data-ttu-id="89d89-212">Nome</span><span class="sxs-lookup"><span data-stu-id="89d89-212">Name</span></span>       | <span data-ttu-id="89d89-213">Valor</span><span class="sxs-lookup"><span data-stu-id="89d89-213">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="89d89-214">Autorização</span><span class="sxs-lookup"><span data-stu-id="89d89-214">Authorization</span></span> | <span data-ttu-id="89d89-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89d89-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89d89-217">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89d89-217">Request body</span></span>
<span data-ttu-id="89d89-218">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89d89-218">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89d89-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="89d89-219">Response</span></span>

<span data-ttu-id="89d89-p107">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [openTypeExtension](../resources/opentypeextension.md) no corpo da resposta. Dependendo da consulta GET, o corpo da resposta exato pode ser diferente.</span><span class="sxs-lookup"><span data-stu-id="89d89-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="89d89-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89d89-222">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="89d89-223">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="89d89-223">Request 1</span></span>

<span data-ttu-id="89d89-p108">O primeiro exemplo mostra 2 maneiras de referenciar uma extensão e obtém a extensão na mensagem especificada. A resposta é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="89d89-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="89d89-226">Em primeiro lugar, por nome:</span><span class="sxs-lookup"><span data-stu-id="89d89-226">First, by its name:</span></span> 


# <a name="http"></a>[<span data-ttu-id="89d89-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="89d89-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="89d89-228">C#</span><span class="sxs-lookup"><span data-stu-id="89d89-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89d89-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89d89-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89d89-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89d89-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89d89-231">Java</span><span class="sxs-lookup"><span data-stu-id="89d89-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="89d89-232">Em segundo lugar, por ID (nome totalmente qualificado):</span><span class="sxs-lookup"><span data-stu-id="89d89-232">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==='/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

#### <a name="response-1"></a><span data-ttu-id="89d89-233">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="89d89-233">Response 1</span></span>
<span data-ttu-id="89d89-234">Veja a seguir a resposta para o primeiro exemplo.</span><span class="sxs-lookup"><span data-stu-id="89d89-234">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="89d89-235">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="89d89-235">Request 2</span></span>

<span data-ttu-id="89d89-236">O segundo exemplo faz referência a uma extensão por nome e obtém essa extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="89d89-236">The second example references an extension by its name and gets the extension in the specified group event.</span></span>


# <a name="http"></a>[<span data-ttu-id="89d89-237">HTTP</span><span class="sxs-lookup"><span data-stu-id="89d89-237">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal
```
# <a name="c"></a>[<span data-ttu-id="89d89-238">C#</span><span class="sxs-lookup"><span data-stu-id="89d89-238">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89d89-239">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89d89-239">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89d89-240">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89d89-240">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89d89-241">Java</span><span class="sxs-lookup"><span data-stu-id="89d89-241">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="89d89-242">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="89d89-242">Response 2</span></span>

<span data-ttu-id="89d89-243">Veja a seguir a resposta do segundo exemplo.</span><span class="sxs-lookup"><span data-stu-id="89d89-243">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl7IsAAA%3D/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="89d89-244">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="89d89-244">Request 3</span></span>

<span data-ttu-id="89d89-p109">O terceiro exemplo obtém e expande a mensagem especificada, incluindo a extensão retornada de um filtro. O filtro retorna a extensão cujo **id** corresponde a um nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="89d89-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>


# <a name="http"></a>[<span data-ttu-id="89d89-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="89d89-247">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```
# <a name="c"></a>[<span data-ttu-id="89d89-248">C#</span><span class="sxs-lookup"><span data-stu-id="89d89-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89d89-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89d89-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89d89-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89d89-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89d89-251">Java</span><span class="sxs-lookup"><span data-stu-id="89d89-251">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response-3"></a><span data-ttu-id="89d89-252">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="89d89-252">Response 3</span></span>

<span data-ttu-id="89d89-p110">Veja a seguir a resposta do terceiro exemplo. Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89d89-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
}
```

****

#### <a name="request-4"></a><span data-ttu-id="89d89-256">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="89d89-256">Request 4</span></span>

<span data-ttu-id="89d89-257">O quarto exemplo faz referência a uma extensão por nome totalmente qualificado e obtém essa extensão na postagem de grupo especificada.</span><span class="sxs-lookup"><span data-stu-id="89d89-257">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>


# <a name="http"></a>[<span data-ttu-id="89d89-258">HTTP</span><span class="sxs-lookup"><span data-stu-id="89d89-258">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```
# <a name="c"></a>[<span data-ttu-id="89d89-259">C#</span><span class="sxs-lookup"><span data-stu-id="89d89-259">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89d89-260">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89d89-260">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89d89-261">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89d89-261">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89d89-262">Java</span><span class="sxs-lookup"><span data-stu-id="89d89-262">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-4"></a><span data-ttu-id="89d89-263">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="89d89-263">Response 4</span></span>

<span data-ttu-id="89d89-264">Veja a seguir a resposta do quarto exemplo.</span><span class="sxs-lookup"><span data-stu-id="89d89-264">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```


#### <a name="request-5"></a><span data-ttu-id="89d89-265">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="89d89-265">Request 5</span></span>

<span data-ttu-id="89d89-p111">O quinto exemplo analisa todas as mensagens na caixa de correio do usuário conectado para localizar aquelas uma contêm uma extensão correspondente a um filtro e as expande com a inclusão dessa extensão. O filtro retorna extensões cuja propriedade **id** corresponde ao nome da extensão `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="89d89-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


#### <a name="response-5"></a><span data-ttu-id="89d89-268">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="89d89-268">Response 5</span></span>

<span data-ttu-id="89d89-269">Nessa resposta do quinto exemplo, há apenas uma mensagem na caixa de correio do usuário que tem uma extensão cuja **id** é igual a `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="89d89-269">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="89d89-p112">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89d89-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/beta/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
        "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
  }
  ]
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


