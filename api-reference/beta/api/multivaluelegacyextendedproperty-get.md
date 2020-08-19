---
title: Obter multiValueLegacyExtendedProperty
description: Expanda '.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 952b20ba5fd7825c1094559952c239681d950db2
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810871"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="5de1e-103">Obter multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="5de1e-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="5de1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5de1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5de1e-105">Obtenha uma instância do recurso que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="5de1e-105">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="5de1e-106">Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada.</span><span class="sxs-lookup"><span data-stu-id="5de1e-106">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="5de1e-107">Atualmente, esta é a única maneira de obter o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="5de1e-107">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="5de1e-108">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="5de1e-108">The following user resources are supported:</span></span>

- [<span data-ttu-id="5de1e-109">calendar</span><span class="sxs-lookup"><span data-stu-id="5de1e-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="5de1e-110">contact</span><span class="sxs-lookup"><span data-stu-id="5de1e-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="5de1e-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5de1e-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="5de1e-112">event</span><span class="sxs-lookup"><span data-stu-id="5de1e-112">event</span></span>](../resources/event.md)
- [<span data-ttu-id="5de1e-113">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5de1e-113">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="5de1e-114">message</span><span class="sxs-lookup"><span data-stu-id="5de1e-114">message</span></span>](../resources/message.md)
- [<span data-ttu-id="5de1e-115">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="5de1e-115">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="5de1e-116">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="5de1e-116">Outlook task folder</span></span>](../resources/outlooktaskfolder.md)

<span data-ttu-id="5de1e-117">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="5de1e-117">As well as the following group resources:</span></span>

- <span data-ttu-id="5de1e-118">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="5de1e-118">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="5de1e-119">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="5de1e-119">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="5de1e-120">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="5de1e-120">group [post](../resources/post.md)</span></span>

<span data-ttu-id="5de1e-121">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="5de1e-121">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5de1e-122">Permissões</span><span class="sxs-lookup"><span data-stu-id="5de1e-122">Permissions</span></span>
<span data-ttu-id="5de1e-123">Dependendo do recurso para o qual você está obtendo a propriedade estendida e o tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o mínimo necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5de1e-123">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="5de1e-124">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5de1e-124">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5de1e-125">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="5de1e-125">Supported resource</span></span> | <span data-ttu-id="5de1e-126">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5de1e-126">Delegated (work or school account)</span></span> | <span data-ttu-id="5de1e-127">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5de1e-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5de1e-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5de1e-128">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="5de1e-129">calendar</span><span class="sxs-lookup"><span data-stu-id="5de1e-129">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="5de1e-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-130">Calendars.Read</span></span> | <span data-ttu-id="5de1e-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-131">Calendars.Read</span></span> | <span data-ttu-id="5de1e-132">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-132">Calendars.Read</span></span> |
| [<span data-ttu-id="5de1e-133">contato</span><span class="sxs-lookup"><span data-stu-id="5de1e-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="5de1e-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-134">Contacts.Read</span></span> | <span data-ttu-id="5de1e-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-135">Contacts.Read</span></span> | <span data-ttu-id="5de1e-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-136">Contacts.Read</span></span> |
| [<span data-ttu-id="5de1e-137">contactFolder</span><span class="sxs-lookup"><span data-stu-id="5de1e-137">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="5de1e-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-138">Contacts.Read</span></span> | <span data-ttu-id="5de1e-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-139">Contacts.Read</span></span> | <span data-ttu-id="5de1e-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-140">Contacts.Read</span></span> |
| [<span data-ttu-id="5de1e-141">evento</span><span class="sxs-lookup"><span data-stu-id="5de1e-141">event</span></span>](../resources/event.md) | <span data-ttu-id="5de1e-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-142">Calendars.Read</span></span> | <span data-ttu-id="5de1e-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-143">Calendars.Read</span></span> |  <span data-ttu-id="5de1e-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-144">Calendars.Read</span></span>|
| <span data-ttu-id="5de1e-145">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="5de1e-145">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="5de1e-146">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5de1e-146">Group.Read.All</span></span> | <span data-ttu-id="5de1e-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5de1e-147">Not supported</span></span> | <span data-ttu-id="5de1e-148">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5de1e-148">Not supported</span></span> |
| <span data-ttu-id="5de1e-149">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="5de1e-149">group [event](../resources/event.md)</span></span> | <span data-ttu-id="5de1e-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5de1e-150">Group.Read.All</span></span> | <span data-ttu-id="5de1e-151">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5de1e-151">Not supported</span></span> | <span data-ttu-id="5de1e-152">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5de1e-152">Not supported</span></span> |
| <span data-ttu-id="5de1e-153">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="5de1e-153">group [post](../resources/post.md)</span></span> | <span data-ttu-id="5de1e-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5de1e-154">Group.Read.All</span></span> | <span data-ttu-id="5de1e-155">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5de1e-155">Not supported</span></span> | <span data-ttu-id="5de1e-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5de1e-156">Group.Read.All</span></span> |
| [<span data-ttu-id="5de1e-157">mailFolder</span><span class="sxs-lookup"><span data-stu-id="5de1e-157">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="5de1e-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-158">Mail.Read</span></span> | <span data-ttu-id="5de1e-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-159">Mail.Read</span></span> | <span data-ttu-id="5de1e-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-160">Mail.Read</span></span> |
| [<span data-ttu-id="5de1e-161">message</span><span class="sxs-lookup"><span data-stu-id="5de1e-161">message</span></span>](../resources/message.md) | <span data-ttu-id="5de1e-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-162">Mail.Read</span></span> | <span data-ttu-id="5de1e-163">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-163">Mail.Read</span></span> | <span data-ttu-id="5de1e-164">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-164">Mail.Read</span></span> |
| [<span data-ttu-id="5de1e-165">Tarefa do Outlook</span><span class="sxs-lookup"><span data-stu-id="5de1e-165">Outlook task</span></span>](../resources/outlooktask.md) | <span data-ttu-id="5de1e-166">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-166">Tasks.Read</span></span> | <span data-ttu-id="5de1e-167">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-167">Tasks.Read</span></span> | <span data-ttu-id="5de1e-168">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5de1e-168">Not supported</span></span> |
| [<span data-ttu-id="5de1e-169">Pasta de tarefas do Outlook</span><span class="sxs-lookup"><span data-stu-id="5de1e-169">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) | <span data-ttu-id="5de1e-170">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-170">Tasks.Read</span></span> | <span data-ttu-id="5de1e-171">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5de1e-171">Tasks.Read</span></span> | <span data-ttu-id="5de1e-172">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="5de1e-172">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="5de1e-173">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5de1e-173">HTTP request</span></span>

<span data-ttu-id="5de1e-p103">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="5de1e-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="5de1e-176">Obtenha uma instância de **message**:</span><span class="sxs-lookup"><span data-stu-id="5de1e-176">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5de1e-177">Obtenha uma instância de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="5de1e-177">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5de1e-178">Obtenha uma instância de **event**:</span><span class="sxs-lookup"><span data-stu-id="5de1e-178">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5de1e-179">Obtenha uma instância de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="5de1e-179">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5de1e-180">Obtenha uma instância de **contact**:</span><span class="sxs-lookup"><span data-stu-id="5de1e-180">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5de1e-181">Obtenha uma instância de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="5de1e-181">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5de1e-182">Obtenha uma instância de **outlookTask** :</span><span class="sxs-lookup"><span data-stu-id="5de1e-182">Get an **outlookTask** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="5de1e-183">Obtenha uma instância de **outlookTaskFolder** :</span><span class="sxs-lookup"><span data-stu-id="5de1e-183">Get an **outlookTaskFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5de1e-184">Obtenha uma instância de **group event**:</span><span class="sxs-lookup"><span data-stu-id="5de1e-184">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="5de1e-185">Acesse uma instância de **postar** em grupo:</span><span class="sxs-lookup"><span data-stu-id="5de1e-185">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="5de1e-186">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="5de1e-186">Path parameters</span></span>
|<span data-ttu-id="5de1e-187">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="5de1e-187">**Parameter**</span></span>|<span data-ttu-id="5de1e-188">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="5de1e-188">**Type**</span></span>|<span data-ttu-id="5de1e-189">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5de1e-189">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5de1e-190">id_value</span><span class="sxs-lookup"><span data-stu-id="5de1e-190">id_value</span></span>|<span data-ttu-id="5de1e-191">String</span><span class="sxs-lookup"><span data-stu-id="5de1e-191">String</span></span>|<span data-ttu-id="5de1e-p104">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5de1e-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5de1e-196">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5de1e-196">Request headers</span></span>
| <span data-ttu-id="5de1e-197">Nome</span><span class="sxs-lookup"><span data-stu-id="5de1e-197">Name</span></span>      |<span data-ttu-id="5de1e-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="5de1e-198">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5de1e-199">Autorização</span><span class="sxs-lookup"><span data-stu-id="5de1e-199">Authorization</span></span>  | <span data-ttu-id="5de1e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5de1e-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5de1e-202">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5de1e-202">Request body</span></span>
<span data-ttu-id="5de1e-203">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5de1e-203">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5de1e-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="5de1e-204">Response</span></span>

<span data-ttu-id="5de1e-205">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="5de1e-205">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="5de1e-206">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="5de1e-206">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="5de1e-207">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5de1e-207">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5de1e-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5de1e-208">Request</span></span>
<span data-ttu-id="5de1e-p106">Este exemplo obtém e expande o evento especificado incluindo uma propriedade estendida de vários valores. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="5de1e-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="5de1e-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="5de1e-211">Response</span></span>

<span data-ttu-id="5de1e-212">O corpo da resposta inclui todas as propriedades do evento especificado e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="5de1e-212">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="5de1e-p107">Observação: O objeto **event** mostrado aqui é truncado para concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5de1e-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
