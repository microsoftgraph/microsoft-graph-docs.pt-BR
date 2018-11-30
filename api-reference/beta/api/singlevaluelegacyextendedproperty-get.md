---
title: Obter singleValueLegacyExtendedProperty
description: Você pode obter uma instância de recurso único expandida com uma propriedade estendida específica, ou uma coleção de instâncias de recurso
ms.openlocfilehash: 72ae071d2c5c92af02d26af2474c776a5dc1c83c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039610"
---
# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="5e63b-103">Obter singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="5e63b-103">Get singleValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="5e63b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5e63b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e63b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5e63b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e63b-106">Você pode acessar uma instância de recurso único expandida com uma propriedade estendida específica ou uma coleção de instâncias de recurso que incluem as propriedades estendidas que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-106">You can get a single resource instance expanded with a specific extended property, or a collection of resource instances that include extended properties matching a filter.</span></span>

<span data-ttu-id="5e63b-107">Usar o parâmetro de consulta `$expand` permite que você acesse a instância de recurso especificada expandida com uma propriedade estendida específica.</span><span class="sxs-lookup"><span data-stu-id="5e63b-107">Using the query parameter `$expand` allows you to get the specified resource instance expanded with a specific extended property.</span></span> <span data-ttu-id="5e63b-108">Use um `$filter` e um operador `eq` na propriedade **id** para especificar a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="5e63b-108">Use a `$filter` and `eq` operator on the **id** property to specify the extended property.</span></span> <span data-ttu-id="5e63b-109">Atualmente, esta é a única maneira de acessar o objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="5e63b-109">This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object that represents an extended property.</span></span> 

<span data-ttu-id="5e63b-110">Para acessar instâncias de recurso com determinadas propriedades estendidas, use o parâmetro de consulta `$filter` e aplique um operador `eq` na propriedade **id**.</span><span class="sxs-lookup"><span data-stu-id="5e63b-110">To get resource instances that have certain extended properties, use the `$filter` query parameter and apply an `eq` operator on the **id** property.</span></span> <span data-ttu-id="5e63b-111">Além disso, em propriedades estendidas numéricas, aplique um dos seguintes operadores na propriedade **valor**: `eq`, `ne`,`ge`, `gt`, `le` ou `lt`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-111">In addition, for numeric extended properties, apply one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="5e63b-112">Para propriedades estendidas de cadeia de caracteres digitados, aplique um operador `contains`, `startswith`, `eq` ou `ne` em **value**.</span><span class="sxs-lookup"><span data-stu-id="5e63b-112">For string-typed extended properties, apply a `contains`, `startswith`, `eq`, or `ne` operator on **value**.</span></span> 

<span data-ttu-id="5e63b-113">Maiúsculas e minúsculas são diferenciadas ao filtrar o nome de cadeia de caracteres (`Name`) na **id** de uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="5e63b-113">Filtering the string name (`Name`) in the **id** of an extended property is case-sensitive.</span></span> <span data-ttu-id="5e63b-114">Maiúsculas e minúsculas não são diferenciadas ao filtrar a propriedade **value** de uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="5e63b-114">Filtering the **value** property of an extended property is case-insensitive.</span></span>

<span data-ttu-id="5e63b-115">Há suporte para os seguintes recursos de usuário:</span><span class="sxs-lookup"><span data-stu-id="5e63b-115">The following user resources are supported:</span></span>

- [<span data-ttu-id="5e63b-116">calendar</span><span class="sxs-lookup"><span data-stu-id="5e63b-116">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="5e63b-117">contact</span><span class="sxs-lookup"><span data-stu-id="5e63b-117">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="5e63b-118">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5e63b-118">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="5e63b-119">evento</span><span class="sxs-lookup"><span data-stu-id="5e63b-119">event</span></span>](../resources/event.md)
- [<span data-ttu-id="5e63b-120">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5e63b-120">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="5e63b-121">message</span><span class="sxs-lookup"><span data-stu-id="5e63b-121">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="5e63b-122">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="5e63b-122">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="5e63b-123">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="5e63b-123">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="5e63b-124">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="5e63b-124">As well as the following group resources:</span></span>

- <span data-ttu-id="5e63b-125">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="5e63b-125">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="5e63b-126">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="5e63b-126">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="5e63b-127">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="5e63b-127">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="5e63b-128">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="5e63b-128">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e63b-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e63b-129">Permissions</span></span>
<span data-ttu-id="5e63b-130">Dependendo do recurso estiver recebendo a propriedade estendida da e a permissão digite (delegada ou aplicativos) você solicitação, a permissão especificada na tabela a seguir é o mínimo necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5e63b-130">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="5e63b-131">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e63b-131">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e63b-132">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="5e63b-132">Supported resource</span></span> | <span data-ttu-id="5e63b-133">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e63b-133">Delegated (work or school account)</span></span> | <span data-ttu-id="5e63b-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e63b-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e63b-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e63b-135">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="5e63b-136">calendar</span><span class="sxs-lookup"><span data-stu-id="5e63b-136">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="5e63b-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-137">Calendars.Read</span></span> | <span data-ttu-id="5e63b-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-138">Calendars.Read</span></span> | <span data-ttu-id="5e63b-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-139">Calendars.Read</span></span> |
| [<span data-ttu-id="5e63b-140">contato</span><span class="sxs-lookup"><span data-stu-id="5e63b-140">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5e63b-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-141">Contacts.Read</span></span> | <span data-ttu-id="5e63b-142">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-142">Contacts.Read</span></span> | <span data-ttu-id="5e63b-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-143">Contacts.Read</span></span> |
| [<span data-ttu-id="5e63b-144">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5e63b-144">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="5e63b-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-145">Contacts.Read</span></span> | <span data-ttu-id="5e63b-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-146">Contacts.Read</span></span> | <span data-ttu-id="5e63b-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-147">Contacts.Read</span></span> |
| [<span data-ttu-id="5e63b-148">evento</span><span class="sxs-lookup"><span data-stu-id="5e63b-148">event</span></span>](../resources/event.md) | <span data-ttu-id="5e63b-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-149">Calendars.Read</span></span> | <span data-ttu-id="5e63b-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-150">Calendars.Read</span></span> |  <span data-ttu-id="5e63b-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-151">Calendars.Read</span></span>|
| <span data-ttu-id="5e63b-152">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="5e63b-152">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="5e63b-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e63b-153">Group.Read.All</span></span> | <span data-ttu-id="5e63b-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e63b-154">Not supported</span></span> | <span data-ttu-id="5e63b-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e63b-155">Not supported</span></span> |
| <span data-ttu-id="5e63b-156">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="5e63b-156">group [event](../resources/event.md)</span></span> | <span data-ttu-id="5e63b-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e63b-157">Group.Read.All</span></span> | <span data-ttu-id="5e63b-158">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e63b-158">Not supported</span></span> | <span data-ttu-id="5e63b-159">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e63b-159">Not supported</span></span> |
| <span data-ttu-id="5e63b-160">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="5e63b-160">group [post](../resources/post.md)</span></span> | <span data-ttu-id="5e63b-161">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e63b-161">Group.Read.All</span></span> | <span data-ttu-id="5e63b-162">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e63b-162">Not supported</span></span> | <span data-ttu-id="5e63b-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e63b-163">Group.Read.All</span></span> |
| [<span data-ttu-id="5e63b-164">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5e63b-164">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="5e63b-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-165">Mail.Read</span></span> | <span data-ttu-id="5e63b-166">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-166">Mail.Read</span></span> | <span data-ttu-id="5e63b-167">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-167">Mail.Read</span></span> |
| [<span data-ttu-id="5e63b-168">message</span><span class="sxs-lookup"><span data-stu-id="5e63b-168">message</span></span>](../resources/message.md) | <span data-ttu-id="5e63b-169">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-169">Mail.Read</span></span> | <span data-ttu-id="5e63b-170">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-170">Mail.Read</span></span> | <span data-ttu-id="5e63b-171">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-171">Mail.Read</span></span> |
| [<span data-ttu-id="5e63b-172">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="5e63b-172">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="5e63b-173">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-173">Tasks.Read</span></span> | <span data-ttu-id="5e63b-174">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-174">Tasks.Read</span></span> | <span data-ttu-id="5e63b-175">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e63b-175">Not supported</span></span> |
| [<span data-ttu-id="5e63b-176">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="5e63b-176">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="5e63b-177">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-177">Tasks.Read</span></span> | <span data-ttu-id="5e63b-178">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5e63b-178">Tasks.Read</span></span> | <span data-ttu-id="5e63b-179">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5e63b-179">Not supported</span></span> |


## <a name="http-request"></a><span data-ttu-id="5e63b-180">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e63b-180">HTTP request</span></span>

#### <a name="get-a-resource-instance-expanded-with-an-extended-property-that-matches-a-filter"></a><span data-ttu-id="5e63b-181">Instância de recurso GET expandida com uma propriedade estendida que corresponde a um filtro</span><span class="sxs-lookup"><span data-stu-id="5e63b-181">GET a resource instance expanded with an extended property that matches a filter</span></span>
<span data-ttu-id="5e63b-p106">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-p106">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="5e63b-184">Obtenha uma instância de **mensagem** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-184">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5e63b-185">Obtenha uma instância de **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-185">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5e63b-186">Obtenha uma instância do **evento** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-186">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5e63b-187">Obtenha uma instância de **calendário** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-187">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5e63b-188">Obtenha uma instância de **contato** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-188">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5e63b-189">Obtenha uma instância de **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-189">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5e63b-190">Obtenha uma instância de **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-190">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5e63b-191">Obtenha uma instância de **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-191">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5e63b-192">Obtenha uma instância de **evento** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-192">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5e63b-193">Obtenha uma instância de **postagem** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-193">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-that-include-numeric-extended-properties-matching-a-filter"></a><span data-ttu-id="5e63b-194">Instâncias de recurso GET que incluem as propriedades estendidas numéricas que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-194">GET resource instances that include numeric extended properties matching a filter</span></span>

<span data-ttu-id="5e63b-195">Acesse as instâncias de um recurso com suporte que têm uma propriedade estendida numérica que corresponde a um filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-195">Get instances of a supported resource that have a numeric extended property matching a filter.</span></span> <span data-ttu-id="5e63b-196">O filtro usa um operador `eq` na propriedade **id** e um dos seguintes operadores na propriedade **value**: `eq`, `ne`,`ge`, `gt`, `le` ou `lt`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-196">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `eq`, `ne`,`ge`, `gt`, `le`, or `lt`.</span></span> <span data-ttu-id="5e63b-197">Certificar-se de que você aplicar tornar certeza de que você aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) para os seguintes caracteres na cadeia de caracteres de filtro - e-vírgula, barra invertida e espaço.</span><span class="sxs-lookup"><span data-stu-id="5e63b-197">Make sure you apply Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>

<span data-ttu-id="5e63b-198">As linhas de sintaxe a seguir mostram um filtro que usa um operador `eq` na id e outro operador `eq` no valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="5e63b-198">The following syntax lines show a filter that uses an `eq` operator on the id, and another `eq` operator on the property value.</span></span> <span data-ttu-id="5e63b-199">Você pode substituir o operador `eq` no **value** por qualquer um dos outros operadores (`ne`,`ge`, `gt`, `le` ou `lt`) que se aplicam aos valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="5e63b-199">You can substitute the `eq` operator on the **value** by any one of the other operators (`ne`,`ge`, `gt`, `le`, or `lt`) that apply to numeric values.</span></span>

<span data-ttu-id="5e63b-200">Obtenha as instâncias de **mensagem** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-200">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5e63b-201">Obtenha as instâncias de **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-201">Get **mailFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="5e63b-202">Obtenha as instâncias de **evento** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-202">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5e63b-203">Obtenha as instâncias de **calendário** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-203">Get **calendar** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5e63b-204">Obtenha as instâncias de **contato** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-204">Get **contact** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5e63b-205">Obtenha as instâncias de **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-205">Get **contactFolder** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="5e63b-206">Obtenha uma instância de **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-206">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="5e63b-207">Obtenha uma instância de **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-207">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="5e63b-208">Obtenha as instâncias de **eventos** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-208">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="5e63b-209">Obtenha as instâncias de **postagem** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-209">Get group **post** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

#### <a name="get-resource-instances-with-string-typed-extended-properties-matching-a-filter"></a><span data-ttu-id="5e63b-210">Instâncias de recurso GET com propriedades estendidas de cadeia de caracteres digitados que correspondem a um filtro</span><span class="sxs-lookup"><span data-stu-id="5e63b-210">GET resource instances with string-typed extended properties matching a filter</span></span>

<span data-ttu-id="5e63b-211">Acesse as instâncias do recurso **message** ou **event** que têm uma propriedade estendida de cadeia de caracteres digitados que correspondem a um filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-211">Get instances of the **message** or **event** resource that have a string-typed extended property matching a filter.</span></span> <span data-ttu-id="5e63b-212">O filtro usa um operador `eq` na propriedade **id** e um dos seguintes operadores na propriedade **valor**: `contains`, `startswith`, `eq` ou `ne`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-212">The filter uses an `eq` operator on the **id** property, and one of the following operators on the **value** property: `contains`, `startswith`, `eq`, or `ne`.</span></span> <span data-ttu-id="5e63b-213">Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos seguintes caracteres na cadeia de filtro: dois pontos, barra inclinada e espaço.</span><span class="sxs-lookup"><span data-stu-id="5e63b-213">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - colon, forward slash, and space.</span></span>


<span data-ttu-id="5e63b-214">Obtenha as instâncias de **mensagem** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-214">Get **message** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="5e63b-215">Obtenha as instâncias de **evento** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-215">Get **event** instances: <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="5e63b-216">Obtenha as instâncias de **eventos** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="5e63b-216">Get group **event** instances: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and contains(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and startswith(ep/value, '{property_value}'))
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value ne '{property_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="5e63b-217">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="5e63b-217">Path parameters</span></span>
|<span data-ttu-id="5e63b-218">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="5e63b-218">**Parameter**</span></span>|<span data-ttu-id="5e63b-219">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="5e63b-219">**Type**</span></span>|<span data-ttu-id="5e63b-220">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5e63b-220">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5e63b-221">id_value</span><span class="sxs-lookup"><span data-stu-id="5e63b-221">id_value</span></span>|<span data-ttu-id="5e63b-222">String</span><span class="sxs-lookup"><span data-stu-id="5e63b-222">String</span></span>|<span data-ttu-id="5e63b-p110">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e63b-p110">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="5e63b-227">property_value</span><span class="sxs-lookup"><span data-stu-id="5e63b-227">property_value</span></span> |<span data-ttu-id="5e63b-228">String</span><span class="sxs-lookup"><span data-stu-id="5e63b-228">String</span></span>|<span data-ttu-id="5e63b-229">O valor da propriedade estendida a ser correspondida.</span><span class="sxs-lookup"><span data-stu-id="5e63b-229">The value of the extended property to match.</span></span> <span data-ttu-id="5e63b-230">Obrigatório quando indicado na seção **Solicitação HTTP** acima.</span><span class="sxs-lookup"><span data-stu-id="5e63b-230">Required where listed in the **HTTP request** section above.</span></span> <span data-ttu-id="5e63b-231">Se {property_value} não for uma cadeia de caracteres, converta o `ep/value` para o tipo de dado Edm apropriado ao compará-lo com {property_value}.</span><span class="sxs-lookup"><span data-stu-id="5e63b-231">If {property_value} is not a string, make sure you explicitly cast `ep/value` to the appropriate Edm data type when comparing it with {property_value}.</span></span> <span data-ttu-id="5e63b-232">Confira exemplos na [solicitação 4](#request-4) abaixo.</span><span class="sxs-lookup"><span data-stu-id="5e63b-232">See [request 4](#request-4) below for examples.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5e63b-233">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e63b-233">Request headers</span></span>
| <span data-ttu-id="5e63b-234">Nome</span><span class="sxs-lookup"><span data-stu-id="5e63b-234">Name</span></span>      |<span data-ttu-id="5e63b-235">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e63b-235">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e63b-236">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e63b-236">Authorization</span></span>  | <span data-ttu-id="5e63b-p112">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e63b-p112">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e63b-239">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e63b-239">Request body</span></span>
<span data-ttu-id="5e63b-240">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e63b-240">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e63b-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e63b-241">Response</span></span>

<span data-ttu-id="5e63b-242">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-242">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="5e63b-243">OBTER instância de recurso usando `$expand`</span><span class="sxs-lookup"><span data-stu-id="5e63b-243">GET resource instance using `$expand`</span></span>
<span data-ttu-id="5e63b-244">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="5e63b-244">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-that-contain-an-extended-property-matching-a-filter"></a><span data-ttu-id="5e63b-245">Instâncias de recurso GET que contenham uma propriedade estendida correspondente a um filtro</span><span class="sxs-lookup"><span data-stu-id="5e63b-245">GET resource instances that contain an extended property matching a filter</span></span>
<span data-ttu-id="5e63b-246">O corpo da resposta inclui um ou mais objetos que representam as instâncias de recursos contendo uma propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="5e63b-246">The response body includes one or more objects representing the resource instances that contain a matching extended property.</span></span> <span data-ttu-id="5e63b-247">O corpo da resposta não inclui a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="5e63b-247">The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="5e63b-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e63b-248">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="5e63b-249">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="5e63b-249">Request 1</span></span>

<span data-ttu-id="5e63b-p114">O primeiro exemplo obtém e expande a mensagem especificada, incluindo uma propriedade estendida de valor único. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="5e63b-p114">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
#### <a name="response-1"></a><span data-ttu-id="5e63b-252">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="5e63b-252">Response 1</span></span>
<span data-ttu-id="5e63b-253">O corpo da resposta inclui todas as propriedades da mensagem especificada e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-253">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="5e63b-p115">Observação: O objeto **message** mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e63b-p115">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="5e63b-256">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="5e63b-256">Request 2</span></span>

<span data-ttu-id="5e63b-257">O segundo exemplo obtém mensagens que possuem a propriedade estendida de valor único com cadeia de caracteres digitada especificada no filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-257">The second example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="5e63b-258">O filtro procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="5e63b-258">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="5e63b-259">**id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação aqui removida para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="5e63b-259">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="5e63b-260">O **valor** igual à cadeia de caracteres `Green`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-260">Its **value** equal to the string `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

#### <a name="response-2"></a><span data-ttu-id="5e63b-261">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="5e63b-261">Response 2</span></span>

<span data-ttu-id="5e63b-p117">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK`, e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro. O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md). A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="5e63b-p117">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user-list-messages.md). The response does not include the matching extended property.</span></span>


#### <a name="request-3"></a><span data-ttu-id="5e63b-265">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="5e63b-265">Request 3</span></span>

<span data-ttu-id="5e63b-266">O terceiro exemplo obtém mensagens que possuem a propriedade estendida de valor único com cadeia de caracteres digitada especificada no filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-266">The third example gets messages that have the string-typed single-value extended property specified in the filter.</span></span> <span data-ttu-id="5e63b-267">O filtro procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="5e63b-267">The filter looks for the extended property that has:</span></span>

- <span data-ttu-id="5e63b-268">**id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação aqui removida para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="5e63b-268">Its **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

- <span data-ttu-id="5e63b-269">O **value** que contém a cadeia de caracteres `green`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-269">Its **value** containing the string `green`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/Me/messages?$filter=singleValueExtendedProperties/any(ep:ep/Id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color' and contains(ep/Value, 'green'))
```

#### <a name="response-3"></a><span data-ttu-id="5e63b-270">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="5e63b-270">Response 3</span></span>

<span data-ttu-id="5e63b-271">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK` e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-271">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter.</span></span> <span data-ttu-id="5e63b-272">Por exemplo, uma mensagem com uma propriedade estendida de valor único com a **id** igual à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` e ao **value** `Light green` corresponderia ao filtro e seria incluída na resposta.</span><span class="sxs-lookup"><span data-stu-id="5e63b-272">For example, a message that has a single-value extended property with the **id** equal to the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color`, and the **value** `Light green`, would match the filter and be included in the response.</span></span>

<span data-ttu-id="5e63b-273">O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="5e63b-273">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="5e63b-274">A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="5e63b-274">The response does not include the matching extended property.</span></span>


#### <a name="request-4"></a><span data-ttu-id="5e63b-275">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="5e63b-275">Request 4</span></span>

<span data-ttu-id="5e63b-276">Os próximos dois exemplos mostram como acessar mensagens que possuam propriedades estendidas de valor único sem cadeia de caracteres digitada.</span><span class="sxs-lookup"><span data-stu-id="5e63b-276">The next 2 examples show how to get messages that have non-string typed single-value extended properties.</span></span> <span data-ttu-id="5e63b-277">Para facilitar a leitura, elas não incluem a codificação de URL necessária.</span><span class="sxs-lookup"><span data-stu-id="5e63b-277">For ease of reading, they do not include the necessary URL encoding.</span></span>

<span data-ttu-id="5e63b-278">O exemplo a seguir mostra um filtro que procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="5e63b-278">The following example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="5e63b-279">O **id** correspondente à cadeia de caracteres `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-279">Its **id** matching the string `CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid`.</span></span>

- <span data-ttu-id="5e63b-280">Sendo o **valor** o GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-280">Its **value** being the GUID `b9cf8971-7d55-4b73-9ffa-a584611b600b`.</span></span> <span data-ttu-id="5e63b-281">Para comparar o valor da propriedade com um GUID, converta o `ep/value` para `Edm.Guid`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-281">To compare the property value with a GUID, cast `ep/value` to `Edm.Guid`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'CLSID {00062008-0000-0000-C000-000000000046} Name ConnectorSenderGuid' and cast(ep/value, Edm.Guid) eq (b9cf8971-7d55-4b73-9ffa-a584611b600b))
```

<span data-ttu-id="5e63b-282">O próximo exemplo mostra um filtro que procura a propriedade estendida com:</span><span class="sxs-lookup"><span data-stu-id="5e63b-282">The next example shows a filter that looks for the extended property that has:</span></span>

- <span data-ttu-id="5e63b-283">O **id** correspondente à cadeia de caracteres `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-283">Its **id** matching the string `Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete`.</span></span>

- <span data-ttu-id="5e63b-284">O **valor** igual inteiro 12.</span><span class="sxs-lookup"><span data-stu-id="5e63b-284">Its **value** equal to the integer 12.</span></span> <span data-ttu-id="5e63b-285">Para comparar o valor da propriedade com um número inteiro, converta o `ep/value` para `Edm.Int32`.</span><span class="sxs-lookup"><span data-stu-id="5e63b-285">To compare the property value with an integer, cast `ep/value` to `Edm.Int32`.</span></span>


<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=singleValueExtendedProperties/any(ep:ep/id eq 'Integer {66f5a359-4659-4830-9070-00047ec6ac6e} Name Pallete' and cast(ep/value, Edm.Int32) eq 12)
```


#### <a name="response-4"></a><span data-ttu-id="5e63b-286">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="5e63b-286">Response 4</span></span>

<span data-ttu-id="5e63b-287">Para cada um dos dois exemplos anteriores, uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK`, e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro.</span><span class="sxs-lookup"><span data-stu-id="5e63b-287">For each of the preceding 2 examples, a successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the corresponding filter.</span></span> <span data-ttu-id="5e63b-288">O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user-list-messages.md).</span><span class="sxs-lookup"><span data-stu-id="5e63b-288">The response body is similar to the response from [getting a message collection](../api/user-list-messages.md).</span></span> <span data-ttu-id="5e63b-289">A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="5e63b-289">The response does not include the matching extended property.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->