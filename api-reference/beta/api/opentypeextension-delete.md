---
title: Excluir extensão aberta
description: 'Exclua uma extensão aberta (objeto openTypeExtension) da instância especificada de um recurso. '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 280ca648abf20622b92d9724c0cbe504e6b207d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071938"
---
# <a name="delete-open-extension"></a><span data-ttu-id="e1e6a-103">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="e1e6a-103">Delete open extension</span></span>

<span data-ttu-id="e1e6a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1e6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1e6a-105">Exclua uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) da instância especificada de um recurso.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e1e6a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1e6a-106">Permissions</span></span>

<span data-ttu-id="e1e6a-107">Dependendo do recurso do qual você está excluindo a extensão e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-107">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="e1e6a-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1e6a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1e6a-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="e1e6a-109">Supported resource</span></span> | <span data-ttu-id="e1e6a-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1e6a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e1e6a-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1e6a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1e6a-112">Application</span><span class="sxs-lookup"><span data-stu-id="e1e6a-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="e1e6a-113">device</span><span class="sxs-lookup"><span data-stu-id="e1e6a-113">device</span></span>](../resources/device.md) | <span data-ttu-id="e1e6a-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="e1e6a-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1e6a-115">Not supported</span></span> | <span data-ttu-id="e1e6a-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="e1e6a-117">evento</span><span class="sxs-lookup"><span data-stu-id="e1e6a-117">event</span></span>](../resources/event.md) | <span data-ttu-id="e1e6a-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="e1e6a-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="e1e6a-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="e1e6a-121">grupo</span><span class="sxs-lookup"><span data-stu-id="e1e6a-121">group</span></span>](../resources/group.md) | <span data-ttu-id="e1e6a-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="e1e6a-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1e6a-123">Not supported</span></span> | <span data-ttu-id="e1e6a-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-124">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="e1e6a-125">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="e1e6a-125">group event</span></span>](../resources/event.md) | <span data-ttu-id="e1e6a-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="e1e6a-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1e6a-127">Not supported</span></span> | <span data-ttu-id="e1e6a-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1e6a-128">Not supported</span></span> |
| [<span data-ttu-id="e1e6a-129">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="e1e6a-129">group post</span></span>](../resources/post.md) | <span data-ttu-id="e1e6a-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="e1e6a-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1e6a-131">Not supported</span></span> | <span data-ttu-id="e1e6a-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="e1e6a-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="e1e6a-133">message</span></span>](../resources/message.md) | <span data-ttu-id="e1e6a-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-134">Mail.ReadWrite</span></span> | <span data-ttu-id="e1e6a-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-135">Mail.ReadWrite</span></span> | <span data-ttu-id="e1e6a-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="e1e6a-137">organization</span><span class="sxs-lookup"><span data-stu-id="e1e6a-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="e1e6a-138">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-138">Organization.ReadWrite.All</span></span> | <span data-ttu-id="e1e6a-139">Incompatível</span><span class="sxs-lookup"><span data-stu-id="e1e6a-139">Not supported</span></span> | <span data-ttu-id="e1e6a-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-140">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="e1e6a-141">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="e1e6a-141">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="e1e6a-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="e1e6a-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="e1e6a-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="e1e6a-145">user</span><span class="sxs-lookup"><span data-stu-id="e1e6a-145">user</span></span>](../resources/user.md) | <span data-ttu-id="e1e6a-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-146">User.ReadWrite</span></span> | <span data-ttu-id="e1e6a-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-147">User.ReadWrite</span></span> | <span data-ttu-id="e1e6a-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-148">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="e1e6a-149">task</span><span class="sxs-lookup"><span data-stu-id="e1e6a-149">task</span></span>](../resources/todotask.md) | <span data-ttu-id="e1e6a-150">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-150">Tasks.ReadWrite</span></span> | <span data-ttu-id="e1e6a-151">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-151">Tasks.ReadWrite</span></span> | <span data-ttu-id="e1e6a-152">Tasks. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-152">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="e1e6a-153">TaskList</span><span class="sxs-lookup"><span data-stu-id="e1e6a-153">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="e1e6a-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-154">Tasks.ReadWrite</span></span> | <span data-ttu-id="e1e6a-155">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1e6a-155">Tasks.ReadWrite</span></span> | <span data-ttu-id="e1e6a-156">Tasks. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e1e6a-156">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1e6a-157">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1e6a-157">HTTP request</span></span>

<span data-ttu-id="e1e6a-158">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-158">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{Id}/extensions/{extensionId}
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
DELETE /users/me/todo/lists/{todoTaskListId}/extensions/{extensionId}
DELETE /users/me/todo/lists/{todoTaskListId}/tasks/{taskId}/extensions/{extensionId}
```

><span data-ttu-id="e1e6a-p102">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="e1e6a-161">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="e1e6a-161">Path parameters</span></span>
|<span data-ttu-id="e1e6a-162">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="e1e6a-162">**Parameter**</span></span>|<span data-ttu-id="e1e6a-163">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="e1e6a-163">**Type**</span></span>|<span data-ttu-id="e1e6a-164">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1e6a-164">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e1e6a-165">id</span><span class="sxs-lookup"><span data-stu-id="e1e6a-165">id</span></span>|<span data-ttu-id="e1e6a-166">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1e6a-166">string</span></span>|<span data-ttu-id="e1e6a-p103">Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="e1e6a-169">extensionId</span><span class="sxs-lookup"><span data-stu-id="e1e6a-169">extensionId</span></span>|<span data-ttu-id="e1e6a-170">string</span><span class="sxs-lookup"><span data-stu-id="e1e6a-170">string</span></span>|<span data-ttu-id="e1e6a-p104">Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="e1e6a-174">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1e6a-174">Request headers</span></span>
| <span data-ttu-id="e1e6a-175">Nome</span><span class="sxs-lookup"><span data-stu-id="e1e6a-175">Name</span></span>       | <span data-ttu-id="e1e6a-176">Valor</span><span class="sxs-lookup"><span data-stu-id="e1e6a-176">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e1e6a-177">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1e6a-177">Authorization</span></span> | <span data-ttu-id="e1e6a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1e6a-180">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1e6a-180">Request body</span></span>
<span data-ttu-id="e1e6a-181">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-181">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1e6a-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1e6a-182">Response</span></span>

<span data-ttu-id="e1e6a-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1e6a-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1e6a-185">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1e6a-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1e6a-186">Request</span></span>
<span data-ttu-id="e1e6a-187">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-187">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1e6a-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1e6a-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="c"></a>[<span data-ttu-id="e1e6a-189">C#</span><span class="sxs-lookup"><span data-stu-id="e1e6a-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1e6a-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1e6a-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1e6a-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1e6a-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e1e6a-192">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-192">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="e1e6a-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1e6a-193">Response</span></span>
<span data-ttu-id="e1e6a-194">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1e6a-194">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


