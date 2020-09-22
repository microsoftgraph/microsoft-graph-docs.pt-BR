---
title: Excluir extensão aberta
description: Exclua uma extensão aberta (objeto openTypeExtension) da instância especificada de um recurso.
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: ebaa3a22728fb2e64137b755b0874c5420923f0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988678"
---
# <a name="delete-open-extension"></a><span data-ttu-id="2e4b7-103">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="2e4b7-103">Delete open extension</span></span>

<span data-ttu-id="2e4b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e4b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2e4b7-105">Exclua uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) da instância especificada de um recurso.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-105">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2e4b7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e4b7-106">Permissions</span></span>

<span data-ttu-id="2e4b7-107">Dependendo do recurso do qual você está excluindo a extensão e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-107">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2e4b7-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e4b7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e4b7-109">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="2e4b7-109">Supported resource</span></span> | <span data-ttu-id="2e4b7-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e4b7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e4b7-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e4b7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e4b7-112">Application</span><span class="sxs-lookup"><span data-stu-id="2e4b7-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="2e4b7-113">device</span><span class="sxs-lookup"><span data-stu-id="2e4b7-113">device</span></span>](../resources/device.md) | <span data-ttu-id="2e4b7-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-114">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="2e4b7-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2e4b7-115">Not supported</span></span> | <span data-ttu-id="2e4b7-116">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-116">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="2e4b7-117">evento</span><span class="sxs-lookup"><span data-stu-id="2e4b7-117">event</span></span>](../resources/event.md) | <span data-ttu-id="2e4b7-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="2e4b7-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="2e4b7-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-120">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="2e4b7-121">grupo</span><span class="sxs-lookup"><span data-stu-id="2e4b7-121">group</span></span>](../resources/group.md) | <span data-ttu-id="2e4b7-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-122">Group.ReadWrite.All</span></span> | <span data-ttu-id="2e4b7-123">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2e4b7-123">Not supported</span></span> | <span data-ttu-id="2e4b7-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-124">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2e4b7-125">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="2e4b7-125">group event</span></span>](../resources/event.md) | <span data-ttu-id="2e4b7-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-126">Group.ReadWrite.All</span></span> | <span data-ttu-id="2e4b7-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2e4b7-127">Not supported</span></span> | <span data-ttu-id="2e4b7-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2e4b7-128">Not supported</span></span> |
| [<span data-ttu-id="2e4b7-129">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="2e4b7-129">group post</span></span>](../resources/post.md) | <span data-ttu-id="2e4b7-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-130">Group.ReadWrite.All</span></span> | <span data-ttu-id="2e4b7-131">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2e4b7-131">Not supported</span></span> | <span data-ttu-id="2e4b7-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-132">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="2e4b7-133">mensagem</span><span class="sxs-lookup"><span data-stu-id="2e4b7-133">message</span></span>](../resources/message.md) | <span data-ttu-id="2e4b7-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-134">Mail.ReadWrite</span></span> | <span data-ttu-id="2e4b7-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-135">Mail.ReadWrite</span></span> | <span data-ttu-id="2e4b7-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-136">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="2e4b7-137">organization</span><span class="sxs-lookup"><span data-stu-id="2e4b7-137">organization</span></span>](../resources/organization.md) | <span data-ttu-id="2e4b7-138">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-138">Organization.ReadWrite.All</span></span> | <span data-ttu-id="2e4b7-139">Incompatível</span><span class="sxs-lookup"><span data-stu-id="2e4b7-139">Not supported</span></span> | <span data-ttu-id="2e4b7-140">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-140">Organization.ReadWrite.All</span></span> |
| [<span data-ttu-id="2e4b7-141">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="2e4b7-141">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="2e4b7-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="2e4b7-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="2e4b7-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-144">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="2e4b7-145">user</span><span class="sxs-lookup"><span data-stu-id="2e4b7-145">user</span></span>](../resources/user.md) | <span data-ttu-id="2e4b7-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-146">User.ReadWrite</span></span> | <span data-ttu-id="2e4b7-147">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e4b7-147">User.ReadWrite</span></span> | <span data-ttu-id="2e4b7-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4b7-148">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e4b7-149">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4b7-149">HTTP request</span></span>
<span data-ttu-id="2e4b7-150">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-150">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="2e4b7-p102">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="2e4b7-153">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="2e4b7-153">Path parameters</span></span>
|<span data-ttu-id="2e4b7-154">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2e4b7-154">Parameter</span></span>|<span data-ttu-id="2e4b7-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e4b7-155">Type</span></span>|<span data-ttu-id="2e4b7-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e4b7-156">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2e4b7-157">id</span><span class="sxs-lookup"><span data-stu-id="2e4b7-157">id</span></span>|<span data-ttu-id="2e4b7-158">string</span><span class="sxs-lookup"><span data-stu-id="2e4b7-158">string</span></span>|<span data-ttu-id="2e4b7-p103">Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="2e4b7-161">extensionId</span><span class="sxs-lookup"><span data-stu-id="2e4b7-161">extensionId</span></span>|<span data-ttu-id="2e4b7-162">string</span><span class="sxs-lookup"><span data-stu-id="2e4b7-162">string</span></span>|<span data-ttu-id="2e4b7-p104">Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2e4b7-166">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4b7-166">Request headers</span></span>
| <span data-ttu-id="2e4b7-167">Nome</span><span class="sxs-lookup"><span data-stu-id="2e4b7-167">Name</span></span>       | <span data-ttu-id="2e4b7-168">Valor</span><span class="sxs-lookup"><span data-stu-id="2e4b7-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="2e4b7-169">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e4b7-169">Authorization</span></span> | <span data-ttu-id="2e4b7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e4b7-172">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4b7-172">Request body</span></span>
<span data-ttu-id="2e4b7-173">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-173">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e4b7-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4b7-174">Response</span></span>

<span data-ttu-id="2e4b7-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e4b7-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e4b7-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e4b7-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4b7-178">Request</span></span>
<span data-ttu-id="2e4b7-179">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-179">The first example references an extension by its name and deletes the extension in the specified message.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e4b7-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4b7-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```
# <a name="c"></a>[<span data-ttu-id="2e4b7-181">C#</span><span class="sxs-lookup"><span data-stu-id="2e4b7-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-opentypeextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e4b7-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e4b7-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-opentypeextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e4b7-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e4b7-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-opentypeextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2e4b7-184">Java</span><span class="sxs-lookup"><span data-stu-id="2e4b7-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-opentypeextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2e4b7-185">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-185">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="2e4b7-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4b7-186">Response</span></span>
<span data-ttu-id="2e4b7-187">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4b7-187">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

