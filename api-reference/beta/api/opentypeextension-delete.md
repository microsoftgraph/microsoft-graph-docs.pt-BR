---
title: Excluir extensão aberta
description: 'Exclua uma extensão aberta (objeto openTypeExtension) da instância especificada de um recurso. '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 157fe63cf76273e9e968cac890a336e33f5124d0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338121"
---
# <a name="delete-open-extension"></a><span data-ttu-id="b80d4-103">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="b80d4-103">Delete open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b80d4-104">Exclua uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) da instância especificada de um recurso.</span><span class="sxs-lookup"><span data-stu-id="b80d4-104">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b80d4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b80d4-105">Permissions</span></span>

<span data-ttu-id="b80d4-106">Dependendo do recurso do qual você está excluindo a extensão e do tipo de permissão (delegado ou aplicativo) solicitado, a permissão especificada na tabela a seguir é o menos privilegiado necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b80d4-106">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="b80d4-107">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b80d4-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b80d4-108">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="b80d4-108">Supported resource</span></span> | <span data-ttu-id="b80d4-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b80d4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b80d4-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b80d4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b80d4-111">Application</span><span class="sxs-lookup"><span data-stu-id="b80d4-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="b80d4-112">device</span><span class="sxs-lookup"><span data-stu-id="b80d4-112">device</span></span>](../resources/device.md) | <span data-ttu-id="b80d4-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-113">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="b80d4-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b80d4-114">Not supported</span></span> | <span data-ttu-id="b80d4-115">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-115">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="b80d4-116">evento</span><span class="sxs-lookup"><span data-stu-id="b80d4-116">event</span></span>](../resources/event.md) | <span data-ttu-id="b80d4-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="b80d4-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-118">Calendars.ReadWrite</span></span> | <span data-ttu-id="b80d4-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-119">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="b80d4-120">grupo</span><span class="sxs-lookup"><span data-stu-id="b80d4-120">group</span></span>](../resources/group.md) | <span data-ttu-id="b80d4-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-121">Group.ReadWrite.All</span></span> | <span data-ttu-id="b80d4-122">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b80d4-122">Not supported</span></span> | <span data-ttu-id="b80d4-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-123">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="b80d4-124">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="b80d4-124">group event</span></span>](../resources/event.md) | <span data-ttu-id="b80d4-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-125">Group.ReadWrite.All</span></span> | <span data-ttu-id="b80d4-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b80d4-126">Not supported</span></span> | <span data-ttu-id="b80d4-127">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b80d4-127">Not supported</span></span> |
| [<span data-ttu-id="b80d4-128">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="b80d4-128">group post</span></span>](../resources/post.md) | <span data-ttu-id="b80d4-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-129">Group.ReadWrite.All</span></span> | <span data-ttu-id="b80d4-130">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b80d4-130">Not supported</span></span> | <span data-ttu-id="b80d4-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-131">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="b80d4-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="b80d4-132">message</span></span>](../resources/message.md) | <span data-ttu-id="b80d4-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-133">Mail.ReadWrite</span></span> | <span data-ttu-id="b80d4-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-134">Mail.ReadWrite</span></span> | <span data-ttu-id="b80d4-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-135">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="b80d4-136">organização</span><span class="sxs-lookup"><span data-stu-id="b80d4-136">organization</span></span>](../resources/organization.md) | <span data-ttu-id="b80d4-137">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-137">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="b80d4-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b80d4-138">Not supported</span></span> | <span data-ttu-id="b80d4-139">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b80d4-139">Not supported</span></span> |
| [<span data-ttu-id="b80d4-140">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="b80d4-140">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="b80d4-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="b80d4-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-142">Contacts.ReadWrite</span></span> | <span data-ttu-id="b80d4-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-143">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="b80d4-144">user</span><span class="sxs-lookup"><span data-stu-id="b80d4-144">user</span></span>](../resources/user.md) | <span data-ttu-id="b80d4-145">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-145">User.ReadWrite.All</span></span> | <span data-ttu-id="b80d4-146">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b80d4-146">User.ReadWrite</span></span> | <span data-ttu-id="b80d4-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b80d4-147">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b80d4-148">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b80d4-148">HTTP request</span></span>

<span data-ttu-id="b80d4-149">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="b80d4-149">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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
```

><span data-ttu-id="b80d4-p102">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="b80d4-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="b80d4-152">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="b80d4-152">Path parameters</span></span>
|<span data-ttu-id="b80d4-153">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="b80d4-153">**Parameter**</span></span>|<span data-ttu-id="b80d4-154">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="b80d4-154">**Type**</span></span>|<span data-ttu-id="b80d4-155">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b80d4-155">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b80d4-156">id</span><span class="sxs-lookup"><span data-stu-id="b80d4-156">id</span></span>|<span data-ttu-id="b80d4-157">string</span><span class="sxs-lookup"><span data-stu-id="b80d4-157">string</span></span>|<span data-ttu-id="b80d4-p103">Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b80d4-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="b80d4-160">extensionId</span><span class="sxs-lookup"><span data-stu-id="b80d4-160">extensionId</span></span>|<span data-ttu-id="b80d4-161">string</span><span class="sxs-lookup"><span data-stu-id="b80d4-161">string</span></span>|<span data-ttu-id="b80d4-p104">Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b80d4-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b80d4-165">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b80d4-165">Request headers</span></span>
| <span data-ttu-id="b80d4-166">Nome</span><span class="sxs-lookup"><span data-stu-id="b80d4-166">Name</span></span>       | <span data-ttu-id="b80d4-167">Valor</span><span class="sxs-lookup"><span data-stu-id="b80d4-167">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b80d4-168">Autorização</span><span class="sxs-lookup"><span data-stu-id="b80d4-168">Authorization</span></span> | <span data-ttu-id="b80d4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b80d4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b80d4-171">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b80d4-171">Request body</span></span>
<span data-ttu-id="b80d4-172">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b80d4-172">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b80d4-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="b80d4-173">Response</span></span>

<span data-ttu-id="b80d4-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b80d4-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b80d4-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b80d4-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b80d4-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b80d4-177">Request</span></span>
<span data-ttu-id="b80d4-178">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="b80d4-178">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral/
```

<span data-ttu-id="b80d4-179">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="b80d4-179">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVlN17IsAAA=/extensions/Com.Contoso.Referral
```

 

##### <a name="response"></a><span data-ttu-id="b80d4-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="b80d4-180">Response</span></span>
<span data-ttu-id="b80d4-181">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b80d4-181">Here is an example of the response.</span></span>
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
  "suppressions": []
}
-->
