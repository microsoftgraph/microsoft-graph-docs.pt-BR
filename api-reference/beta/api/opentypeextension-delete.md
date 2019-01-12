---
title: Excluir extensão aberta
description: 'Exclua uma extensão aberta (objeto openTypeExtension) da instância especificada de um recurso. '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 617971d4e31e65a662415c75f4a6cdac330ebcb0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983174"
---
# <a name="delete-open-extension"></a><span data-ttu-id="d0df6-103">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="d0df6-103">Delete open extension</span></span>

> <span data-ttu-id="d0df6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0df6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0df6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0df6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0df6-106">Exclua uma extensão aberta (objeto [openTypeExtension](../resources/opentypeextension.md)) da instância especificada de um recurso.</span><span class="sxs-lookup"><span data-stu-id="d0df6-106">Delete an open extension ([openTypeExtension](../resources/opentypeextension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d0df6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d0df6-107">Permissions</span></span>

<span data-ttu-id="d0df6-108">Dependendo de permissão e o recurso que você está excluindo a extensão do tipo (delegado ou aplicativo) solicitada, a permissão especificada na tabela a seguir é menos privilegiada necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d0df6-108">Depending on the resource you're deleting the extension from and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="d0df6-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0df6-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0df6-110">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="d0df6-110">Supported resource</span></span> | <span data-ttu-id="d0df6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0df6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d0df6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0df6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0df6-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0df6-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="d0df6-114">device</span><span class="sxs-lookup"><span data-stu-id="d0df6-114">device</span></span>](../resources/device.md) | <span data-ttu-id="d0df6-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-115">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="d0df6-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0df6-116">Not supported</span></span> | <span data-ttu-id="d0df6-117">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-117">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="d0df6-118">evento</span><span class="sxs-lookup"><span data-stu-id="d0df6-118">event</span></span>](../resources/event.md) | <span data-ttu-id="d0df6-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-119">Calendars.ReadWrite</span></span> | <span data-ttu-id="d0df6-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="d0df6-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-121">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="d0df6-122">grupo</span><span class="sxs-lookup"><span data-stu-id="d0df6-122">group</span></span>](../resources/group.md) | <span data-ttu-id="d0df6-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-123">Group.ReadWrite.All</span></span> | <span data-ttu-id="d0df6-124">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0df6-124">Not supported</span></span> | <span data-ttu-id="d0df6-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-125">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="d0df6-126">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="d0df6-126">group event</span></span>](../resources/event.md) | <span data-ttu-id="d0df6-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-127">Group.ReadWrite.All</span></span> | <span data-ttu-id="d0df6-128">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0df6-128">Not supported</span></span> | <span data-ttu-id="d0df6-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0df6-129">Not supported</span></span> |
| [<span data-ttu-id="d0df6-130">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="d0df6-130">group post</span></span>](../resources/post.md) | <span data-ttu-id="d0df6-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-131">Group.ReadWrite.All</span></span> | <span data-ttu-id="d0df6-132">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0df6-132">Not supported</span></span> | <span data-ttu-id="d0df6-133">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-133">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="d0df6-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="d0df6-134">message</span></span>](../resources/message.md) | <span data-ttu-id="d0df6-135">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-135">Mail.ReadWrite</span></span> | <span data-ttu-id="d0df6-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-136">Mail.ReadWrite</span></span> | <span data-ttu-id="d0df6-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-137">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="d0df6-138">organização</span><span class="sxs-lookup"><span data-stu-id="d0df6-138">organization</span></span>](../resources/organization.md) | <span data-ttu-id="d0df6-139">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-139">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="d0df6-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0df6-140">Not supported</span></span> | <span data-ttu-id="d0df6-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d0df6-141">Not supported</span></span> |
| [<span data-ttu-id="d0df6-142">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="d0df6-142">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="d0df6-143">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-143">Contacts.ReadWrite</span></span> | <span data-ttu-id="d0df6-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="d0df6-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-145">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="d0df6-146">usuário</span><span class="sxs-lookup"><span data-stu-id="d0df6-146">user</span></span>](../resources/user.md) | <span data-ttu-id="d0df6-147">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-147">User.ReadWrite.All</span></span> | <span data-ttu-id="d0df6-148">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0df6-148">User.ReadWrite</span></span> | <span data-ttu-id="d0df6-149">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0df6-149">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0df6-150">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0df6-150">HTTP request</span></span>

<span data-ttu-id="d0df6-151">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="d0df6-151">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

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

><span data-ttu-id="d0df6-p103">**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="d0df6-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="d0df6-154">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d0df6-154">Path parameters</span></span>
|<span data-ttu-id="d0df6-155">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="d0df6-155">**Parameter**</span></span>|<span data-ttu-id="d0df6-156">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="d0df6-156">**Type**</span></span>|<span data-ttu-id="d0df6-157">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0df6-157">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d0df6-158">id</span><span class="sxs-lookup"><span data-stu-id="d0df6-158">id</span></span>|<span data-ttu-id="d0df6-159">string</span><span class="sxs-lookup"><span data-stu-id="d0df6-159">string</span></span>|<span data-ttu-id="d0df6-p104">Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0df6-p104">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="d0df6-162">extensionId</span><span class="sxs-lookup"><span data-stu-id="d0df6-162">extensionId</span></span>|<span data-ttu-id="d0df6-163">string</span><span class="sxs-lookup"><span data-stu-id="d0df6-163">string</span></span>|<span data-ttu-id="d0df6-p105">Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0df6-p105">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d0df6-167">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0df6-167">Request headers</span></span>
| <span data-ttu-id="d0df6-168">Nome</span><span class="sxs-lookup"><span data-stu-id="d0df6-168">Name</span></span>       | <span data-ttu-id="d0df6-169">Valor</span><span class="sxs-lookup"><span data-stu-id="d0df6-169">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d0df6-170">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0df6-170">Authorization</span></span> | <span data-ttu-id="d0df6-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0df6-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0df6-173">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0df6-173">Request body</span></span>
<span data-ttu-id="d0df6-174">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d0df6-174">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0df6-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0df6-175">Response</span></span>

<span data-ttu-id="d0df6-p107">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0df6-p107">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0df6-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0df6-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0df6-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0df6-179">Request</span></span>
<span data-ttu-id="d0df6-180">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="d0df6-180">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="d0df6-181">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="d0df6-181">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/beta/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="d0df6-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0df6-182">Response</span></span>
<span data-ttu-id="d0df6-183">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0df6-183">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
