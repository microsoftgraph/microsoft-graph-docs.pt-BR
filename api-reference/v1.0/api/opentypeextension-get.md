---
title: Obter extensão aberta
description: Obtenha uma extensão aberta (objeto openTypeExtension) identificada por nome ou nome totalmente qualificado.
localization_priority: Priority
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 0678c741172d34d6558aa56724378d18811432ee
ms.sourcegitcommit: 0f39f39a1c0300ef013ebd12e4df2b5ba4dabbf8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2020
ms.locfileid: "41558778"
---
# <a name="get-open-extension"></a><span data-ttu-id="c62d9-103">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="c62d9-103">Get open extension</span></span>

<span data-ttu-id="c62d9-104">Obtenha uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) identificada por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="c62d9-104">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="c62d9-105">A tabela a seguir lista os três cenários em que é possível obter uma extensão aberta de uma instância de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="c62d9-105">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="c62d9-106">**Cenário GET**</span><span class="sxs-lookup"><span data-stu-id="c62d9-106">**GET scenario**</span></span>|<span data-ttu-id="c62d9-107">**Recursos com suporte**</span><span class="sxs-lookup"><span data-stu-id="c62d9-107">**Supported resources**</span></span>|<span data-ttu-id="c62d9-108">**Corpo da resposta**</span><span class="sxs-lookup"><span data-stu-id="c62d9-108">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c62d9-109">Obtenha uma extensão específica de uma instância de recurso conhecida.</span><span class="sxs-lookup"><span data-stu-id="c62d9-109">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="c62d9-110">[Dispositivo](../resources/device.md), [evento](../resources/event.md), [grupo](../resources/group.md), [evento de grupo](../resources/event.md), [postagem de grupo](../resources/post.md), [mensagem](../resources/message.md), [organização](../resources/organization.md), [contato pessoal](../resources/contact.md), [usuário](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="c62d9-110">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="c62d9-111">Somente extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="c62d9-111">Open extension only.</span></span>|
|<span data-ttu-id="c62d9-112">Obtenha uma instância de recurso conhecida, expandida com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="c62d9-112">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="c62d9-113">Dispositivo, evento, grupo, evento de grupo, postagem de grupo, mensagem, organização, contato pessoal, usuário</span><span class="sxs-lookup"><span data-stu-id="c62d9-113">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="c62d9-114">Uma instância de recurso expandida com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="c62d9-114">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="c62d9-115">Encontre e expanda instâncias de recursos com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="c62d9-115">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="c62d9-116">Evento, evento de grupo, postagem de grupo, mensagem, contato pessoal</span><span class="sxs-lookup"><span data-stu-id="c62d9-116">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="c62d9-117">Instâncias de recursos expandidas com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="c62d9-117">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="c62d9-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="c62d9-118">Permissions</span></span>

<span data-ttu-id="c62d9-119">Dependendo do recurso que contém a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para fazer chamadas a esta API.</span><span class="sxs-lookup"><span data-stu-id="c62d9-119">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c62d9-120">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c62d9-120">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c62d9-121">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="c62d9-121">Supported resource</span></span> | <span data-ttu-id="c62d9-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c62d9-122">Delegated (work or school account)</span></span> | <span data-ttu-id="c62d9-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c62d9-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c62d9-124">Application</span><span class="sxs-lookup"><span data-stu-id="c62d9-124">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="c62d9-125">device</span><span class="sxs-lookup"><span data-stu-id="c62d9-125">device</span></span>](../resources/device.md) | <span data-ttu-id="c62d9-126">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62d9-126">Directory.Read.All</span></span> | <span data-ttu-id="c62d9-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c62d9-127">Not supported</span></span> | <span data-ttu-id="c62d9-128">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c62d9-128">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="c62d9-129">evento</span><span class="sxs-lookup"><span data-stu-id="c62d9-129">event</span></span>](../resources/event.md) | <span data-ttu-id="c62d9-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-130">Calendars.Read</span></span> | <span data-ttu-id="c62d9-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-131">Calendars.Read</span></span> | <span data-ttu-id="c62d9-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-132">Calendars.Read</span></span> |
| [<span data-ttu-id="c62d9-133">grupo</span><span class="sxs-lookup"><span data-stu-id="c62d9-133">group</span></span>](../resources/group.md) | <span data-ttu-id="c62d9-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62d9-134">Group.Read.All</span></span> | <span data-ttu-id="c62d9-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c62d9-135">Not supported</span></span> | <span data-ttu-id="c62d9-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62d9-136">Group.Read.All</span></span> |
| [<span data-ttu-id="c62d9-137">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="c62d9-137">group event</span></span>](../resources/event.md) | <span data-ttu-id="c62d9-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62d9-138">Group.Read.All</span></span> | <span data-ttu-id="c62d9-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c62d9-139">Not supported</span></span> | <span data-ttu-id="c62d9-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c62d9-140">Not supported</span></span> |
| [<span data-ttu-id="c62d9-141">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="c62d9-141">group post</span></span>](../resources/post.md) | <span data-ttu-id="c62d9-142">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62d9-142">Group.Read.All</span></span> | <span data-ttu-id="c62d9-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c62d9-143">Not supported</span></span> | <span data-ttu-id="c62d9-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62d9-144">Group.Read.All</span></span> |
| [<span data-ttu-id="c62d9-145">message</span><span class="sxs-lookup"><span data-stu-id="c62d9-145">message</span></span>](../resources/message.md) | <span data-ttu-id="c62d9-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-146">Mail.Read</span></span> | <span data-ttu-id="c62d9-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-147">Mail.Read</span></span> | <span data-ttu-id="c62d9-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-148">Mail.Read</span></span> | 
| [<span data-ttu-id="c62d9-149">organização</span><span class="sxs-lookup"><span data-stu-id="c62d9-149">organization</span></span>](../resources/organization.md) | <span data-ttu-id="c62d9-150">User.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-150">User.Read</span></span> | <span data-ttu-id="c62d9-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c62d9-151">Not supported</span></span> | <span data-ttu-id="c62d9-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="c62d9-152">Not supported</span></span> |
| [<span data-ttu-id="c62d9-153">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="c62d9-153">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="c62d9-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-154">Contacts.Read</span></span> | <span data-ttu-id="c62d9-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-155">Contacts.Read</span></span> | <span data-ttu-id="c62d9-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-156">Contacts.Read</span></span> |
| [<span data-ttu-id="c62d9-157">usuário</span><span class="sxs-lookup"><span data-stu-id="c62d9-157">user</span></span>](../resources/user.md) | <span data-ttu-id="c62d9-158">User.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-158">User.Read</span></span> | <span data-ttu-id="c62d9-159">User.Read</span><span class="sxs-lookup"><span data-stu-id="c62d9-159">User.Read</span></span> | <span data-ttu-id="c62d9-160">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c62d9-160">User.Read.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="c62d9-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c62d9-161">HTTP request</span></span>

<span data-ttu-id="c62d9-162">Esta seção lista a sintaxe de cada um dos três cenários `GET` descritos acima</span><span class="sxs-lookup"><span data-stu-id="c62d9-162">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="c62d9-163">Obtenha uma extensão específica em uma instância de recurso conhecida</span><span class="sxs-lookup"><span data-stu-id="c62d9-163">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="c62d9-164">Use a mesma solicitação REST obtendo a instância do recurso e identifique a extensão usando a propriedade de navegação **extensions** dessa instância.</span><span class="sxs-lookup"><span data-stu-id="c62d9-164">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

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


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="c62d9-165">Obtenha uma instância de recurso conhecida, expandida com uma extensão correspondente.</span><span class="sxs-lookup"><span data-stu-id="c62d9-165">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="c62d9-166">Para os tipos de recurso de evento, evento de grupo, postagem de grupo, mensagem e contato pessoal, você pode usar a mesma solicitação REST e, enquanto obtém a instância de recurso, procure uma extensão que corresponda a um filtro em sua propriedade **id** e expanda a instância com a extensão.</span><span class="sxs-lookup"><span data-stu-id="c62d9-166">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension.</span></span> <span data-ttu-id="c62d9-167">A resposta inclui a maioria das propriedades do recurso.</span><span class="sxs-lookup"><span data-stu-id="c62d9-167">The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="c62d9-168">Para os tipos de recurso de dispositivo, grupo, organização e usuário, você também deve usar um parâmetro `$select` para incluir a propriedade **id** e quaisquer outras propriedades que você deseja na instância do recurso:</span><span class="sxs-lookup"><span data-stu-id="c62d9-168">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="c62d9-169">Filtrar as instâncias do recurso expandidas com uma extensão correspondente</span><span class="sxs-lookup"><span data-stu-id="c62d9-169">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="c62d9-170">Use a mesma solicitação REST para obter uma coleção do recurso suportado, filtre a coleção para instâncias que contêm uma extensão com uma propriedade **id** correspondente e expanda essas instâncias com a extensão.</span><span class="sxs-lookup"><span data-stu-id="c62d9-170">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="c62d9-171">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso ou coleção, para obter uma extensão dela.</span><span class="sxs-lookup"><span data-stu-id="c62d9-171">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it.</span></span> <span data-ttu-id="c62d9-172">Todas as outras sintaxes que permitem identificar essas instâncias de recursos ou coleções dão suporte à obtenção de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="c62d9-172">All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="c62d9-173">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="c62d9-173">Path parameters</span></span>
|<span data-ttu-id="c62d9-174">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c62d9-174">Parameter</span></span>|<span data-ttu-id="c62d9-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="c62d9-175">Type</span></span>|<span data-ttu-id="c62d9-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="c62d9-176">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c62d9-177">Id</span><span class="sxs-lookup"><span data-stu-id="c62d9-177">Id</span></span>|<span data-ttu-id="c62d9-178">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c62d9-178">string</span></span>|<span data-ttu-id="c62d9-p104">Espaço reservado para um identificador exclusivo de um objeto na coleção correspondente, como mensagens, contatos e eventos. Obrigatório. Não deve ser confundido com a propriedade **id** de uma **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="c62d9-182">extensionId</span><span class="sxs-lookup"><span data-stu-id="c62d9-182">extensionId</span></span>|<span data-ttu-id="c62d9-183">string</span><span class="sxs-lookup"><span data-stu-id="c62d9-183">string</span></span>|<span data-ttu-id="c62d9-p105">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para um a uma extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade **id** quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="c62d9-187">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c62d9-187">Optional query parameters</span></span>

<span data-ttu-id="c62d9-188">Verifique se aplicou a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de caracteres `$filter`.</span><span class="sxs-lookup"><span data-stu-id="c62d9-188">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="c62d9-189">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c62d9-189">Parameter</span></span>|<span data-ttu-id="c62d9-190">Descrição</span><span class="sxs-lookup"><span data-stu-id="c62d9-190">Description</span></span>|<span data-ttu-id="c62d9-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c62d9-191">Example</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="c62d9-192">$filter</span><span class="sxs-lookup"><span data-stu-id="c62d9-192">$filter</span></span>|<span data-ttu-id="c62d9-193">Retorna uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="c62d9-193">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="c62d9-194">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="c62d9-194">Request 3</span></span>](#request-3)|
|<span data-ttu-id="c62d9-195">$filter com o operador **any**</span><span class="sxs-lookup"><span data-stu-id="c62d9-195">$filter with **any** operator</span></span>|<span data-ttu-id="c62d9-196">Retorna instâncias de uma coleção de recursos que contêm uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="c62d9-196">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|[<span data-ttu-id="c62d9-197">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="c62d9-197">Request 5</span></span>](#request-5)|
|<span data-ttu-id="c62d9-198">$expand</span><span class="sxs-lookup"><span data-stu-id="c62d9-198">$expand</span></span>|<span data-ttu-id="c62d9-199">Expande uma instância de recurso para incluir uma extensão.</span><span class="sxs-lookup"><span data-stu-id="c62d9-199">Expands a resource instance to include an extension.</span></span> |<span data-ttu-id="c62d9-200">[Solicitação 3](#request-3) e [solicitação 5](#request-5)</span><span class="sxs-lookup"><span data-stu-id="c62d9-200">[Request 3](#request-3) and [request 5](#request-5)</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c62d9-201">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c62d9-201">Request headers</span></span>
| <span data-ttu-id="c62d9-202">Nome</span><span class="sxs-lookup"><span data-stu-id="c62d9-202">Name</span></span>       | <span data-ttu-id="c62d9-203">Valor</span><span class="sxs-lookup"><span data-stu-id="c62d9-203">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c62d9-204">Autorização</span><span class="sxs-lookup"><span data-stu-id="c62d9-204">Authorization</span></span> | <span data-ttu-id="c62d9-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c62d9-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c62d9-207">Request body</span></span>
<span data-ttu-id="c62d9-208">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c62d9-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c62d9-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="c62d9-209">Response</span></span>

<span data-ttu-id="c62d9-p107">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [openTypeExtension](../resources/opentypeextension.md) no corpo da resposta. Dependendo da consulta GET, o corpo da resposta exato pode ser diferente.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="c62d9-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c62d9-212">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="c62d9-213">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="c62d9-213">Request 1</span></span>

<span data-ttu-id="c62d9-p108">O primeiro exemplo mostra 2 maneiras de referenciar uma extensão e obtém a extensão na mensagem especificada. A resposta é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="c62d9-216">Em primeiro lugar, por nome:</span><span class="sxs-lookup"><span data-stu-id="c62d9-216">First, by its name:</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="c62d9-217">HTTP</span><span class="sxs-lookup"><span data-stu-id="c62d9-217">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c62d9-218">C#</span><span class="sxs-lookup"><span data-stu-id="c62d9-218">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c62d9-219">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c62d9-219">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c62d9-220">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c62d9-220">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c62d9-221">Java</span><span class="sxs-lookup"><span data-stu-id="c62d9-221">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c62d9-222">Em segundo lugar, por ID (nome totalmente qualificado):</span><span class="sxs-lookup"><span data-stu-id="c62d9-222">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

#### <a name="response-1"></a><span data-ttu-id="c62d9-223">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="c62d9-223">Response 1</span></span>
<span data-ttu-id="c62d9-224">Veja a seguir a resposta para o primeiro exemplo.</span><span class="sxs-lookup"><span data-stu-id="c62d9-224">Here is the response for the first example.</span></span>
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


#### <a name="request-2"></a><span data-ttu-id="c62d9-225">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="c62d9-225">Request 2</span></span>

<span data-ttu-id="c62d9-226">O segundo exemplo faz referência a uma extensão por nome e obtém essa extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="c62d9-226">The second example references an extension by its name and gets the extension in the specified group event.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c62d9-227">HTTP</span><span class="sxs-lookup"><span data-stu-id="c62d9-227">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Deal", "f5480dfd-7d77-4d0b-ba2e-3391953cc74a", "AAMkADVl17IsAAA="],
  "name": "get_opentypeextension_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c62d9-228">C#</span><span class="sxs-lookup"><span data-stu-id="c62d9-228">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c62d9-229">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c62d9-229">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c62d9-230">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c62d9-230">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c62d9-231">Java</span><span class="sxs-lookup"><span data-stu-id="c62d9-231">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response-2"></a><span data-ttu-id="c62d9-232">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="c62d9-232">Response 2</span></span>

<span data-ttu-id="c62d9-233">Veja a seguir a resposta do segundo exemplo.</span><span class="sxs-lookup"><span data-stu-id="c62d9-233">Here is the response from the second example.</span></span>

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

#### <a name="request-3"></a><span data-ttu-id="c62d9-234">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="c62d9-234">Request 3</span></span>

<span data-ttu-id="c62d9-p109">O terceiro exemplo obtém e expande a mensagem especificada, incluindo a extensão retornada de um filtro. O filtro retorna a extensão cujo **id** corresponde a um nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c62d9-237">HTTP</span><span class="sxs-lookup"><span data-stu-id="c62d9-237">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c62d9-238">C#</span><span class="sxs-lookup"><span data-stu-id="c62d9-238">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-opentypeextension-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c62d9-239">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c62d9-239">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-opentypeextension-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c62d9-240">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c62d9-240">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-opentypeextension-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c62d9-241">Java</span><span class="sxs-lookup"><span data-stu-id="c62d9-241">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-opentypeextension-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response-3"></a><span data-ttu-id="c62d9-242">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="c62d9-242">Response 3</span></span>

<span data-ttu-id="c62d9-p110">Veja a seguir a resposta do terceiro exemplo. Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

#### <a name="request-4"></a><span data-ttu-id="c62d9-246">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="c62d9-246">Request 4</span></span>

<span data-ttu-id="c62d9-247">O quarto exemplo faz referência a uma extensão por nome totalmente qualificado e obtém essa extensão na postagem de grupo especificada.</span><span class="sxs-lookup"><span data-stu-id="c62d9-247">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```

#### <a name="response-4"></a><span data-ttu-id="c62d9-248">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="c62d9-248">Response 4</span></span>

<span data-ttu-id="c62d9-249">Veja a seguir a resposta do quarto exemplo.</span><span class="sxs-lookup"><span data-stu-id="c62d9-249">Here is the response from the fourth example.</span></span> 

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


#### <a name="request-5"></a><span data-ttu-id="c62d9-250">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="c62d9-250">Request 5</span></span>

<span data-ttu-id="c62d9-p111">O quinto exemplo analisa todas as mensagens na caixa de correio do usuário conectado para localizar aquelas uma contêm uma extensão correspondente a um filtro e as expande com a inclusão dessa extensão. O filtro retorna extensões cuja propriedade **id** corresponde ao nome da extensão `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


#### <a name="response-5"></a><span data-ttu-id="c62d9-253">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="c62d9-253">Response 5</span></span>

<span data-ttu-id="c62d9-254">Nessa resposta do quinto exemplo, há apenas uma mensagem na caixa de correio do usuário que tem uma extensão cuja **id** é igual a `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="c62d9-254">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="c62d9-p112">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c62d9-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
