---
title: Obter extensão aberta
description: Obtenha uma extensão aberta (objeto openTypeExtension) identificada por nome ou nome totalmente qualificado.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 0ac9dac1b7e5cb4267cba07c174fd8e277af0dab
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864039"
---
# <a name="get-open-extension"></a><span data-ttu-id="f70a4-103">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="f70a4-103">Get open extension</span></span>

<span data-ttu-id="f70a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f70a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f70a4-105">Obtenha uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) identificada por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="f70a4-105">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="f70a4-106">A tabela a seguir lista os três cenários em que é possível obter uma extensão aberta de uma instância de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="f70a4-106">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="f70a4-107">**Cenário GET**</span><span class="sxs-lookup"><span data-stu-id="f70a4-107">**GET scenario**</span></span>|<span data-ttu-id="f70a4-108">**Recursos com suporte**</span><span class="sxs-lookup"><span data-stu-id="f70a4-108">**Supported resources**</span></span>|<span data-ttu-id="f70a4-109">**Corpo da resposta**</span><span class="sxs-lookup"><span data-stu-id="f70a4-109">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f70a4-110">Obtenha uma extensão específica de uma instância de recurso conhecida.</span><span class="sxs-lookup"><span data-stu-id="f70a4-110">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="f70a4-111">[Dispositivo](../resources/device.md), [evento](../resources/event.md), [grupo](../resources/group.md), [evento de grupo](../resources/event.md), [postagem de grupo](../resources/post.md), [mensagem](../resources/message.md), [organização](../resources/organization.md), [contato pessoal](../resources/contact.md), [usuário](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="f70a4-111">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="f70a4-112">Somente extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="f70a4-112">Open extension only.</span></span>|
|<span data-ttu-id="f70a4-113">Obtenha uma instância de recurso conhecida, expandida com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="f70a4-113">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="f70a4-114">Dispositivo, evento, grupo, evento de grupo, postagem de grupo, mensagem, organização, contato pessoal, usuário</span><span class="sxs-lookup"><span data-stu-id="f70a4-114">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="f70a4-115">Uma instância de recurso expandida com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="f70a4-115">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="f70a4-116">Encontre e expanda instâncias de recursos com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="f70a4-116">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="f70a4-117">Evento, evento de grupo, postagem de grupo, mensagem, contato pessoal</span><span class="sxs-lookup"><span data-stu-id="f70a4-117">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="f70a4-118">Instâncias de recursos expandidas com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="f70a4-118">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="f70a4-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="f70a4-119">Permissions</span></span>

<span data-ttu-id="f70a4-120">Dependendo do recurso que contém a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="f70a4-120">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="f70a4-121">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f70a4-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f70a4-122">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="f70a4-122">Supported resource</span></span> | <span data-ttu-id="f70a4-123">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f70a4-123">Delegated (work or school account)</span></span> | <span data-ttu-id="f70a4-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f70a4-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f70a4-125">Application</span><span class="sxs-lookup"><span data-stu-id="f70a4-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="f70a4-126">device</span><span class="sxs-lookup"><span data-stu-id="f70a4-126">device</span></span>](../resources/device.md) | <span data-ttu-id="f70a4-127">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-127">Directory.Read.All</span></span> | <span data-ttu-id="f70a4-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f70a4-128">Not supported</span></span> | <span data-ttu-id="f70a4-129">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-129">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="f70a4-130">evento</span><span class="sxs-lookup"><span data-stu-id="f70a4-130">event</span></span>](../resources/event.md) | <span data-ttu-id="f70a4-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-131">Calendars.Read</span></span> | <span data-ttu-id="f70a4-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-132">Calendars.Read</span></span> | <span data-ttu-id="f70a4-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-133">Calendars.Read</span></span> |
| [<span data-ttu-id="f70a4-134">grupo</span><span class="sxs-lookup"><span data-stu-id="f70a4-134">group</span></span>](../resources/group.md) | <span data-ttu-id="f70a4-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-135">Group.Read.All</span></span> | <span data-ttu-id="f70a4-136">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f70a4-136">Not supported</span></span> | <span data-ttu-id="f70a4-137">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-137">Group.Read.All</span></span> |
| [<span data-ttu-id="f70a4-138">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="f70a4-138">group event</span></span>](../resources/event.md) | <span data-ttu-id="f70a4-139">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-139">Group.Read.All</span></span> | <span data-ttu-id="f70a4-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f70a4-140">Not supported</span></span> | <span data-ttu-id="f70a4-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f70a4-141">Not supported</span></span> |
| [<span data-ttu-id="f70a4-142">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="f70a4-142">group post</span></span>](../resources/post.md) | <span data-ttu-id="f70a4-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-143">Group.Read.All</span></span> | <span data-ttu-id="f70a4-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f70a4-144">Not supported</span></span> | <span data-ttu-id="f70a4-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-145">Group.Read.All</span></span> |
| [<span data-ttu-id="f70a4-146">message</span><span class="sxs-lookup"><span data-stu-id="f70a4-146">message</span></span>](../resources/message.md) | <span data-ttu-id="f70a4-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-147">Mail.Read</span></span> | <span data-ttu-id="f70a4-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-148">Mail.Read</span></span> | <span data-ttu-id="f70a4-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-149">Mail.Read</span></span> | 
| [<span data-ttu-id="f70a4-150">organização</span><span class="sxs-lookup"><span data-stu-id="f70a4-150">organization</span></span>](../resources/organization.md) | <span data-ttu-id="f70a4-151">User.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-151">User.Read</span></span> | <span data-ttu-id="f70a4-152">Incompatível</span><span class="sxs-lookup"><span data-stu-id="f70a4-152">Not supported</span></span> | <span data-ttu-id="f70a4-153">Organization.Read.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-153">Organization.Read.All</span></span> |
| [<span data-ttu-id="f70a4-154">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="f70a4-154">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="f70a4-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-155">Contacts.Read</span></span> | <span data-ttu-id="f70a4-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-156">Contacts.Read</span></span> | <span data-ttu-id="f70a4-157">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-157">Contacts.Read</span></span> |
| [<span data-ttu-id="f70a4-158">usuário</span><span class="sxs-lookup"><span data-stu-id="f70a4-158">user</span></span>](../resources/user.md) | <span data-ttu-id="f70a4-159">User.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-159">User.Read</span></span> | <span data-ttu-id="f70a4-160">User.Read</span><span class="sxs-lookup"><span data-stu-id="f70a4-160">User.Read</span></span> | <span data-ttu-id="f70a4-161">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f70a4-161">User.Read.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="f70a4-162">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f70a4-162">HTTP request</span></span>

<span data-ttu-id="f70a4-163">Esta seção lista a sintaxe de cada um dos três cenários `GET` descritos acima</span><span class="sxs-lookup"><span data-stu-id="f70a4-163">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="f70a4-164">Obtenha uma extensão específica em uma instância de recurso conhecida</span><span class="sxs-lookup"><span data-stu-id="f70a4-164">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="f70a4-165">Use a mesma solicitação REST obtendo a instância do recurso e identifique a extensão usando a propriedade de navegação **extensions** dessa instância.</span><span class="sxs-lookup"><span data-stu-id="f70a4-165">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

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


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="f70a4-166">Obtenha uma instância de recurso conhecida, expandida com uma extensão correspondente.</span><span class="sxs-lookup"><span data-stu-id="f70a4-166">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="f70a4-167">Para os tipos de recurso de evento, evento de grupo, postagem de grupo, mensagem e contato pessoal, você pode usar a mesma solicitação REST e, enquanto obtém a instância de recurso, procure uma extensão que corresponda a um filtro em sua propriedade **id** e expanda a instância com a extensão.</span><span class="sxs-lookup"><span data-stu-id="f70a4-167">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension.</span></span> <span data-ttu-id="f70a4-168">A resposta inclui a maioria das propriedades do recurso.</span><span class="sxs-lookup"><span data-stu-id="f70a4-168">The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="f70a4-169">Para os tipos de recurso de dispositivo, grupo, organização e usuário, você também deve usar um parâmetro `$select` para incluir a propriedade **id** e quaisquer outras propriedades que você deseja na instância do recurso:</span><span class="sxs-lookup"><span data-stu-id="f70a4-169">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="f70a4-170">Filtrar as instâncias do recurso expandidas com uma extensão correspondente</span><span class="sxs-lookup"><span data-stu-id="f70a4-170">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="f70a4-171">Use a mesma solicitação REST para obter uma coleção do recurso suportado, filtre a coleção para instâncias que contêm uma extensão com uma propriedade **id** correspondente e expanda essas instâncias com a extensão.</span><span class="sxs-lookup"><span data-stu-id="f70a4-171">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="f70a4-172">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso ou coleção, para obter uma extensão dela.</span><span class="sxs-lookup"><span data-stu-id="f70a4-172">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it.</span></span> <span data-ttu-id="f70a4-173">Todas as outras sintaxes que permitem identificar essas instâncias de recursos ou coleções dão suporte à obtenção de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="f70a4-173">All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="f70a4-174">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="f70a4-174">Path parameters</span></span>
|<span data-ttu-id="f70a4-175">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f70a4-175">Parameter</span></span>|<span data-ttu-id="f70a4-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="f70a4-176">Type</span></span>|<span data-ttu-id="f70a4-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="f70a4-177">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f70a4-178">Id</span><span class="sxs-lookup"><span data-stu-id="f70a4-178">Id</span></span>|<span data-ttu-id="f70a4-179">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f70a4-179">string</span></span>|<span data-ttu-id="f70a4-180">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts.</span><span class="sxs-lookup"><span data-stu-id="f70a4-180">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts.</span></span> <span data-ttu-id="f70a4-181">Required.</span><span class="sxs-lookup"><span data-stu-id="f70a4-181">Required.</span></span> <span data-ttu-id="f70a4-182">Not to be confused with the **id** property of an **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="f70a4-182">Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="f70a4-183">extensionId</span><span class="sxs-lookup"><span data-stu-id="f70a4-183">extensionId</span></span>|<span data-ttu-id="f70a4-184">string</span><span class="sxs-lookup"><span data-stu-id="f70a4-184">string</span></span>|<span data-ttu-id="f70a4-185">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier.</span><span class="sxs-lookup"><span data-stu-id="f70a4-185">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier.</span></span> <span data-ttu-id="f70a4-186">The fully qualified name is returned in the **id** property when you create the extension.</span><span class="sxs-lookup"><span data-stu-id="f70a4-186">The fully qualified name is returned in the **id** property when you create the extension.</span></span> <span data-ttu-id="f70a4-187">Required.</span><span class="sxs-lookup"><span data-stu-id="f70a4-187">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="f70a4-188">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f70a4-188">Optional query parameters</span></span>

<span data-ttu-id="f70a4-189">Verifique se aplicou a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de caracteres `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f70a4-189">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="f70a4-190">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f70a4-190">Parameter</span></span>|<span data-ttu-id="f70a4-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="f70a4-191">Description</span></span>|<span data-ttu-id="f70a4-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f70a4-192">Example</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="f70a4-193">$filter</span><span class="sxs-lookup"><span data-stu-id="f70a4-193">$filter</span></span>|<span data-ttu-id="f70a4-194">Retorna uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="f70a4-194">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="f70a4-195">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="f70a4-195">Request 3</span></span>](#request-3)|
|<span data-ttu-id="f70a4-196">$filter com o operador **any**</span><span class="sxs-lookup"><span data-stu-id="f70a4-196">$filter with **any** operator</span></span>|<span data-ttu-id="f70a4-197">Retorna instâncias de uma coleção de recursos que contêm uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="f70a4-197">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="f70a4-198">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="f70a4-198">Request 5</span></span>](#request-5)|
|<span data-ttu-id="f70a4-199">$expand</span><span class="sxs-lookup"><span data-stu-id="f70a4-199">$expand</span></span>|<span data-ttu-id="f70a4-200">Expande uma instância de recurso para incluir uma extensão.</span><span class="sxs-lookup"><span data-stu-id="f70a4-200">Expands a resource instance to include an extension.</span></span> |<span data-ttu-id="f70a4-201">[Solicitação 3](#request-3) e [solicitação 5](#request-5)</span><span class="sxs-lookup"><span data-stu-id="f70a4-201">[Request 3](#request-3) and [request 5](#request-5)</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f70a4-202">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f70a4-202">Request headers</span></span>
| <span data-ttu-id="f70a4-203">Nome</span><span class="sxs-lookup"><span data-stu-id="f70a4-203">Name</span></span>       | <span data-ttu-id="f70a4-204">Valor</span><span class="sxs-lookup"><span data-stu-id="f70a4-204">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f70a4-205">Autorização</span><span class="sxs-lookup"><span data-stu-id="f70a4-205">Authorization</span></span> | <span data-ttu-id="f70a4-206">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f70a4-206">Bearer {token}.</span></span> <span data-ttu-id="f70a4-207">Required.</span><span class="sxs-lookup"><span data-stu-id="f70a4-207">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f70a4-208">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f70a4-208">Request body</span></span>
<span data-ttu-id="f70a4-209">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f70a4-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f70a4-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="f70a4-210">Response</span></span>

<span data-ttu-id="f70a4-211">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body.</span><span class="sxs-lookup"><span data-stu-id="f70a4-211">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body.</span></span>
<span data-ttu-id="f70a4-212">Depending on the GET query, the exact response body differs.</span><span class="sxs-lookup"><span data-stu-id="f70a4-212">Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="f70a4-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f70a4-213">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="f70a4-214">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="f70a4-214">Request 1</span></span>

<span data-ttu-id="f70a4-215">The first example shows 2 ways of referencing an extension and gets the extension in the specified message.</span><span class="sxs-lookup"><span data-stu-id="f70a4-215">The first example shows 2 ways of referencing an extension and gets the extension in the specified message.</span></span> <span data-ttu-id="f70a4-216">The response is the same regardless of the way used to reference the extension.</span><span class="sxs-lookup"><span data-stu-id="f70a4-216">The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="f70a4-217">Em primeiro lugar, por nome:</span><span class="sxs-lookup"><span data-stu-id="f70a4-217">First, by its name:</span></span> 


# <a name="http"></a>[<span data-ttu-id="f70a4-218">HTTP</span><span class="sxs-lookup"><span data-stu-id="f70a4-218">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="f70a4-219">C#</span><span class="sxs-lookup"><span data-stu-id="f70a4-219">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f70a4-220">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f70a4-220">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f70a4-221">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f70a4-221">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f70a4-222">Java</span><span class="sxs-lookup"><span data-stu-id="f70a4-222">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="f70a4-223">Em segundo lugar, por ID (nome totalmente qualificado):</span><span class="sxs-lookup"><span data-stu-id="f70a4-223">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

#### <a name="response-1"></a><span data-ttu-id="f70a4-224">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="f70a4-224">Response 1</span></span>
<span data-ttu-id="f70a4-225">Veja a seguir a resposta para o primeiro exemplo.</span><span class="sxs-lookup"><span data-stu-id="f70a4-225">Here is the response for the first example.</span></span>
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


#### <a name="request-2"></a><span data-ttu-id="f70a4-226">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="f70a4-226">Request 2</span></span>

<span data-ttu-id="f70a4-227">O segundo exemplo faz referência a uma extensão por nome e obtém essa extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="f70a4-227">The second example references an extension by its name and gets the extension in the specified group event.</span></span>


# <a name="http"></a>[<span data-ttu-id="f70a4-228">HTTP</span><span class="sxs-lookup"><span data-stu-id="f70a4-228">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Deal", "f5480dfd-7d77-4d0b-ba2e-3391953cc74a", "AAMkADVl17IsAAA="],
  "name": "get_opentypeextension_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/
```
# <a name="c"></a>[<span data-ttu-id="f70a4-229">C#</span><span class="sxs-lookup"><span data-stu-id="f70a4-229">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f70a4-230">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f70a4-230">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f70a4-231">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f70a4-231">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f70a4-232">Java</span><span class="sxs-lookup"><span data-stu-id="f70a4-232">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="f70a4-233">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="f70a4-233">Response 2</span></span>

<span data-ttu-id="f70a4-234">Veja a seguir a resposta do segundo exemplo.</span><span class="sxs-lookup"><span data-stu-id="f70a4-234">Here is the response from the second example.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="f70a4-235">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="f70a4-235">Request 3</span></span>

<span data-ttu-id="f70a4-236">The third example gets and expands the specified message by including the extension returned from a filter.</span><span class="sxs-lookup"><span data-stu-id="f70a4-236">The third example gets and expands the specified message by including the extension returned from a filter.</span></span> <span data-ttu-id="f70a4-237">The filter returns the extension that has its **id** matching a fully qualified name.</span><span class="sxs-lookup"><span data-stu-id="f70a4-237">The filter returns the extension that has its **id** matching a fully qualified name.</span></span>


# <a name="http"></a>[<span data-ttu-id="f70a4-238">HTTP</span><span class="sxs-lookup"><span data-stu-id="f70a4-238">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```
# <a name="c"></a>[<span data-ttu-id="f70a4-239">C#</span><span class="sxs-lookup"><span data-stu-id="f70a4-239">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f70a4-240">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f70a4-240">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f70a4-241">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f70a4-241">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f70a4-242">Java</span><span class="sxs-lookup"><span data-stu-id="f70a4-242">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response-3"></a><span data-ttu-id="f70a4-243">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="f70a4-243">Response 3</span></span>

<span data-ttu-id="f70a4-244">And here is the response from the third example.</span><span class="sxs-lookup"><span data-stu-id="f70a4-244">And here is the response from the third example.</span></span> <span data-ttu-id="f70a4-245">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f70a4-245">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f70a4-246">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f70a4-246">All of the properties will be returned from an actual call.</span></span>

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

#### <a name="request-4"></a><span data-ttu-id="f70a4-247">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="f70a4-247">Request 4</span></span>

<span data-ttu-id="f70a4-248">O quarto exemplo faz referência a uma extensão por nome totalmente qualificado e obtém essa extensão na postagem de grupo especificada.</span><span class="sxs-lookup"><span data-stu-id="f70a4-248">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```

#### <a name="response-4"></a><span data-ttu-id="f70a4-249">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="f70a4-249">Response 4</span></span>

<span data-ttu-id="f70a4-250">Veja a seguir a resposta do quarto exemplo.</span><span class="sxs-lookup"><span data-stu-id="f70a4-250">Here is the response from the fourth example.</span></span> 

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


#### <a name="request-5"></a><span data-ttu-id="f70a4-251">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="f70a4-251">Request 5</span></span>

<span data-ttu-id="f70a4-252">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension.</span><span class="sxs-lookup"><span data-stu-id="f70a4-252">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension.</span></span> <span data-ttu-id="f70a4-253">The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="f70a4-253">The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


#### <a name="response-5"></a><span data-ttu-id="f70a4-254">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="f70a4-254">Response 5</span></span>

<span data-ttu-id="f70a4-255">Nessa resposta do quinto exemplo, há apenas uma mensagem na caixa de correio do usuário que tem uma extensão cuja **id** é igual a `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="f70a4-255">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="f70a4-256">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f70a4-256">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f70a4-257">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f70a4-257">All of the properties will be returned from an actual call.</span></span>

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
