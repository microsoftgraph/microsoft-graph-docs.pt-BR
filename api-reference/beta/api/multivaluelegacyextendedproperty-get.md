---
title: Obter multiValueLegacyExtendedProperty
description: Expanda '.
localization_priority: Normal
ms.openlocfilehash: 7a649020bf326d4ec1ed3a83ae0c759a012378d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540258"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="1946a-103">Obter multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1946a-103">Get multiValueLegacyExtendedProperty</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1946a-104">Obtenha uma instância do recurso que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="1946a-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="1946a-105">Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada.</span><span class="sxs-lookup"><span data-stu-id="1946a-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="1946a-106">Atualmente, esta é a única maneira de obter o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="1946a-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="1946a-107">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="1946a-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="1946a-108">calendar</span><span class="sxs-lookup"><span data-stu-id="1946a-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="1946a-109">contact</span><span class="sxs-lookup"><span data-stu-id="1946a-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="1946a-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="1946a-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="1946a-111">evento</span><span class="sxs-lookup"><span data-stu-id="1946a-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="1946a-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="1946a-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="1946a-113">mensagem</span><span class="sxs-lookup"><span data-stu-id="1946a-113">message</span></span>](../resources/message.md) 
- [<span data-ttu-id="1946a-114">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="1946a-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="1946a-115">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="1946a-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="1946a-116">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="1946a-116">As well as the following group resources:</span></span>

- <span data-ttu-id="1946a-117">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="1946a-117">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="1946a-118">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="1946a-118">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="1946a-119">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="1946a-119">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="1946a-120">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="1946a-120">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1946a-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="1946a-121">Permissions</span></span>
<span data-ttu-id="1946a-122">Dependendo do recurso para o qual você está obtendo a propriedade estendida e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1946a-122">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="1946a-123">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1946a-123">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1946a-124">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="1946a-124">Supported resource</span></span> | <span data-ttu-id="1946a-125">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1946a-125">Delegated (work or school account)</span></span> | <span data-ttu-id="1946a-126">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1946a-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1946a-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1946a-127">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="1946a-128">calendar</span><span class="sxs-lookup"><span data-stu-id="1946a-128">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="1946a-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-129">Calendars.Read</span></span> | <span data-ttu-id="1946a-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-130">Calendars.Read</span></span> | <span data-ttu-id="1946a-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-131">Calendars.Read</span></span> |
| [<span data-ttu-id="1946a-132">contato</span><span class="sxs-lookup"><span data-stu-id="1946a-132">contact</span></span>](../resources/contact.md) | <span data-ttu-id="1946a-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-133">Contacts.Read</span></span> | <span data-ttu-id="1946a-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-134">Contacts.Read</span></span> | <span data-ttu-id="1946a-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-135">Contacts.Read</span></span> |
| [<span data-ttu-id="1946a-136">contactFolder</span><span class="sxs-lookup"><span data-stu-id="1946a-136">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="1946a-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-137">Contacts.Read</span></span> | <span data-ttu-id="1946a-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-138">Contacts.Read</span></span> | <span data-ttu-id="1946a-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-139">Contacts.Read</span></span> |
| [<span data-ttu-id="1946a-140">evento</span><span class="sxs-lookup"><span data-stu-id="1946a-140">event</span></span>](../resources/event.md) | <span data-ttu-id="1946a-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-141">Calendars.Read</span></span> | <span data-ttu-id="1946a-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-142">Calendars.Read</span></span> |  <span data-ttu-id="1946a-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-143">Calendars.Read</span></span>|
| <span data-ttu-id="1946a-144">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="1946a-144">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="1946a-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1946a-145">Group.Read.All</span></span> | <span data-ttu-id="1946a-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1946a-146">Not supported</span></span> | <span data-ttu-id="1946a-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1946a-147">Not supported</span></span> |
| <span data-ttu-id="1946a-148">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="1946a-148">group [event](../resources/event.md)</span></span> | <span data-ttu-id="1946a-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1946a-149">Group.Read.All</span></span> | <span data-ttu-id="1946a-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1946a-150">Not supported</span></span> | <span data-ttu-id="1946a-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1946a-151">Not supported</span></span> |
| <span data-ttu-id="1946a-152">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="1946a-152">group [post](../resources/post.md)</span></span> | <span data-ttu-id="1946a-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1946a-153">Group.Read.All</span></span> | <span data-ttu-id="1946a-154">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1946a-154">Not supported</span></span> | <span data-ttu-id="1946a-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1946a-155">Group.Read.All</span></span> |
| [<span data-ttu-id="1946a-156">mailFolder</span><span class="sxs-lookup"><span data-stu-id="1946a-156">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="1946a-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-157">Mail.Read</span></span> | <span data-ttu-id="1946a-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-158">Mail.Read</span></span> | <span data-ttu-id="1946a-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-159">Mail.Read</span></span> |
| [<span data-ttu-id="1946a-160">mensagem</span><span class="sxs-lookup"><span data-stu-id="1946a-160">message</span></span>](../resources/message.md) | <span data-ttu-id="1946a-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-161">Mail.Read</span></span> | <span data-ttu-id="1946a-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-162">Mail.Read</span></span> | <span data-ttu-id="1946a-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-163">Mail.Read</span></span> |
| [<span data-ttu-id="1946a-164">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="1946a-164">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="1946a-165">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-165">Tasks.Read</span></span> | <span data-ttu-id="1946a-166">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-166">Tasks.Read</span></span> | <span data-ttu-id="1946a-167">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1946a-167">Not supported</span></span> |
| [<span data-ttu-id="1946a-168">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="1946a-168">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="1946a-169">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-169">Tasks.Read</span></span> | <span data-ttu-id="1946a-170">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1946a-170">Tasks.Read</span></span> | <span data-ttu-id="1946a-171">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="1946a-171">Not supported</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="1946a-172">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1946a-172">HTTP request</span></span>

<span data-ttu-id="1946a-p103">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="1946a-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="1946a-175">Obtenha uma instância de **message**:</span><span class="sxs-lookup"><span data-stu-id="1946a-175">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1946a-176">Obtenha uma instância de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="1946a-176">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1946a-177">Obtenha uma instância de **event**:</span><span class="sxs-lookup"><span data-stu-id="1946a-177">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1946a-178">Obtenha uma instância de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="1946a-178">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1946a-179">Obtenha uma instância de **contact**:</span><span class="sxs-lookup"><span data-stu-id="1946a-179">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1946a-180">Obtenha uma instância de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="1946a-180">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1946a-181">Obtenha uma instância de **outlookTask** :</span><span class="sxs-lookup"><span data-stu-id="1946a-181">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1946a-182">Obtenha uma instância de **outlookTaskFolder** :</span><span class="sxs-lookup"><span data-stu-id="1946a-182">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1946a-183">Obtenha uma instância de **group event**:</span><span class="sxs-lookup"><span data-stu-id="1946a-183">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1946a-184">Acesse uma instância de **postar** em grupo:</span><span class="sxs-lookup"><span data-stu-id="1946a-184">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="1946a-185">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="1946a-185">Path parameters</span></span>
|<span data-ttu-id="1946a-186">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="1946a-186">**Parameter**</span></span>|<span data-ttu-id="1946a-187">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="1946a-187">**Type**</span></span>|<span data-ttu-id="1946a-188">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1946a-188">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1946a-189">id_value</span><span class="sxs-lookup"><span data-stu-id="1946a-189">id_value</span></span>|<span data-ttu-id="1946a-190">String</span><span class="sxs-lookup"><span data-stu-id="1946a-190">String</span></span>|<span data-ttu-id="1946a-p104">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1946a-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1946a-195">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1946a-195">Request headers</span></span>
| <span data-ttu-id="1946a-196">Nome</span><span class="sxs-lookup"><span data-stu-id="1946a-196">Name</span></span>      |<span data-ttu-id="1946a-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="1946a-197">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1946a-198">Autorização</span><span class="sxs-lookup"><span data-stu-id="1946a-198">Authorization</span></span>  | <span data-ttu-id="1946a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1946a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1946a-201">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1946a-201">Request body</span></span>
<span data-ttu-id="1946a-202">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1946a-202">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1946a-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="1946a-203">Response</span></span>

<span data-ttu-id="1946a-204">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1946a-204">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="1946a-205">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="1946a-205">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="1946a-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1946a-206">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1946a-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1946a-207">Request</span></span>
<span data-ttu-id="1946a-p106">Este exemplo obtém e expande o evento especificado incluindo uma propriedade estendida de vários valores. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="1946a-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="1946a-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="1946a-210">Response</span></span>

<span data-ttu-id="1946a-211">O corpo da resposta inclui todas as propriedades do evento especificado e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="1946a-211">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="1946a-p107">Observação: O objeto **event** mostrado aqui é truncado para concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1946a-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/multivaluelegacyextendedproperty-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
