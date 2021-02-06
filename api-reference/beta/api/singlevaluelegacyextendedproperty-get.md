---
title: Obter singleValueLegacyExtendedProperty
description: Você pode obter uma única instância de recurso expandida com uma propriedade estendida específica ou uma coleção de instâncias de recursos
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: dedb7eefacd028a837c39b3712ec6f61e0ee032f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134089"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="1d515-103">Obter singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1d515-103">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="1d515-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d515-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="1d515-105">Você pode acessar uma instância de recurso único expandida com uma propriedade estendida específica ou uma coleção de instâncias de recurso que incluem as propriedades estendidas que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-105">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="1d515-106">Usar o parâmetro de consulta `$expand` permite que você acesse a instância de recurso especificada expandida com uma propriedade estendida específica.</span><span class="sxs-lookup"><span data-stu-id="1d515-106">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="1d515-107">Use um `$filter` e um operador `eq` na propriedade **id** para especificar a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="1d515-107">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="1d515-108">Atualmente, esta é a única maneira de acessar o objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="1d515-108">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="1d515-109">Para acessar instâncias de recurso com determinadas propriedades estendidas, use o parâmetro de consulta `$filter` e aplique um operador `eq` na propriedade **id**.</span><span class="sxs-lookup"><span data-stu-id="1d515-109">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="1d515-110">Além disso, em propriedades estendidas numéricas, aplique um dos seguintes operadores na propriedade **valor**: `eq`, `ne`,`ge`, `gt`, `le` ou `lt`.</span><span class="sxs-lookup"><span data-stu-id="1d515-110">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="1d515-111">Para propriedades estendidas de cadeia de caracteres digitados, aplique um operador `contains`, `startswith`, `eq` ou `ne` em **value**.</span><span class="sxs-lookup"><span data-stu-id="1d515-111">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span>

<span data-ttu-id="1d515-112">Maiúsculas e minúsculas são diferenciadas ao filtrar o nome de cadeia de caracteres (`Name`) na **id** de uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="1d515-112">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="1d515-113">Maiúsculas e minúsculas não são diferenciadas ao filtrar a propriedade **value** de uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="1d515-113">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="1d515-114">Há suporte para os seguintes recursos de usuário:</span><span class="sxs-lookup"><span data-stu-id="1d515-114">The following user resources are supported:</span></span>

- [<span data-ttu-id="1d515-115">calendar</span><span class="sxs-lookup"><span data-stu-id="1d515-115">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="1d515-116">contact</span><span class="sxs-lookup"><span data-stu-id="1d515-116">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="1d515-117">contactFolder</span><span class="sxs-lookup"><span data-stu-id="1d515-117">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="1d515-118">evento</span><span class="sxs-lookup"><span data-stu-id="1d515-118">event</span></span>](../resources/event.md)
- [<span data-ttu-id="1d515-119">mailFolder</span><span class="sxs-lookup"><span data-stu-id="1d515-119">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="1d515-120">message</span><span class="sxs-lookup"><span data-stu-id="1d515-120">message</span></span>](../resources/message.md)
- [<span data-ttu-id="1d515-121">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="1d515-121">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="1d515-122">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="1d515-122">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="1d515-123">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="1d515-123">As well as the following group resources:</span></span>

- <span data-ttu-id="1d515-124">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="1d515-124">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="1d515-125">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="1d515-125">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="1d515-126">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="1d515-126">group [post](../resources/post.md)</span></span>

<span data-ttu-id="1d515-127">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="1d515-127">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d515-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d515-128">Permissions</span></span>
<span data-ttu-id="1d515-129">Dependendo do recurso do qual você está recebendo a propriedade estendida e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1d515-129">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="1d515-130">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d515-130">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d515-131">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="1d515-131">Supported resource</span></span> | <span data-ttu-id="1d515-132">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d515-132">Delegated (work or school account)</span></span> | <span data-ttu-id="1d515-133">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d515-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d515-134">Application</span><span class="sxs-lookup"><span data-stu-id="1d515-134">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="1d515-135">calendar</span><span class="sxs-lookup"><span data-stu-id="1d515-135">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="1d515-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-136">Calendars.Read</span></span> | <span data-ttu-id="1d515-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-137">Calendars.Read</span></span> | <span data-ttu-id="1d515-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-138">Calendars.Read</span></span> |
| [<span data-ttu-id="1d515-139">contato</span><span class="sxs-lookup"><span data-stu-id="1d515-139">contact</span></span>](../resources/contact.md) | <span data-ttu-id="1d515-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-140">Contacts.Read</span></span> | <span data-ttu-id="1d515-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-141">Contacts.Read</span></span> | <span data-ttu-id="1d515-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-142">Contacts.Read</span></span> |
| [<span data-ttu-id="1d515-143">contactFolder</span><span class="sxs-lookup"><span data-stu-id="1d515-143">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="1d515-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-144">Contacts.Read</span></span> | <span data-ttu-id="1d515-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-145">Contacts.Read</span></span> | <span data-ttu-id="1d515-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-146">Contacts.Read</span></span> |
| [<span data-ttu-id="1d515-147">evento</span><span class="sxs-lookup"><span data-stu-id="1d515-147">event</span></span>](../resources/event.md) | <span data-ttu-id="1d515-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-148">Calendars.Read</span></span> | <span data-ttu-id="1d515-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-149">Calendars.Read</span></span> |  <span data-ttu-id="1d515-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-150">Calendars.Read</span></span>|
| <span data-ttu-id="1d515-151">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="1d515-151">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="1d515-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d515-152">Group.Read.All</span></span> | <span data-ttu-id="1d515-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1d515-153">Not supported</span></span> | <span data-ttu-id="1d515-154">Incompatível</span><span class="sxs-lookup"><span data-stu-id="1d515-154">Not supported</span></span> |
| <span data-ttu-id="1d515-155">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="1d515-155">group [event](../resources/event.md)</span></span> | <span data-ttu-id="1d515-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d515-156">Group.Read.All</span></span> | <span data-ttu-id="1d515-157">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1d515-157">Not supported</span></span> | <span data-ttu-id="1d515-158">Incompatível</span><span class="sxs-lookup"><span data-stu-id="1d515-158">Not supported</span></span> |
| <span data-ttu-id="1d515-159">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="1d515-159">group [post](../resources/post.md)</span></span> | <span data-ttu-id="1d515-160">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d515-160">Group.Read.All</span></span> | <span data-ttu-id="1d515-161">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1d515-161">Not supported</span></span> | <span data-ttu-id="1d515-162">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d515-162">Group.Read.All</span></span> |
| [<span data-ttu-id="1d515-163">mailFolder</span><span class="sxs-lookup"><span data-stu-id="1d515-163">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="1d515-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-164">Mail.Read</span></span> | <span data-ttu-id="1d515-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-165">Mail.Read</span></span> | <span data-ttu-id="1d515-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-166">Mail.Read</span></span> |
| [<span data-ttu-id="1d515-167">message</span><span class="sxs-lookup"><span data-stu-id="1d515-167">message</span></span>](../resources/message.md) | <span data-ttu-id="1d515-168">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-168">Mail.Read</span></span> | <span data-ttu-id="1d515-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-169">Mail.Read</span></span> | <span data-ttu-id="1d515-170">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-170">Mail.Read</span></span> |
| [<span data-ttu-id="1d515-171">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="1d515-171">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="1d515-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-172">Tasks.Read</span></span> | <span data-ttu-id="1d515-173">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-173">Tasks.Read</span></span> | <span data-ttu-id="1d515-174">Incompatível</span><span class="sxs-lookup"><span data-stu-id="1d515-174">Not supported</span></span> |
| [<span data-ttu-id="1d515-175">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="1d515-175">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="1d515-176">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-176">Tasks.Read</span></span> | <span data-ttu-id="1d515-177">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1d515-177">Tasks.Read</span></span> | <span data-ttu-id="1d515-178">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1d515-178">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="1d515-179">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d515-179">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="1d515-180">Instância de recurso GET expandida com uma propriedade estendida que corresponde a um filtro</span><span class="sxs-lookup"><span data-stu-id="1d515-180">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="1d515-p105">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-p105">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="1d515-183">Obtenha uma instância de **message**:</span><span class="sxs-lookup"><span data-stu-id="1d515-183">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1d515-184">Obtenha uma instância de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="1d515-184">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1d515-185">Obtenha uma instância de **event**:</span><span class="sxs-lookup"><span data-stu-id="1d515-185">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1d515-186">Obtenha uma instância de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="1d515-186">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1d515-187">Obtenha uma instância de **contact**:</span><span class="sxs-lookup"><span data-stu-id="1d515-187">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1d515-188">Obtenha uma instância de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="1d515-188">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1d515-189">Obter uma **instância do outlookTask:**</span><span class="sxs-lookup"><span data-stu-id="1d515-189">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1d515-190">Obter uma **instância do outlookTaskFolder:**</span><span class="sxs-lookup"><span data-stu-id="1d515-190">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1d515-191">Obtenha uma instância de **group event**:</span><span class="sxs-lookup"><span data-stu-id="1d515-191">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1d515-192">Acesse uma instância de **postar** em grupo:</span><span class="sxs-lookup"><span data-stu-id="1d515-192">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="1d515-193">Instâncias de recurso GET que incluem as propriedades estendidas numéricas que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-193">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="1d515-194">Acesse as instâncias de um recurso com suporte que têm uma propriedade estendida numérica que corresponde a um filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-194">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="1d515-195">O filtro usa um operador `eq` na propriedade **id** e um dos seguintes operadores na propriedade **value**: `eq`, `ne`,`ge`, `gt`, `le` ou `lt`.</span><span class="sxs-lookup"><span data-stu-id="1d515-195">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span>
<span data-ttu-id="1d515-196">Certifique-se de aplicar a codificação [de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos seguintes caracteres na cadeia de caracteres de filtro - dois-pontos, barra e espaço.</span><span class="sxs-lookup"><span data-stu-id="1d515-196">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="1d515-197">As linhas de sintaxe a seguir mostram um filtro que usa um operador `eq` na id e outro operador `eq` no valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="1d515-197">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="1d515-198">Você pode substituir o operador `eq` no **value** por qualquer um dos outros operadores (`ne`,`ge`, `gt`, `le` ou `lt`) que se aplicam aos valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="1d515-198">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="1d515-199">Acesse as instâncias de **mensagem**:</span><span class="sxs-lookup"><span data-stu-id="1d515-199">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1d515-200">Acesse as instâncias de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="1d515-200">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="1d515-201">Acesse as instâncias de **event**:</span><span class="sxs-lookup"><span data-stu-id="1d515-201">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1d515-202">Acesse as instâncias de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="1d515-202">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1d515-203">Acesse as instâncias de **contact**:</span><span class="sxs-lookup"><span data-stu-id="1d515-203">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1d515-204">Acesse as instâncias de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="1d515-204">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="1d515-205">Obter uma **instância do outlookTask:**</span><span class="sxs-lookup"><span data-stu-id="1d515-205">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1d515-206">Obter uma **instância do outlookTaskFolder:**</span><span class="sxs-lookup"><span data-stu-id="1d515-206">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="1d515-207">Acesse as instâncias de **group event**:</span><span class="sxs-lookup"><span data-stu-id="1d515-207">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="1d515-208">Acesse as instâncias de **postar** em grupo:</span><span class="sxs-lookup"><span data-stu-id="1d515-208">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="1d515-209">Instâncias de recurso GET com propriedades estendidas de cadeia de caracteres digitados que correspondem a um filtro</span><span class="sxs-lookup"><span data-stu-id="1d515-209">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="1d515-210">Acesse as instâncias do recurso **message** ou **event** que têm uma propriedade estendida de cadeia de caracteres digitados que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-210">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="1d515-211">O filtro usa um operador `eq` na propriedade **id** e um dos seguintes operadores na propriedade **valor**: `contains`, `startswith`, `eq` ou `ne`.</span><span class="sxs-lookup"><span data-stu-id="1d515-211">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="1d515-212">Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos seguintes caracteres na cadeia de filtro: dois pontos, barra inclinada e espaço.</span><span class="sxs-lookup"><span data-stu-id="1d515-212">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="1d515-213">Acesse as instâncias de **mensagem**:</span><span class="sxs-lookup"><span data-stu-id="1d515-213">Get **message** instances:</span></span>
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

<span data-ttu-id="1d515-214">Acesse as instâncias de **event**:</span><span class="sxs-lookup"><span data-stu-id="1d515-214">Get **event** instances:</span></span>
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

<span data-ttu-id="1d515-215">Acesse as instâncias de **group event**:</span><span class="sxs-lookup"><span data-stu-id="1d515-215">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="1d515-216">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1d515-216">Path parameters</span></span>
|<span data-ttu-id="1d515-217">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="1d515-217">**Parameter**</span></span>|<span data-ttu-id="1d515-218">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="1d515-218">**Type**</span></span>|<span data-ttu-id="1d515-219">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1d515-219">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1d515-220">id_value</span><span class="sxs-lookup"><span data-stu-id="1d515-220">id_value</span></span>|<span data-ttu-id="1d515-221">String</span><span class="sxs-lookup"><span data-stu-id="1d515-221">String</span></span>|<span data-ttu-id="1d515-p109">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d515-p109">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="1d515-226">property_value</span><span class="sxs-lookup"><span data-stu-id="1d515-226">property_value</span></span> |<span data-ttu-id="1d515-227">String</span><span class="sxs-lookup"><span data-stu-id="1d515-227">String</span></span>|<span data-ttu-id="1d515-228">O valor da propriedade estendida a ser correspondida.</span><span class="sxs-lookup"><span data-stu-id="1d515-228">The value of the extended property to match.</span></span> <span data-ttu-id="1d515-229">Obrigatório quando indicado na seção **Solicitação HTTP** acima.</span><span class="sxs-lookup"><span data-stu-id="1d515-229">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="1d515-230">Se {property_value} não for uma cadeia de caracteres, converta o `ep/value` para o tipo de dado Edm apropriado ao compará-lo com {property_value}.</span><span class="sxs-lookup"><span data-stu-id="1d515-230">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="1d515-231">Confira exemplos na [solicitação 4](#request-4) abaixo.</span><span class="sxs-lookup"><span data-stu-id="1d515-231">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1d515-232">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d515-232">Request headers</span></span>
| <span data-ttu-id="1d515-233">Nome</span><span class="sxs-lookup"><span data-stu-id="1d515-233">Name</span></span>      |<span data-ttu-id="1d515-234">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d515-234">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1d515-235">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d515-235">Authorization</span></span>  | <span data-ttu-id="1d515-p111">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d515-p111">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d515-238">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d515-238">Request body</span></span>
<span data-ttu-id="1d515-239">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d515-239">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d515-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d515-240">Response</span></span>

<span data-ttu-id="1d515-241">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1d515-241">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="1d515-242">OBTER instância de recurso usando `$expand`</span><span class="sxs-lookup"><span data-stu-id="1d515-242">GET resource instance using `$expand`</span></span>
<span data-ttu-id="1d515-243">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="1d515-243">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>

#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="1d515-244">Instâncias de recurso GET que contenham uma propriedade estendida correspondente a um filtro</span><span class="sxs-lookup"><span data-stu-id="1d515-244">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="1d515-245">O corpo da resposta inclui um ou mais objetos que representam as instâncias de recursos contendo uma propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="1d515-245">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="1d515-246">O corpo da resposta não inclui a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="1d515-246">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="1d515-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d515-247">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="1d515-248">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="1d515-248">Request 1</span></span>

<span data-ttu-id="1d515-p113">O primeiro exemplo obtém e expande a mensagem especificada, incluindo uma propriedade estendida de valor único. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="1d515-p113">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>


# <a name="http"></a>[<span data-ttu-id="1d515-251">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d515-251">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=/?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
# <a name="c"></a>[<span data-ttu-id="1d515-252">C#</span><span class="sxs-lookup"><span data-stu-id="1d515-252">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-singlevaluelegacyextendedproperty-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d515-253">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d515-253">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-singlevaluelegacyextendedproperty-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d515-254">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d515-254">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-singlevaluelegacyextendedproperty-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d515-255">Java</span><span class="sxs-lookup"><span data-stu-id="1d515-255">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-singlevaluelegacyextendedproperty-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response-1"></a><span data-ttu-id="1d515-256">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="1d515-256">Response 1</span></span>
<span data-ttu-id="1d515-257">O corpo da resposta inclui todas as propriedades da mensagem especificada e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-257">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="1d515-p114">Observação: O objeto **message** mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d515-p114">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
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
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

#### <a name="request-2"></a><span data-ttu-id="1d515-260">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="1d515-260">Request 2</span></span>

<span data-ttu-id="1d515-261">O segundo exemplo obtém mensagens que possuem a propriedade estendida de valor único com cadeia de caracteres digitada especificada no filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-261">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="1d515-262">O filtro procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="1d515-262">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="1d515-263">**id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação aqui removida para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="1d515-263">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="1d515-264">O **valor** igual à cadeia de caracteres `Green`.</span><span class="sxs-lookup"><span data-stu-id="1d515-264">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="1d515-265">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="1d515-265">Response 2</span></span>

<span data-ttu-id="1d515-p116">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK`, e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro. O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md). A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="1d515-p116">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="1d515-269">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="1d515-269">Request 3</span></span>

<span data-ttu-id="1d515-270">O terceiro exemplo obtém mensagens que possuem a propriedade estendida de valor único com cadeia de caracteres digitada especificada no filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-270">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="1d515-271">O filtro procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="1d515-271">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="1d515-272">**id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação aqui removida para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="1d515-272">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="1d515-273">O **value** que contém a cadeia de caracteres `green`.</span><span class="sxs-lookup"><span data-stu-id="1d515-273">Its **value** containing the string `green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="1d515-274">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="1d515-274">Response 3</span></span>

<span data-ttu-id="1d515-275">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK` e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-275">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="1d515-276">Por exemplo, uma mensagem com uma propriedade estendida de valor único com a **id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` e ao **value** `Light green` corresponderia ao filtro e seria incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="1d515-276">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="1d515-277">O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="1d515-277">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="1d515-278">A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="1d515-278">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="1d515-279">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="1d515-279">Request 4</span></span>

<span data-ttu-id="1d515-280">Os próximos dois exemplos mostram como acessar mensagens que possuam propriedades estendidas de valor único sem cadeia de caracteres digitada.</span><span class="sxs-lookup"><span data-stu-id="1d515-280">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="1d515-281">Para facilitar a leitura, elas não incluem a codificação de URL necessária.</span><span class="sxs-lookup"><span data-stu-id="1d515-281">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="1d515-282">O exemplo a seguir mostra um filtro que procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="1d515-282">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="1d515-283">O **id** correspondente à cadeia de caracteres `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="1d515-283">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="1d515-284">Sendo o **valor** o GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="1d515-284">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="1d515-285">Para comparar o valor da propriedade com um GUID, converta o `ep/value` para `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="1d515-285">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="1d515-286">O próximo exemplo mostra um filtro que procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="1d515-286">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="1d515-287">O **id** correspondente à cadeia de caracteres `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="1d515-287">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="1d515-288">O **valor** igual inteiro 12.</span><span class="sxs-lookup"><span data-stu-id="1d515-288">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="1d515-289">Para comparar o valor da propriedade com um número inteiro, converta o `ep/value` para `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="1d515-289">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="1d515-290">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="1d515-290">Response 4</span></span>

<span data-ttu-id="1d515-291">Para cada um dos dois exemplos anteriores, uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK`, e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro.</span><span class="sxs-lookup"><span data-stu-id="1d515-291">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="1d515-292">O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="1d515-292">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="1d515-293">A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="1d515-293">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


