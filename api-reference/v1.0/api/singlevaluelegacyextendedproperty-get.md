---
title: Obter singleValueLegacyExtendedProperty
description: Você pode obter uma única instância de recurso expandida com uma propriedade estendida específica ou uma coleção de instâncias de recurso
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f1830619c33067e1c4f892cff531c72d0ce1a4f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021498"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="addbe-103">Obter singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="addbe-103">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="addbe-104">Você pode acessar uma instância de recurso único expandida com uma propriedade estendida específica ou uma coleção de instâncias de recurso que incluem as propriedades estendidas que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-104">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="addbe-105">Usar o parâmetro de consulta `$expand` permite que você acesse a instância de recurso especificada expandida com uma propriedade estendida específica.</span><span class="sxs-lookup"><span data-stu-id="addbe-105">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="addbe-106">Use um `$filter` e um operador `eq` na propriedade **id** para especificar a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="addbe-106">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="addbe-107">Atualmente, esta é a única maneira de acessar o objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="addbe-107">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="addbe-108">Para acessar instâncias de recurso com determinadas propriedades estendidas, use o parâmetro de consulta `$filter` e aplique um operador `eq` na propriedade **id**.</span><span class="sxs-lookup"><span data-stu-id="addbe-108">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="addbe-109">Além disso, em propriedades estendidas numéricas, aplique um dos seguintes operadores na propriedade **valor**: `eq`, `ne`,`ge`, `gt`, `le` ou `lt`.</span><span class="sxs-lookup"><span data-stu-id="addbe-109">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="addbe-110">Para propriedades estendidas de cadeia de caracteres digitados, aplique um operador `contains`, `startswith`, `eq` ou `ne` em **value**.</span><span class="sxs-lookup"><span data-stu-id="addbe-110">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="addbe-111">O filtro é aplicado a todas as instâncias do recurso na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="addbe-111">The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span> 

<span data-ttu-id="addbe-112">Maiúsculas e minúsculas são diferenciadas ao filtrar o nome de cadeia de caracteres (`Name`) na **id** de uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="addbe-112">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="addbe-113">Maiúsculas e minúsculas não são diferenciadas ao filtrar a propriedade **value** de uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="addbe-113">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="addbe-114">Há suporte para os seguintes recursos de usuário:</span><span class="sxs-lookup"><span data-stu-id="addbe-114">The following user resources are supported:</span></span>

- [<span data-ttu-id="addbe-115">calendar</span><span class="sxs-lookup"><span data-stu-id="addbe-115">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="addbe-116">contact</span><span class="sxs-lookup"><span data-stu-id="addbe-116">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="addbe-117">contactFolder</span><span class="sxs-lookup"><span data-stu-id="addbe-117">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="addbe-118">evento</span><span class="sxs-lookup"><span data-stu-id="addbe-118">event</span></span>](../resources/event.md)
- [<span data-ttu-id="addbe-119">mailFolder</span><span class="sxs-lookup"><span data-stu-id="addbe-119">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="addbe-120">message</span><span class="sxs-lookup"><span data-stu-id="addbe-120">message</span></span>](../resources/message.md) 

<span data-ttu-id="addbe-121">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="addbe-121">As well as the following group resources:</span></span>

- <span data-ttu-id="addbe-122">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="addbe-122">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="addbe-123">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="addbe-123">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="addbe-124">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="addbe-124">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="addbe-125">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="addbe-125">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="addbe-126">Permissões</span><span class="sxs-lookup"><span data-stu-id="addbe-126">Permissions</span></span>
<span data-ttu-id="addbe-127">Dependendo do recurso para o qual você está obtendo a propriedade estendida e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="addbe-127">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="addbe-128">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="addbe-128">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="addbe-129">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="addbe-129">Supported resource</span></span> | <span data-ttu-id="addbe-130">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="addbe-130">Delegated (work or school account)</span></span> | <span data-ttu-id="addbe-131">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="addbe-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="addbe-132">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="addbe-132">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="addbe-133">calendar</span><span class="sxs-lookup"><span data-stu-id="addbe-133">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="addbe-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-134">Calendars.Read</span></span> | <span data-ttu-id="addbe-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-135">Calendars.Read</span></span> | <span data-ttu-id="addbe-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-136">Calendars.Read</span></span> |
| [<span data-ttu-id="addbe-137">contato</span><span class="sxs-lookup"><span data-stu-id="addbe-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="addbe-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-138">Contacts.Read</span></span> | <span data-ttu-id="addbe-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-139">Contacts.Read</span></span> | <span data-ttu-id="addbe-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-140">Contacts.Read</span></span> |
| [<span data-ttu-id="addbe-141">contactFolder</span><span class="sxs-lookup"><span data-stu-id="addbe-141">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="addbe-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-142">Contacts.Read</span></span> | <span data-ttu-id="addbe-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-143">Contacts.Read</span></span> | <span data-ttu-id="addbe-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-144">Contacts.Read</span></span> |
| [<span data-ttu-id="addbe-145">evento</span><span class="sxs-lookup"><span data-stu-id="addbe-145">event</span></span>](../resources/event.md) | <span data-ttu-id="addbe-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-146">Calendars.Read</span></span> | <span data-ttu-id="addbe-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-147">Calendars.Read</span></span> |  <span data-ttu-id="addbe-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-148">Calendars.Read</span></span>|
| <span data-ttu-id="addbe-149">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="addbe-149">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="addbe-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="addbe-150">Group.Read.All</span></span> | <span data-ttu-id="addbe-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="addbe-151">Not supported</span></span> | <span data-ttu-id="addbe-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="addbe-152">Not supported</span></span> |
| <span data-ttu-id="addbe-153">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="addbe-153">group [event](../resources/event.md)</span></span> | <span data-ttu-id="addbe-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="addbe-154">Group.Read.All</span></span> | <span data-ttu-id="addbe-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="addbe-155">Not supported</span></span> | <span data-ttu-id="addbe-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="addbe-156">Not supported</span></span> |
| <span data-ttu-id="addbe-157">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="addbe-157">group [post](../resources/post.md)</span></span> | <span data-ttu-id="addbe-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="addbe-158">Group.Read.All</span></span> | <span data-ttu-id="addbe-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="addbe-159">Not supported</span></span> | <span data-ttu-id="addbe-160">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="addbe-160">Group.Read.All</span></span> |
| [<span data-ttu-id="addbe-161">mailFolder</span><span class="sxs-lookup"><span data-stu-id="addbe-161">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="addbe-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-162">Mail.Read</span></span> | <span data-ttu-id="addbe-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-163">Mail.Read</span></span> | <span data-ttu-id="addbe-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-164">Mail.Read</span></span> |
| [<span data-ttu-id="addbe-165">message</span><span class="sxs-lookup"><span data-stu-id="addbe-165">message</span></span>](../resources/message.md) | <span data-ttu-id="addbe-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-166">Mail.Read</span></span> | <span data-ttu-id="addbe-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-167">Mail.Read</span></span> | <span data-ttu-id="addbe-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="addbe-168">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="addbe-169">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="addbe-169">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="addbe-170">Instância de recurso GET expandida com uma propriedade estendida que corresponde a um filtro</span><span class="sxs-lookup"><span data-stu-id="addbe-170">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="addbe-p105">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="addbe-173">Obtenha uma instância de **message**:</span><span class="sxs-lookup"><span data-stu-id="addbe-173">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="addbe-174">Obtenha uma instância de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="addbe-174">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="addbe-175">Obtenha uma instância de **event**:</span><span class="sxs-lookup"><span data-stu-id="addbe-175">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="addbe-176">Obtenha uma instância de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="addbe-176">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="addbe-177">Obtenha uma instância de **contact**:</span><span class="sxs-lookup"><span data-stu-id="addbe-177">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="addbe-178">Obtenha uma instância de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="addbe-178">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="addbe-179">Obtenha uma instância de **group event**:</span><span class="sxs-lookup"><span data-stu-id="addbe-179">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="addbe-180">Acesse uma instância de **postar** em grupo:</span><span class="sxs-lookup"><span data-stu-id="addbe-180">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="addbe-181">Instâncias de recurso GET que incluem as propriedades estendidas numéricas que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-181">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="addbe-182">Acesse as instâncias de um recurso com suporte que têm uma propriedade estendida numérica que corresponde a um filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-182">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="addbe-183">O filtro usa um operador `eq` na propriedade **id** e um dos seguintes operadores na propriedade **value**: `eq`, `ne`,`ge`, `gt`, `le` ou `lt`.</span><span class="sxs-lookup"><span data-stu-id="addbe-183">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="addbe-184">Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos seguintes caracteres na cadeia de filtro: dois pontos, barra inclinada e espaço.</span><span class="sxs-lookup"><span data-stu-id="addbe-184">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="addbe-185">As linhas de sintaxe a seguir mostram um filtro que usa um operador `eq` na id e outro operador `eq` no valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="addbe-185">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="addbe-186">Você pode substituir o operador `eq` no **value** por qualquer um dos outros operadores (`ne`,`ge`, `gt`, `le` ou `lt`) que se aplicam aos valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="addbe-186">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="addbe-187">Obtenha instâncias de **message**:</span><span class="sxs-lookup"><span data-stu-id="addbe-187">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="addbe-188">Acesse as instâncias de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="addbe-188">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="addbe-189">Obtenha instâncias de **event**:</span><span class="sxs-lookup"><span data-stu-id="addbe-189">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="addbe-190">Acesse as instâncias de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="addbe-190">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="addbe-191">Acesse as instâncias de **contact**:</span><span class="sxs-lookup"><span data-stu-id="addbe-191">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="addbe-192">Acesse as instâncias de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="addbe-192">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="addbe-193">Obtenha instâncias de **group event**:</span><span class="sxs-lookup"><span data-stu-id="addbe-193">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="addbe-194">Acesse as instâncias de **postar** em grupo:</span><span class="sxs-lookup"><span data-stu-id="addbe-194">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="addbe-195">Instâncias de recurso GET com propriedades estendidas de cadeia de caracteres digitados que correspondem a um filtro</span><span class="sxs-lookup"><span data-stu-id="addbe-195">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="addbe-196">Acesse as instâncias do recurso **message** ou **event** que têm uma propriedade estendida de cadeia de caracteres digitados que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-196">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="addbe-197">O filtro usa um operador `eq` na propriedade **id** e um dos seguintes operadores na propriedade **valor**: `contains`, `startswith`, `eq` ou `ne`.</span><span class="sxs-lookup"><span data-stu-id="addbe-197">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="addbe-198">Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos seguintes caracteres na cadeia de filtro: dois pontos, barra inclinada e espaço.</span><span class="sxs-lookup"><span data-stu-id="addbe-198">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="addbe-199">Acesse as instâncias de **mensagem**:</span><span class="sxs-lookup"><span data-stu-id="addbe-199">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="addbe-200">Acesse as instâncias de **event**:</span><span class="sxs-lookup"><span data-stu-id="addbe-200">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')

GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

<span data-ttu-id="addbe-201">Acesse as instâncias de **group event**:</span><span class="sxs-lookup"><span data-stu-id="addbe-201">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="addbe-202">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="addbe-202">Path parameters</span></span>
|<span data-ttu-id="addbe-203">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="addbe-203">Parameter</span></span>|<span data-ttu-id="addbe-204">Tipo</span><span class="sxs-lookup"><span data-stu-id="addbe-204">Type</span></span>|<span data-ttu-id="addbe-205">Descrição</span><span class="sxs-lookup"><span data-stu-id="addbe-205">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="addbe-206">id_value</span><span class="sxs-lookup"><span data-stu-id="addbe-206">id_value</span></span>|<span data-ttu-id="addbe-207">String</span><span class="sxs-lookup"><span data-stu-id="addbe-207">String</span></span>|<span data-ttu-id="addbe-p109">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="addbe-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="addbe-212">property_value</span><span class="sxs-lookup"><span data-stu-id="addbe-212">property_value</span></span> |<span data-ttu-id="addbe-213">String</span><span class="sxs-lookup"><span data-stu-id="addbe-213">String</span></span>|<span data-ttu-id="addbe-214">O valor da propriedade estendida a ser correspondida.</span><span class="sxs-lookup"><span data-stu-id="addbe-214">The value of the extended property to match.</span></span> <span data-ttu-id="addbe-215">Obrigatório quando indicado na seção **Solicitação HTTP** acima.</span><span class="sxs-lookup"><span data-stu-id="addbe-215">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="addbe-216">Se {property_value} não for uma cadeia de caracteres, converta o `ep/value` para o tipo de dado Edm apropriado ao compará-lo com {property_value}.</span><span class="sxs-lookup"><span data-stu-id="addbe-216">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="addbe-217">Confira exemplos na [solicitação 4](#request-4) abaixo.</span><span class="sxs-lookup"><span data-stu-id="addbe-217">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="addbe-218">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="addbe-218">Request headers</span></span>
| <span data-ttu-id="addbe-219">Nome</span><span class="sxs-lookup"><span data-stu-id="addbe-219">Name</span></span>      |<span data-ttu-id="addbe-220">Descrição</span><span class="sxs-lookup"><span data-stu-id="addbe-220">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="addbe-221">Autorização</span><span class="sxs-lookup"><span data-stu-id="addbe-221">Authorization</span></span>  | <span data-ttu-id="addbe-p111">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="addbe-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="addbe-224">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="addbe-224">Request body</span></span>
<span data-ttu-id="addbe-225">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="addbe-225">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="addbe-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="addbe-226">Response</span></span>

<span data-ttu-id="addbe-227">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="addbe-227">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-expanded-with-a-matching-extended-property"></a><span data-ttu-id="addbe-228">Instância de recurso GET expandida com uma propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="addbe-228">GET resource instance expanded with a matching extended property</span></span>
<span data-ttu-id="addbe-229">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="addbe-229">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="addbe-230">Instâncias de recurso GET que contenham uma propriedade estendida correspondente a um filtro</span><span class="sxs-lookup"><span data-stu-id="addbe-230">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="addbe-231">O corpo da resposta inclui um ou mais objetos que representam as instâncias de recursos contendo uma propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="addbe-231">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="addbe-232">O corpo da resposta não inclui a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="addbe-232">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="addbe-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="addbe-233">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="addbe-234">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="addbe-234">Request 1</span></span>

<span data-ttu-id="addbe-p113">O primeiro exemplo obtém e expande a mensagem especificada, incluindo uma propriedade estendida de valor único. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="addbe-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="addbe-237">HTTP</span><span class="sxs-lookup"><span data-stu-id="addbe-237">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2_bs88AACHsLqWAAA="],
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="addbe-238">C#</span><span class="sxs-lookup"><span data-stu-id="addbe-238">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-singlevaluelegacyextendedproperty-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="addbe-239">Javascript</span><span class="sxs-lookup"><span data-stu-id="addbe-239">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-singlevaluelegacyextendedproperty-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="addbe-240">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="addbe-240">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-singlevaluelegacyextendedproperty-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="addbe-241">Java</span><span class="sxs-lookup"><span data-stu-id="addbe-241">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-singlevaluelegacyextendedproperty-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-1"></a><span data-ttu-id="addbe-242">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="addbe-242">Response 1</span></span>
<span data-ttu-id="addbe-243">O corpo da resposta inclui todas as propriedades da mensagem especificada e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-243">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="addbe-p114">Observação: O objeto **message** mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="addbe-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a><span data-ttu-id="addbe-246">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="addbe-246">Request 2</span></span>

<span data-ttu-id="addbe-247">O segundo exemplo obtém mensagens que possuem a propriedade estendida de valor único com cadeia de caracteres digitada especificada no filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-247">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="addbe-248">O filtro procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="addbe-248">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="addbe-249">**id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação aqui removida para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="addbe-249">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="addbe-250">O **valor** igual à cadeia de caracteres `Green`.</span><span class="sxs-lookup"><span data-stu-id="addbe-250">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="addbe-251">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="addbe-251">Response 2</span></span>

<span data-ttu-id="addbe-p116">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK`, e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro. O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md). A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="addbe-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="addbe-255">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="addbe-255">Request 3</span></span>

<span data-ttu-id="addbe-256">O terceiro exemplo obtém mensagens que possuem a propriedade estendida de valor único com cadeia de caracteres digitada especificada no filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-256">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="addbe-257">O filtro procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="addbe-257">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="addbe-258">**id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação aqui removida para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="addbe-258">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="addbe-259">O **value** que contém a cadeia de caracteres `green`.</span><span class="sxs-lookup"><span data-stu-id="addbe-259">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="addbe-260">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="addbe-260">Response 3</span></span>

<span data-ttu-id="addbe-261">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK` e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-261">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="addbe-262">Por exemplo, uma mensagem com uma propriedade estendida de valor único com a **id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` e ao **value** `Light green` corresponderia ao filtro e seria incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="addbe-262">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="addbe-263">O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="addbe-263">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="addbe-264">A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="addbe-264">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="addbe-265">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="addbe-265">Request 4</span></span>

<span data-ttu-id="addbe-266">Os próximos dois exemplos mostram como acessar mensagens que possuam propriedades estendidas de valor único sem cadeia de caracteres digitada.</span><span class="sxs-lookup"><span data-stu-id="addbe-266">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="addbe-267">Para facilitar a leitura, elas não incluem a codificação de URL necessária.</span><span class="sxs-lookup"><span data-stu-id="addbe-267">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="addbe-268">O exemplo a seguir mostra um filtro que procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="addbe-268">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="addbe-269">O **id** correspondente à cadeia de caracteres `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="addbe-269">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="addbe-270">Sendo o **valor** o GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="addbe-270">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="addbe-271">Para comparar o valor da propriedade com um GUID, converta o `ep/value` para `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="addbe-271">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="addbe-272">O próximo exemplo mostra um filtro que procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="addbe-272">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="addbe-273">O **id** correspondente à cadeia de caracteres `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="addbe-273">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="addbe-274">O **valor** igual inteiro 12.</span><span class="sxs-lookup"><span data-stu-id="addbe-274">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="addbe-275">Para comparar o valor da propriedade com um número inteiro, converta o `ep/value` para `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="addbe-275">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="addbe-276">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="addbe-276">Response 4</span></span>

<span data-ttu-id="addbe-277">Para cada um dos dois exemplos anteriores, uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK`, e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro.</span><span class="sxs-lookup"><span data-stu-id="addbe-277">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="addbe-278">O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="addbe-278">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="addbe-279">A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="addbe-279">The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
