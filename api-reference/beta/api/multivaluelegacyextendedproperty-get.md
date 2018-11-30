---
title: Obter multiValueLegacyExtendedProperty
description: Expanda '.
ms.openlocfilehash: 9429737f3965acbf4c6bcc61c516327556223111
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038186"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="24ffe-103">Obter multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="24ffe-103">Get multiValueLegacyExtendedProperty</span></span>

> <span data-ttu-id="24ffe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="24ffe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24ffe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="24ffe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24ffe-106">Obtenha uma instância do recurso que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="24ffe-106">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="24ffe-107">Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada.</span><span class="sxs-lookup"><span data-stu-id="24ffe-107">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="24ffe-108">Atualmente, esta é a única maneira de obter o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="24ffe-108">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="24ffe-109">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="24ffe-109">The following user resources are supported:</span></span>

- [<span data-ttu-id="24ffe-110">calendar</span><span class="sxs-lookup"><span data-stu-id="24ffe-110">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="24ffe-111">contact</span><span class="sxs-lookup"><span data-stu-id="24ffe-111">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="24ffe-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="24ffe-112">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="24ffe-113">evento</span><span class="sxs-lookup"><span data-stu-id="24ffe-113">event</span></span>](../resources/event.md)
- [<span data-ttu-id="24ffe-114">mailFolder</span><span class="sxs-lookup"><span data-stu-id="24ffe-114">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="24ffe-115">message</span><span class="sxs-lookup"><span data-stu-id="24ffe-115">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="24ffe-116">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="24ffe-116">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="24ffe-117">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="24ffe-117">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="24ffe-118">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="24ffe-118">As well as the following group resources:</span></span>

- <span data-ttu-id="24ffe-119">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="24ffe-119">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="24ffe-120">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="24ffe-120">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="24ffe-121">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="24ffe-121">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="24ffe-122">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="24ffe-122">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="24ffe-123">Permissões</span><span class="sxs-lookup"><span data-stu-id="24ffe-123">Permissions</span></span>
<span data-ttu-id="24ffe-124">Dependendo do recurso estiver recebendo a propriedade estendida da e a permissão digite (delegada ou aplicativos) você solicitação, a permissão especificada na tabela a seguir é o mínimo necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="24ffe-124">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="24ffe-125">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24ffe-125">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24ffe-126">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="24ffe-126">Supported resource</span></span> | <span data-ttu-id="24ffe-127">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24ffe-127">Delegated (work or school account)</span></span> | <span data-ttu-id="24ffe-128">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24ffe-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24ffe-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24ffe-129">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="24ffe-130">calendar</span><span class="sxs-lookup"><span data-stu-id="24ffe-130">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="24ffe-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-131">Calendars.Read</span></span> | <span data-ttu-id="24ffe-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-132">Calendars.Read</span></span> | <span data-ttu-id="24ffe-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-133">Calendars.Read</span></span> |
| [<span data-ttu-id="24ffe-134">contato</span><span class="sxs-lookup"><span data-stu-id="24ffe-134">contact</span></span>](../resources/contact.md) | <span data-ttu-id="24ffe-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-135">Contacts.Read</span></span> | <span data-ttu-id="24ffe-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-136">Contacts.Read</span></span> | <span data-ttu-id="24ffe-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-137">Contacts.Read</span></span> |
| [<span data-ttu-id="24ffe-138">contactFolder</span><span class="sxs-lookup"><span data-stu-id="24ffe-138">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="24ffe-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-139">Contacts.Read</span></span> | <span data-ttu-id="24ffe-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-140">Contacts.Read</span></span> | <span data-ttu-id="24ffe-141">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-141">Contacts.Read</span></span> |
| [<span data-ttu-id="24ffe-142">evento</span><span class="sxs-lookup"><span data-stu-id="24ffe-142">event</span></span>](../resources/event.md) | <span data-ttu-id="24ffe-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-143">Calendars.Read</span></span> | <span data-ttu-id="24ffe-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-144">Calendars.Read</span></span> |  <span data-ttu-id="24ffe-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-145">Calendars.Read</span></span>|
| <span data-ttu-id="24ffe-146">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="24ffe-146">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="24ffe-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="24ffe-147">Group.Read.All</span></span> | <span data-ttu-id="24ffe-148">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="24ffe-148">Not supported</span></span> | <span data-ttu-id="24ffe-149">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="24ffe-149">Not supported</span></span> |
| <span data-ttu-id="24ffe-150">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="24ffe-150">group [event](../resources/event.md)</span></span> | <span data-ttu-id="24ffe-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="24ffe-151">Group.Read.All</span></span> | <span data-ttu-id="24ffe-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="24ffe-152">Not supported</span></span> | <span data-ttu-id="24ffe-153">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="24ffe-153">Not supported</span></span> |
| <span data-ttu-id="24ffe-154">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="24ffe-154">group [post](../resources/post.md)</span></span> | <span data-ttu-id="24ffe-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="24ffe-155">Group.Read.All</span></span> | <span data-ttu-id="24ffe-156">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="24ffe-156">Not supported</span></span> | <span data-ttu-id="24ffe-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="24ffe-157">Group.Read.All</span></span> |
| [<span data-ttu-id="24ffe-158">mailFolder</span><span class="sxs-lookup"><span data-stu-id="24ffe-158">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="24ffe-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-159">Mail.Read</span></span> | <span data-ttu-id="24ffe-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-160">Mail.Read</span></span> | <span data-ttu-id="24ffe-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-161">Mail.Read</span></span> |
| [<span data-ttu-id="24ffe-162">message</span><span class="sxs-lookup"><span data-stu-id="24ffe-162">message</span></span>](../resources/message.md) | <span data-ttu-id="24ffe-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-163">Mail.Read</span></span> | <span data-ttu-id="24ffe-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-164">Mail.Read</span></span> | <span data-ttu-id="24ffe-165">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-165">Mail.Read</span></span> |
| [<span data-ttu-id="24ffe-166">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="24ffe-166">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="24ffe-167">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-167">Tasks.Read</span></span> | <span data-ttu-id="24ffe-168">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-168">Tasks.Read</span></span> | <span data-ttu-id="24ffe-169">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="24ffe-169">Not supported</span></span> |
| [<span data-ttu-id="24ffe-170">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="24ffe-170">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="24ffe-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-171">Tasks.Read</span></span> | <span data-ttu-id="24ffe-172">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="24ffe-172">Tasks.Read</span></span> | <span data-ttu-id="24ffe-173">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="24ffe-173">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="24ffe-174">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24ffe-174">HTTP request</span></span>

<span data-ttu-id="24ffe-p104">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="24ffe-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="24ffe-177">Obtenha uma instância de **mensagem** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-177">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24ffe-178">Obtenha uma instância de **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-178">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="24ffe-179">Obtenha uma instância do **evento** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-179">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24ffe-180">Obtenha uma instância de **calendário** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-180">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24ffe-181">Obtenha uma instância de **contato** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-181">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24ffe-182">Obtenha uma instância de **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-182">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="24ffe-183">Obtenha uma instância de **outlookTask** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-183">Get an **outlookTask** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="24ffe-184">Obtenha uma instância de **outlookTaskFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-184">Get an **outlookTaskFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="24ffe-185">Obtenha uma instância de **evento** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-185">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="24ffe-186">Obtenha uma instância de **postagem** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="24ffe-186">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="24ffe-187">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="24ffe-187">Path parameters</span></span>
|<span data-ttu-id="24ffe-188">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="24ffe-188">**Parameter**</span></span>|<span data-ttu-id="24ffe-189">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="24ffe-189">**Type**</span></span>|<span data-ttu-id="24ffe-190">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="24ffe-190">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="24ffe-191">id_value</span><span class="sxs-lookup"><span data-stu-id="24ffe-191">id_value</span></span>|<span data-ttu-id="24ffe-192">String</span><span class="sxs-lookup"><span data-stu-id="24ffe-192">String</span></span>|<span data-ttu-id="24ffe-p105">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24ffe-p105">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="24ffe-197">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24ffe-197">Request headers</span></span>
| <span data-ttu-id="24ffe-198">Nome</span><span class="sxs-lookup"><span data-stu-id="24ffe-198">Name</span></span>      |<span data-ttu-id="24ffe-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="24ffe-199">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="24ffe-200">Autorização</span><span class="sxs-lookup"><span data-stu-id="24ffe-200">Authorization</span></span>  | <span data-ttu-id="24ffe-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24ffe-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24ffe-203">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24ffe-203">Request body</span></span>
<span data-ttu-id="24ffe-204">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24ffe-204">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24ffe-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="24ffe-205">Response</span></span>

<span data-ttu-id="24ffe-206">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="24ffe-206">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="24ffe-207">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="24ffe-207">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="24ffe-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24ffe-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24ffe-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24ffe-209">Request</span></span>
<span data-ttu-id="24ffe-p107">Este exemplo obtém e expande o evento especificado incluindo uma propriedade estendida de vários valores. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="24ffe-p107">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="24ffe-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="24ffe-212">Response</span></span>

<span data-ttu-id="24ffe-213">O corpo da resposta inclui todas as propriedades do evento especificado e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="24ffe-213">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="24ffe-p108">Observação: O objeto **event** mostrado aqui é truncado para concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24ffe-p108">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->