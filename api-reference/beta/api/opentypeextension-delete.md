---
title: Excluir extensão aberta
description: 'Exclua uma extensão aberta (objeto openTypeExtension) da instância especificada de um recurso. '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 01be68fc952fbc57debeb054257813cb34d626a5
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092733"
---
# <a name="delete-open-extension"></a><span data-ttu-id="2209c-103">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="2209c-103">Delete open extension</span></span>

<span data-ttu-id="2209c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2209c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2209c-105">Exclua uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) da instância especificada de um recurso.</span><span class="sxs-lookup"><span data-stu-id="2209c-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

<span data-ttu-id="2209c-106">Consulte a tabela na seção [Permissões para](#permissions) ver a lista de recursos que suportam extensões abertas.</span><span class="sxs-lookup"><span data-stu-id="2209c-106">See the table in the [Permissions](#permissions) section for the list of resources that support open extensions.</span></span>

## <a name="permissions"></a><span data-ttu-id="2209c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2209c-107">Permissions</span></span>

<span data-ttu-id="2209c-108">Dependendo do recurso do qual você está excluindo a extensão e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é a menos privilegiada necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2209c-108">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2209c-109">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher permissões mais privilegiadas, procure as seguintes permissões em [Permissões.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="2209c-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2209c-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="2209c-110">Supported resource</span></span> | <span data-ttu-id="2209c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2209c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2209c-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2209c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2209c-113">Application</span><span class="sxs-lookup"><span data-stu-id="2209c-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="2209c-114">device</span><span class="sxs-lookup"><span data-stu-id="2209c-114">device</span></span>](../resources/device.md) | <span data-ttu-id="2209c-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2209c-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="2209c-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2209c-116">Not supported</span></span> | <span data-ttu-id="2209c-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="2209c-118">evento</span><span class="sxs-lookup"><span data-stu-id="2209c-118">event</span></span>](../resources/event.md) | <span data-ttu-id="2209c-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="2209c-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="2209c-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="2209c-122">grupo</span><span class="sxs-lookup"><span data-stu-id="2209c-122">group</span></span>](../resources/group.md) | <span data-ttu-id="2209c-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="2209c-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2209c-124">Not supported</span></span> | <span data-ttu-id="2209c-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2209c-126">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="2209c-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="2209c-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="2209c-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2209c-128">Not supported</span></span> | <span data-ttu-id="2209c-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2209c-129">Not supported</span></span> |
| [<span data-ttu-id="2209c-130">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="2209c-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="2209c-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="2209c-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2209c-132">Not supported</span></span> | <span data-ttu-id="2209c-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2209c-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="2209c-134">message</span></span>](../resources/message.md) | <span data-ttu-id="2209c-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-135">Mail.ReadWrite</span></span> | <span data-ttu-id="2209c-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-136">Mail.ReadWrite</span></span> | <span data-ttu-id="2209c-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="2209c-138">organization</span><span class="sxs-lookup"><span data-stu-id="2209c-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="2209c-139">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-139">Organization.ReadWrite.All</span></span> | <span data-ttu-id="2209c-140">Incompatível</span><span class="sxs-lookup"><span data-stu-id="2209c-140">Not supported</span></span> | <span data-ttu-id="2209c-141">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-141">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="2209c-142">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="2209c-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="2209c-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="2209c-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="2209c-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="2209c-146">user</span><span class="sxs-lookup"><span data-stu-id="2209c-146">user</span></span>](../resources/user.md) | <span data-ttu-id="2209c-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-147">User.ReadWrite</span></span> | <span data-ttu-id="2209c-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-148">User.ReadWrite</span></span> | <span data-ttu-id="2209c-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-149">User.ReadWrite.All</span></span> |
| [<span data-ttu-id="2209c-150">task</span><span class="sxs-lookup"><span data-stu-id="2209c-150">task</span></span>](../resources/todotask.md) | <span data-ttu-id="2209c-151">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-151">Tasks.ReadWrite</span></span> | <span data-ttu-id="2209c-152">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-152">Tasks.ReadWrite</span></span> | <span data-ttu-id="2209c-153">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-153">Tasks.ReadWrite.All</span></span> |
| [<span data-ttu-id="2209c-154">tasklist</span><span class="sxs-lookup"><span data-stu-id="2209c-154">tasklist</span></span>](../resources/todotasklist.md)  | <span data-ttu-id="2209c-155">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-155">Tasks.ReadWrite</span></span> | <span data-ttu-id="2209c-156">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2209c-156">Tasks.ReadWrite</span></span> | <span data-ttu-id="2209c-157">Tasks.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2209c-157">Tasks.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2209c-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2209c-158">HTTP request</span></span>

<span data-ttu-id="2209c-159">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="2209c-159">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="2209c-p102">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="2209c-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="2209c-162">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="2209c-162">Path parameters</span></span>
|<span data-ttu-id="2209c-163">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="2209c-163">**Parameter**</span></span>|<span data-ttu-id="2209c-164">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="2209c-164">**Type**</span></span>|<span data-ttu-id="2209c-165">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2209c-165">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2209c-166">id</span><span class="sxs-lookup"><span data-stu-id="2209c-166">id</span></span>|<span data-ttu-id="2209c-167">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2209c-167">string</span></span>|<span data-ttu-id="2209c-p103">Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2209c-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="2209c-170">extensionId</span><span class="sxs-lookup"><span data-stu-id="2209c-170">extensionId</span></span>|<span data-ttu-id="2209c-171">string</span><span class="sxs-lookup"><span data-stu-id="2209c-171">string</span></span>|<span data-ttu-id="2209c-p104">Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2209c-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2209c-175">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2209c-175">Request headers</span></span>
| <span data-ttu-id="2209c-176">Nome</span><span class="sxs-lookup"><span data-stu-id="2209c-176">Name</span></span>       | <span data-ttu-id="2209c-177">Valor</span><span class="sxs-lookup"><span data-stu-id="2209c-177">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2209c-178">Autorização</span><span class="sxs-lookup"><span data-stu-id="2209c-178">Authorization</span></span> | <span data-ttu-id="2209c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2209c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2209c-181">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2209c-181">Request body</span></span>
<span data-ttu-id="2209c-182">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2209c-182">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2209c-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="2209c-183">Response</span></span>

<span data-ttu-id="2209c-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2209c-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2209c-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2209c-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2209c-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2209c-187">Request</span></span>
<span data-ttu-id="2209c-188">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="2209c-188">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="2209c-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="2209c-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```
# <a name="c"></a>[<span data-ttu-id="2209c-190">C#</span><span class="sxs-lookup"><span data-stu-id="2209c-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2209c-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2209c-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2209c-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2209c-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2209c-193">Java</span><span class="sxs-lookup"><span data-stu-id="2209c-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2209c-194">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="2209c-194">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="2209c-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="2209c-195">Response</span></span>
<span data-ttu-id="2209c-196">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2209c-196">Here is an example of the response.</span></span>
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


