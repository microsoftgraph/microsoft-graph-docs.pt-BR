---
title: Obter extensão aberta
description: Obtenha uma extensão aberta (objeto openTypeExtension) identificada por nome ou nome totalmente qualificado.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 5e861c038a6baa28e820775e4c0030a25e9095ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063097"
---
# <a name="get-open-extension"></a><span data-ttu-id="dfc02-103">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="dfc02-103">Get open extension</span></span>

<span data-ttu-id="dfc02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfc02-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfc02-105">Obtenha uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) identificada por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="dfc02-105">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="dfc02-106">A tabela a seguir lista os três cenários em que é possível obter uma extensão aberta de uma instância de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="dfc02-106">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="dfc02-107">**Cenário GET**</span><span class="sxs-lookup"><span data-stu-id="dfc02-107">**GET scenario**</span></span>|<span data-ttu-id="dfc02-108">**Recursos com suporte**</span><span class="sxs-lookup"><span data-stu-id="dfc02-108">**Supported resources**</span></span>|<span data-ttu-id="dfc02-109">**Corpo da resposta**</span><span class="sxs-lookup"><span data-stu-id="dfc02-109">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dfc02-110">Obtenha uma extensão específica de uma instância de recurso conhecida.</span><span class="sxs-lookup"><span data-stu-id="dfc02-110">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="dfc02-111">[Dispositivo](../resources/device.md), [evento](../resources/event.md), [grupo](../resources/group.md), [evento de grupo](../resources/event.md), [postagem de grupo](../resources/post.md), [mensagem](../resources/message.md), [organização](../resources/organization.md), [contato pessoal](../resources/contact.md), [usuário](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="dfc02-111">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="dfc02-112">Somente extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="dfc02-112">Open extension only.</span></span>|
|<span data-ttu-id="dfc02-113">Obtenha uma instância de recurso conhecida, expandida com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="dfc02-113">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="dfc02-114">Dispositivo, evento, grupo, evento de grupo, postagem de grupo, mensagem, organização, contato pessoal, usuário</span><span class="sxs-lookup"><span data-stu-id="dfc02-114">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="dfc02-115">Uma instância de recurso expandida com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="dfc02-115">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="dfc02-116">Encontre e expanda instâncias de recursos com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="dfc02-116">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="dfc02-117">Evento, evento de grupo, postagem de grupo, mensagem, contato pessoal</span><span class="sxs-lookup"><span data-stu-id="dfc02-117">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="dfc02-118">Instâncias de recursos expandidas com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="dfc02-118">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="dfc02-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfc02-119">Permissions</span></span>

<span data-ttu-id="dfc02-120">Dependendo do recurso que contém a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="dfc02-120">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="dfc02-121">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfc02-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfc02-122">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="dfc02-122">Supported resource</span></span> | <span data-ttu-id="dfc02-123">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfc02-123">Delegated (work or school account)</span></span> | <span data-ttu-id="dfc02-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfc02-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfc02-125">Application</span><span class="sxs-lookup"><span data-stu-id="dfc02-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="dfc02-126">device</span><span class="sxs-lookup"><span data-stu-id="dfc02-126">device</span></span>](../resources/device.md) | <span data-ttu-id="dfc02-127">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-127">Directory.Read.All</span></span> | <span data-ttu-id="dfc02-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc02-128">Not supported</span></span> | <span data-ttu-id="dfc02-129">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-129">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="dfc02-130">evento</span><span class="sxs-lookup"><span data-stu-id="dfc02-130">event</span></span>](../resources/event.md) | <span data-ttu-id="dfc02-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-131">Calendars.Read</span></span> | <span data-ttu-id="dfc02-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-132">Calendars.Read</span></span> | <span data-ttu-id="dfc02-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-133">Calendars.Read</span></span> |
| [<span data-ttu-id="dfc02-134">grupo</span><span class="sxs-lookup"><span data-stu-id="dfc02-134">group</span></span>](../resources/group.md) | <span data-ttu-id="dfc02-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-135">Group.Read.All</span></span> | <span data-ttu-id="dfc02-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc02-136">Not supported</span></span> | <span data-ttu-id="dfc02-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-137">Group.Read.All</span></span> |
| [<span data-ttu-id="dfc02-138">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="dfc02-138">group event</span></span>](../resources/event.md) | <span data-ttu-id="dfc02-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-139">Group.Read.All</span></span> | <span data-ttu-id="dfc02-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc02-140">Not supported</span></span> | <span data-ttu-id="dfc02-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc02-141">Not supported</span></span> |
| [<span data-ttu-id="dfc02-142">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="dfc02-142">group post</span></span>](../resources/post.md) | <span data-ttu-id="dfc02-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-143">Group.Read.All</span></span> | <span data-ttu-id="dfc02-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="dfc02-144">Not supported</span></span> | <span data-ttu-id="dfc02-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-145">Group.Read.All</span></span> |
| [<span data-ttu-id="dfc02-146">message</span><span class="sxs-lookup"><span data-stu-id="dfc02-146">message</span></span>](../resources/message.md) | <span data-ttu-id="dfc02-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-147">Mail.Read</span></span> | <span data-ttu-id="dfc02-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-148">Mail.Read</span></span> | <span data-ttu-id="dfc02-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-149">Mail.Read</span></span> | 
| [<span data-ttu-id="dfc02-150">organização</span><span class="sxs-lookup"><span data-stu-id="dfc02-150">organization</span></span>](../resources/organization.md) | <span data-ttu-id="dfc02-151">User.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-151">User.Read</span></span> | <span data-ttu-id="dfc02-152">Incompatível</span><span class="sxs-lookup"><span data-stu-id="dfc02-152">Not supported</span></span> | <span data-ttu-id="dfc02-153">Organization.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-153">Organization.Read.All</span></span> |
| [<span data-ttu-id="dfc02-154">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="dfc02-154">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="dfc02-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-155">Contacts.Read</span></span> | <span data-ttu-id="dfc02-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-156">Contacts.Read</span></span> | <span data-ttu-id="dfc02-157">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-157">Contacts.Read</span></span> |
| [<span data-ttu-id="dfc02-158">usuário</span><span class="sxs-lookup"><span data-stu-id="dfc02-158">user</span></span>](../resources/user.md) | <span data-ttu-id="dfc02-159">User.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-159">User.Read</span></span> | <span data-ttu-id="dfc02-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="dfc02-160">User.Read</span></span> | <span data-ttu-id="dfc02-161">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc02-161">User.Read.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="dfc02-162">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc02-162">HTTP request</span></span>

<span data-ttu-id="dfc02-163">Esta seção lista a sintaxe de cada um dos três cenários `GET` descritos acima</span><span class="sxs-lookup"><span data-stu-id="dfc02-163">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="dfc02-164">Obtenha uma extensão específica em uma instância de recurso conhecida</span><span class="sxs-lookup"><span data-stu-id="dfc02-164">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="dfc02-165">Use a mesma solicitação REST obtendo a instância do recurso e identifique a extensão usando a propriedade de navegação **extensions** dessa instância.</span><span class="sxs-lookup"><span data-stu-id="dfc02-165">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
```


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="dfc02-166">Obtenha uma instância de recurso conhecida, expandida com uma extensão correspondente.</span><span class="sxs-lookup"><span data-stu-id="dfc02-166">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="dfc02-167">Para os tipos de recurso de evento, evento de grupo, postagem de grupo, mensagem e contato pessoal, você pode usar a mesma solicitação REST e, enquanto obtém a instância de recurso, procure uma extensão que corresponda a um filtro em sua propriedade **id** e expanda a instância com a extensão.</span><span class="sxs-lookup"><span data-stu-id="dfc02-167">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension.</span></span> <span data-ttu-id="dfc02-168">A resposta inclui a maioria das propriedades do recurso.</span><span class="sxs-lookup"><span data-stu-id="dfc02-168">The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="dfc02-169">Para os tipos de recurso de dispositivo, grupo, organização e usuário, você também deve usar um parâmetro `$select` para incluir a propriedade **id** e quaisquer outras propriedades que você deseja na instância do recurso:</span><span class="sxs-lookup"><span data-stu-id="dfc02-169">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="dfc02-170">Filtrar as instâncias do recurso expandidas com uma extensão correspondente</span><span class="sxs-lookup"><span data-stu-id="dfc02-170">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="dfc02-171">Use a mesma solicitação REST para obter uma coleção do recurso suportado, filtre a coleção para instâncias que contêm uma extensão com uma propriedade **id** correspondente e expanda essas instâncias com a extensão.</span><span class="sxs-lookup"><span data-stu-id="dfc02-171">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="dfc02-172">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso ou coleção, para obter uma extensão dela.</span><span class="sxs-lookup"><span data-stu-id="dfc02-172">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it.</span></span> <span data-ttu-id="dfc02-173">Todas as outras sintaxes que permitem identificar essas instâncias de recursos ou coleções dão suporte à obtenção de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="dfc02-173">All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="dfc02-174">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="dfc02-174">Path parameters</span></span>
|<span data-ttu-id="dfc02-175">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dfc02-175">Parameter</span></span>|<span data-ttu-id="dfc02-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfc02-176">Type</span></span>|<span data-ttu-id="dfc02-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfc02-177">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dfc02-178">Id</span><span class="sxs-lookup"><span data-stu-id="dfc02-178">Id</span></span>|<span data-ttu-id="dfc02-179">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfc02-179">string</span></span>|<span data-ttu-id="dfc02-p104">Espaço reservado para um identificador exclusivo de um objeto na coleção correspondente, como mensagens, contatos e eventos. Obrigatório. Não deve ser confundido com a propriedade **id** de uma **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="dfc02-183">extensionId</span><span class="sxs-lookup"><span data-stu-id="dfc02-183">extensionId</span></span>|<span data-ttu-id="dfc02-184">string</span><span class="sxs-lookup"><span data-stu-id="dfc02-184">string</span></span>|<span data-ttu-id="dfc02-p105">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para um a uma extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade **id** quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="dfc02-188">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dfc02-188">Optional query parameters</span></span>

<span data-ttu-id="dfc02-189">Verifique se aplicou a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de caracteres `$filter`.</span><span class="sxs-lookup"><span data-stu-id="dfc02-189">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="dfc02-190">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dfc02-190">Parameter</span></span>|<span data-ttu-id="dfc02-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfc02-191">Description</span></span>|<span data-ttu-id="dfc02-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfc02-192">Example</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="dfc02-193">$filter</span><span class="sxs-lookup"><span data-stu-id="dfc02-193">$filter</span></span>|<span data-ttu-id="dfc02-194">Retorna uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="dfc02-194">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="dfc02-195">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="dfc02-195">Request 3</span></span>](#request-3)|
|<span data-ttu-id="dfc02-196">$filter com o operador **any**</span><span class="sxs-lookup"><span data-stu-id="dfc02-196">$filter with **any** operator</span></span>|<span data-ttu-id="dfc02-197">Retorna instâncias de uma coleção de recursos que contêm uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="dfc02-197">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="dfc02-198">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="dfc02-198">Request 5</span></span>](#request-5)|
|<span data-ttu-id="dfc02-199">$expand</span><span class="sxs-lookup"><span data-stu-id="dfc02-199">$expand</span></span>|<span data-ttu-id="dfc02-200">Expande uma instância de recurso para incluir uma extensão.</span><span class="sxs-lookup"><span data-stu-id="dfc02-200">Expands a resource instance to include an extension.</span></span> |<span data-ttu-id="dfc02-201">[Solicitação 3](#request-3) e [solicitação 5](#request-5)</span><span class="sxs-lookup"><span data-stu-id="dfc02-201">[Request 3](#request-3) and [request 5](#request-5)</span></span>|

## <a name="request-headers"></a><span data-ttu-id="dfc02-202">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc02-202">Request headers</span></span>
| <span data-ttu-id="dfc02-203">Nome</span><span class="sxs-lookup"><span data-stu-id="dfc02-203">Name</span></span>       | <span data-ttu-id="dfc02-204">Valor</span><span class="sxs-lookup"><span data-stu-id="dfc02-204">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="dfc02-205">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfc02-205">Authorization</span></span> | <span data-ttu-id="dfc02-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfc02-208">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc02-208">Request body</span></span>
<span data-ttu-id="dfc02-209">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfc02-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfc02-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc02-210">Response</span></span>

<span data-ttu-id="dfc02-p107">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [openTypeExtension](../resources/opentypeextension.md) no corpo da resposta. Dependendo da consulta GET, o corpo da resposta exato pode ser diferente.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="dfc02-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfc02-213">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="dfc02-214">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="dfc02-214">Request 1</span></span>

<span data-ttu-id="dfc02-p108">O primeiro exemplo mostra 2 maneiras de referenciar uma extensão e obtém a extensão na mensagem especificada. A resposta é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="dfc02-217">Em primeiro lugar, por nome:</span><span class="sxs-lookup"><span data-stu-id="dfc02-217">First, by its name:</span></span> 


# <a name="http"></a>[<span data-ttu-id="dfc02-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc02-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="dfc02-219">C#</span><span class="sxs-lookup"><span data-stu-id="dfc02-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfc02-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfc02-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfc02-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfc02-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfc02-222">Java</span><span class="sxs-lookup"><span data-stu-id="dfc02-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="dfc02-223">Em segundo lugar, por ID (nome totalmente qualificado):</span><span class="sxs-lookup"><span data-stu-id="dfc02-223">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

#### <a name="response-1"></a><span data-ttu-id="dfc02-224">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="dfc02-224">Response 1</span></span>
<span data-ttu-id="dfc02-225">Veja a seguir a resposta para o primeiro exemplo.</span><span class="sxs-lookup"><span data-stu-id="dfc02-225">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="dfc02-226">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="dfc02-226">Request 2</span></span>

<span data-ttu-id="dfc02-227">O segundo exemplo faz referência a uma extensão por nome e obtém essa extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="dfc02-227">The second example references an extension by its name and gets the extension in the specified group event.</span></span>


# <a name="http"></a>[<span data-ttu-id="dfc02-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc02-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Deal", "f5480dfd-7d77-4d0b-ba2e-3391953cc74a", "AAMkADVl17IsAAA="],
  "name": "get_opentypeextension_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/
```
# <a name="c"></a>[<span data-ttu-id="dfc02-229">C#</span><span class="sxs-lookup"><span data-stu-id="dfc02-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfc02-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfc02-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfc02-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfc02-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfc02-232">Java</span><span class="sxs-lookup"><span data-stu-id="dfc02-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="dfc02-233">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="dfc02-233">Response 2</span></span>

<span data-ttu-id="dfc02-234">Veja a seguir a resposta do segundo exemplo.</span><span class="sxs-lookup"><span data-stu-id="dfc02-234">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="dfc02-235">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="dfc02-235">Request 3</span></span>

<span data-ttu-id="dfc02-p109">O terceiro exemplo obtém e expande a mensagem especificada, incluindo a extensão retornada de um filtro. O filtro retorna a extensão cujo **id** corresponde a um nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>


# <a name="http"></a>[<span data-ttu-id="dfc02-238">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc02-238">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```
# <a name="c"></a>[<span data-ttu-id="dfc02-239">C#</span><span class="sxs-lookup"><span data-stu-id="dfc02-239">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfc02-240">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfc02-240">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfc02-241">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfc02-241">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfc02-242">Java</span><span class="sxs-lookup"><span data-stu-id="dfc02-242">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response-3"></a><span data-ttu-id="dfc02-243">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="dfc02-243">Response 3</span></span>

<span data-ttu-id="dfc02-p110">Veja a seguir a resposta do terceiro exemplo. Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
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
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
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

#### <a name="request-4"></a><span data-ttu-id="dfc02-247">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="dfc02-247">Request 4</span></span>

<span data-ttu-id="dfc02-248">O quarto exemplo faz referência a uma extensão por nome totalmente qualificado e obtém essa extensão na postagem de grupo especificada.</span><span class="sxs-lookup"><span data-stu-id="dfc02-248">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```

#### <a name="response-4"></a><span data-ttu-id="dfc02-249">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="dfc02-249">Response 4</span></span>

<span data-ttu-id="dfc02-250">Veja a seguir a resposta do quarto exemplo.</span><span class="sxs-lookup"><span data-stu-id="dfc02-250">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
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


#### <a name="request-5"></a><span data-ttu-id="dfc02-251">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="dfc02-251">Request 5</span></span>

<span data-ttu-id="dfc02-p111">O quinto exemplo analisa todas as mensagens na caixa de correio do usuário conectado para localizar aquelas uma contêm uma extensão correspondente a um filtro e as expande com a inclusão dessa extensão. O filtro retorna extensões cuja propriedade **id** corresponde ao nome da extensão `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


#### <a name="response-5"></a><span data-ttu-id="dfc02-254">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="dfc02-254">Response 5</span></span>

<span data-ttu-id="dfc02-255">Nessa resposta do quinto exemplo, há apenas uma mensagem na caixa de correio do usuário que tem uma extensão cuja **id** é igual a `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="dfc02-255">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="dfc02-p112">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfc02-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
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
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

