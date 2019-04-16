---
title: Obter extensão aberta
description: Obtenha uma extensão aberta (objeto openTypeExtension) identificada por nome ou nome totalmente qualificado.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 010212497eef3de812c87055a5b1db3cd7b305ca
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2019
ms.locfileid: "31890028"
---
# <a name="get-open-extension"></a><span data-ttu-id="f50e2-103">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="f50e2-103">Get open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f50e2-104">Obtenha uma extensão aberta (objeto[openTypeExtension](../resources/opentypeextension.md) ) identificada por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="f50e2-104">Get an open extension ([openTypeExtension](../resources/opentypeextension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="f50e2-105">A tabela a seguir lista os três cenários em que é possível obter uma extensão aberta de uma instância de recurso com suporte.</span><span class="sxs-lookup"><span data-stu-id="f50e2-105">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="f50e2-106">**Cenário GET**</span><span class="sxs-lookup"><span data-stu-id="f50e2-106">**GET scenario**</span></span>|<span data-ttu-id="f50e2-107">**Recursos com suporte**</span><span class="sxs-lookup"><span data-stu-id="f50e2-107">**Supported resources**</span></span>|<span data-ttu-id="f50e2-108">**Corpo da resposta**</span><span class="sxs-lookup"><span data-stu-id="f50e2-108">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f50e2-109">Obtenha uma extensão específica de uma instância de recurso conhecida.</span><span class="sxs-lookup"><span data-stu-id="f50e2-109">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="f50e2-110">[Unidade administrativa](../resources/administrativeunit.md), [dispositivo](../resources/device.md), [evento](../resources/event.md), [grupo](../resources/group.md), [evento de grupo](../resources/event.md), postagem de [grupo](../resources/post.md), [mensagem](../resources/message.md), [organização](../resources/organization.md), [contato pessoal](../resources/contact.md), [usuário](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="f50e2-110">[Administrative unit](../resources/administrativeunit.md), [device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="f50e2-111">Somente a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="f50e2-111">Open extension only.</span></span>|
|<span data-ttu-id="f50e2-112">Obtenha uma instância de recurso conhecida, expandida com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="f50e2-112">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="f50e2-113">Unidade administrativa, dispositivo, evento, grupo, evento de grupo, postagem de grupo, mensagem, organização, contato pessoal, usuário</span><span class="sxs-lookup"><span data-stu-id="f50e2-113">Administrative unit, device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="f50e2-114">Uma instância de recurso expandida com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="f50e2-114">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="f50e2-115">Encontre e expanda instâncias de recursos com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="f50e2-115">Find and expand resource instances with a specific extension.</span></span> | <span data-ttu-id="f50e2-116">Evento, grupo evento, postagem de grupo, mensagem, contato pessoal</span><span class="sxs-lookup"><span data-stu-id="f50e2-116">Event, group event, group post, message, personal contact</span></span> |<span data-ttu-id="f50e2-117">Instâncias de recursos expandidas com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="f50e2-117">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="f50e2-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="f50e2-118">Permissions</span></span>

<span data-ttu-id="f50e2-119">Dependendo do recurso que contém a extensão e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f50e2-119">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="f50e2-120">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f50e2-120">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f50e2-121">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="f50e2-121">Supported resource</span></span> | <span data-ttu-id="f50e2-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f50e2-122">Delegated (work or school account)</span></span> | <span data-ttu-id="f50e2-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f50e2-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f50e2-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f50e2-124">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="f50e2-125">device</span><span class="sxs-lookup"><span data-stu-id="f50e2-125">device</span></span>](../resources/device.md) | <span data-ttu-id="f50e2-126">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e2-126">Directory.Read.All</span></span> | <span data-ttu-id="f50e2-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f50e2-127">Not supported</span></span> | <span data-ttu-id="f50e2-128">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f50e2-128">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="f50e2-129">evento</span><span class="sxs-lookup"><span data-stu-id="f50e2-129">event</span></span>](../resources/event.md) | <span data-ttu-id="f50e2-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-130">Calendars.Read</span></span> | <span data-ttu-id="f50e2-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-131">Calendars.Read</span></span> | <span data-ttu-id="f50e2-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-132">Calendars.Read</span></span> |
| [<span data-ttu-id="f50e2-133">grupo</span><span class="sxs-lookup"><span data-stu-id="f50e2-133">group</span></span>](../resources/group.md) | <span data-ttu-id="f50e2-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e2-134">Group.Read.All</span></span> | <span data-ttu-id="f50e2-135">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f50e2-135">Not supported</span></span> | <span data-ttu-id="f50e2-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e2-136">Group.Read.All</span></span> |
| [<span data-ttu-id="f50e2-137">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="f50e2-137">group event</span></span>](../resources/event.md) | <span data-ttu-id="f50e2-138">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e2-138">Group.Read.All</span></span> | <span data-ttu-id="f50e2-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f50e2-139">Not supported</span></span> | <span data-ttu-id="f50e2-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f50e2-140">Not supported</span></span> |
| [<span data-ttu-id="f50e2-141">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="f50e2-141">group post</span></span>](../resources/post.md) | <span data-ttu-id="f50e2-142">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e2-142">Group.Read.All</span></span> | <span data-ttu-id="f50e2-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f50e2-143">Not supported</span></span> | <span data-ttu-id="f50e2-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e2-144">Group.Read.All</span></span> |
| [<span data-ttu-id="f50e2-145">mensagem</span><span class="sxs-lookup"><span data-stu-id="f50e2-145">message</span></span>](../resources/message.md) | <span data-ttu-id="f50e2-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-146">Mail.Read</span></span> | <span data-ttu-id="f50e2-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-147">Mail.Read</span></span> | <span data-ttu-id="f50e2-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-148">Mail.Read</span></span> | 
| [<span data-ttu-id="f50e2-149">organization</span><span class="sxs-lookup"><span data-stu-id="f50e2-149">organization</span></span>](../resources/organization.md) | <span data-ttu-id="f50e2-150">User.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-150">User.Read</span></span> | <span data-ttu-id="f50e2-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f50e2-151">Not supported</span></span> | <span data-ttu-id="f50e2-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="f50e2-152">Not supported</span></span> |
| [<span data-ttu-id="f50e2-153">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="f50e2-153">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="f50e2-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-154">Contacts.Read</span></span> | <span data-ttu-id="f50e2-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-155">Contacts.Read</span></span> | <span data-ttu-id="f50e2-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-156">Contacts.Read</span></span> |
| [<span data-ttu-id="f50e2-157">user</span><span class="sxs-lookup"><span data-stu-id="f50e2-157">user</span></span>](../resources/user.md) | <span data-ttu-id="f50e2-158">User.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-158">User.Read</span></span> | <span data-ttu-id="f50e2-159">User.Read</span><span class="sxs-lookup"><span data-stu-id="f50e2-159">User.Read</span></span> | <span data-ttu-id="f50e2-160">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="f50e2-160">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f50e2-161">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f50e2-161">HTTP request</span></span>

<span data-ttu-id="f50e2-162">Esta seção lista a sintaxe de cada um dos três cenários `GET` descritos acima</span><span class="sxs-lookup"><span data-stu-id="f50e2-162">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="f50e2-163">Obtenha uma extensão específica em uma instância de recurso conhecida</span><span class="sxs-lookup"><span data-stu-id="f50e2-163">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="f50e2-164">Use a mesma solicitação REST obtendo a instância do recurso e identifique a extensão usando a propriedade de navegação **extensions** dessa instância.</span><span class="sxs-lookup"><span data-stu-id="f50e2-164">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

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
```

### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="f50e2-165">Obtenha uma instância de recurso conhecida, expandida com uma extensão correspondente.</span><span class="sxs-lookup"><span data-stu-id="f50e2-165">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="f50e2-166">Para os tipos de recurso evento, evento de grupo, postagem de grupo, mensagem, contato pessoal, você pode usar a mesma solicitação REST que obter a instância de recurso, procure uma extensão que corresponda a um filtro na propriedade **ID** e expanda a instância com a extensão.</span><span class="sxs-lookup"><span data-stu-id="f50e2-166">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension.</span></span> <span data-ttu-id="f50e2-167">A resposta inclui a maioria das propriedades de recurso.</span><span class="sxs-lookup"><span data-stu-id="f50e2-167">The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="f50e2-168">Para os tipos de recurso dispositivo, grupo, organização e usuário, você também deve usar um `$select` parâmetro para incluir a propriedade **ID** e qualquer outra propriedade que você queira da instância de recurso:</span><span class="sxs-lookup"><span data-stu-id="f50e2-168">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```


### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="f50e2-169">Filtrar as instâncias do recurso expandidas com uma extensão correspondente</span><span class="sxs-lookup"><span data-stu-id="f50e2-169">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="f50e2-170">Use a mesma solicitação REST para obter uma coleção do recurso suportado, filtre a coleção para instâncias que contêm uma extensão com uma propriedade **id** correspondente e expanda essas instâncias com a extensão.</span><span class="sxs-lookup"><span data-stu-id="f50e2-170">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="f50e2-171">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso ou coleção para obter uma extensão dela.</span><span class="sxs-lookup"><span data-stu-id="f50e2-171">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it.</span></span> <span data-ttu-id="f50e2-172">Todas as outras sintaxes que permitem identificar essas instâncias de recursos ou coleções oferecem suporte para a introdução de extensões abertas de forma semelhante.</span><span class="sxs-lookup"><span data-stu-id="f50e2-172">All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>


## <a name="path-parameters"></a><span data-ttu-id="f50e2-173">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="f50e2-173">Path parameters</span></span>
|<span data-ttu-id="f50e2-174">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="f50e2-174">**Parameter**</span></span>|<span data-ttu-id="f50e2-175">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="f50e2-175">**Type**</span></span>|<span data-ttu-id="f50e2-176">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f50e2-176">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f50e2-177">Id</span><span class="sxs-lookup"><span data-stu-id="f50e2-177">Id</span></span>|<span data-ttu-id="f50e2-178">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f50e2-178">string</span></span>|<span data-ttu-id="f50e2-p104">Espaço reservado para um identificador exclusivo de um objeto na coleção correspondente, como mensagens, contatos e eventos. Obrigatório. Não deve ser confundido com a propriedade **id** de uma **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="f50e2-182">extensionId</span><span class="sxs-lookup"><span data-stu-id="f50e2-182">extensionId</span></span>|<span data-ttu-id="f50e2-183">string</span><span class="sxs-lookup"><span data-stu-id="f50e2-183">string</span></span>|<span data-ttu-id="f50e2-p105">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para um a uma extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade **id** quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="f50e2-187">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f50e2-187">Optional query parameters</span></span>

<span data-ttu-id="f50e2-188">Certifique-se de aplicar a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de caracteres `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f50e2-188">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="f50e2-189">**Nome**</span><span class="sxs-lookup"><span data-stu-id="f50e2-189">**Name**</span></span>|<span data-ttu-id="f50e2-190">**Valor**</span><span class="sxs-lookup"><span data-stu-id="f50e2-190">**Value**</span></span>|<span data-ttu-id="f50e2-191">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f50e2-191">**Description**</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="f50e2-192">$filter</span><span class="sxs-lookup"><span data-stu-id="f50e2-192">$filter</span></span>|<span data-ttu-id="f50e2-193">string</span><span class="sxs-lookup"><span data-stu-id="f50e2-193">string</span></span>|<span data-ttu-id="f50e2-194">Retorna uma extensão com sua **id** correspondentes ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="f50e2-194">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="f50e2-195">$filter com o operador **any**</span><span class="sxs-lookup"><span data-stu-id="f50e2-195">$filter with **any** operator</span></span>|<span data-ttu-id="f50e2-196">string</span><span class="sxs-lookup"><span data-stu-id="f50e2-196">string</span></span>|<span data-ttu-id="f50e2-197">Retorna instâncias de uma coleção de recursos que contêm uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="f50e2-197">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="f50e2-198">$expand</span><span class="sxs-lookup"><span data-stu-id="f50e2-198">$expand</span></span>|<span data-ttu-id="f50e2-199">string</span><span class="sxs-lookup"><span data-stu-id="f50e2-199">string</span></span>|<span data-ttu-id="f50e2-200">Expande uma instância de recurso para incluir uma extensão.</span><span class="sxs-lookup"><span data-stu-id="f50e2-200">Expands a resource instance to include an extension.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f50e2-201">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f50e2-201">Request headers</span></span>
| <span data-ttu-id="f50e2-202">Nome</span><span class="sxs-lookup"><span data-stu-id="f50e2-202">Name</span></span>       | <span data-ttu-id="f50e2-203">Valor</span><span class="sxs-lookup"><span data-stu-id="f50e2-203">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f50e2-204">Autorização</span><span class="sxs-lookup"><span data-stu-id="f50e2-204">Authorization</span></span> | <span data-ttu-id="f50e2-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f50e2-207">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f50e2-207">Request body</span></span>
<span data-ttu-id="f50e2-208">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f50e2-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f50e2-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="f50e2-209">Response</span></span>

<span data-ttu-id="f50e2-p107">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [openTypeExtension](../resources/opentypeextension.md) no corpo da resposta. Dependendo da consulta GET, o corpo da resposta exato pode ser diferente.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="f50e2-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f50e2-212">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="f50e2-213">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="f50e2-213">Request 1</span></span>

<span data-ttu-id="f50e2-p108">O primeiro exemplo mostra 2 maneiras de referenciar uma extensão e obtém a extensão na mensagem especificada. A resposta é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="f50e2-216">Em primeiro lugar, por nome:</span><span class="sxs-lookup"><span data-stu-id="f50e2-216">First, by its name:</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="f50e2-217">Em segundo lugar, por ID (nome totalmente qualificado):</span><span class="sxs-lookup"><span data-stu-id="f50e2-217">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

#### <a name="response-1"></a><span data-ttu-id="f50e2-218">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="f50e2-218">Response 1</span></span>
<span data-ttu-id="f50e2-219">Veja a seguir a resposta para o primeiro exemplo.</span><span class="sxs-lookup"><span data-stu-id="f50e2-219">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
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


#### <a name="request-2"></a><span data-ttu-id="f50e2-220">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="f50e2-220">Request 2</span></span>

<span data-ttu-id="f50e2-221">O segundo exemplo faz referência a uma extensão por nome e obtém essa extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="f50e2-221">The second example references an extension by its name and gets the extension in the specified group event.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_2"
}-->
```http
GET https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions('Com.Contoso.Deal') 
```

#### <a name="response-2"></a><span data-ttu-id="f50e2-222">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="f50e2-222">Response 2</span></span>

<span data-ttu-id="f50e2-223">Veja a seguir a resposta do segundo exemplo.</span><span class="sxs-lookup"><span data-stu-id="f50e2-223">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="f50e2-224">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="f50e2-224">Request 3</span></span>

<span data-ttu-id="f50e2-p109">O terceiro exemplo obtém e expande a mensagem especificada, incluindo a extensão retornada de um filtro. O filtro retorna a extensão cujo **id** corresponde a um nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```


#### <a name="response-3"></a><span data-ttu-id="f50e2-227">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="f50e2-227">Response 3</span></span>

<span data-ttu-id="f50e2-p110">Veja a seguir a resposta do terceiro exemplo. Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

#### <a name="request-4"></a><span data-ttu-id="f50e2-231">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="f50e2-231">Request 4</span></span>

<span data-ttu-id="f50e2-232">O quarto exemplo faz referência a uma extensão por nome totalmente qualificado e obtém essa extensão na postagem de grupo especificada.</span><span class="sxs-lookup"><span data-stu-id="f50e2-232">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/beta/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate') 
```

#### <a name="response-4"></a><span data-ttu-id="f50e2-233">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="f50e2-233">Response 4</span></span>

<span data-ttu-id="f50e2-234">Veja a seguir a resposta do quarto exemplo.</span><span class="sxs-lookup"><span data-stu-id="f50e2-234">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
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


#### <a name="request-5"></a><span data-ttu-id="f50e2-235">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="f50e2-235">Request 5</span></span>

<span data-ttu-id="f50e2-p111">O quinto exemplo analisa todas as mensagens na caixa de correio do usuário conectado para localizar aquelas uma contêm uma extensão correspondente a um filtro e as expande com a inclusão dessa extensão. O filtro retorna extensões cuja propriedade **id** corresponde ao nome da extensão `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


#### <a name="response-5"></a><span data-ttu-id="f50e2-238">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="f50e2-238">Response 5</span></span>

<span data-ttu-id="f50e2-239">Nessa resposta do quinto exemplo, há apenas uma mensagem na caixa de correio do usuário que tem uma extensão cuja **id** é igual a `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="f50e2-239">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="f50e2-p112">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f50e2-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/opentypeextension-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
