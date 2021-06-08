---
title: 'Canal de Atualização '
description: Atualize as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8527ae77c6198aea615aff8add5a569dc563bafa
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786212"
---
# <a name="update-channel"></a><span data-ttu-id="4b848-103">Canal de Atualização </span><span class="sxs-lookup"><span data-stu-id="4b848-103">Update channel</span></span>

<span data-ttu-id="4b848-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b848-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b848-105">Atualize as propriedades do canal [especificado](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="4b848-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b848-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4b848-106">Permissions</span></span>

<span data-ttu-id="4b848-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b848-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b848-109">Permission type</span></span>      | <span data-ttu-id="4b848-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b848-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b848-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b848-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b848-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b848-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="4b848-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b848-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b848-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b848-114">Not supported.</span></span>    |
|<span data-ttu-id="4b848-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b848-115">Application</span></span> | <span data-ttu-id="4b848-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b848-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="4b848-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="4b848-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="4b848-p102">**Observação**: esta API dá suporte a permissões de administrador. Os administradores globais e os administradores de serviços do Microsoft Teams podem acessar equipes das quais não são membros.</span><span class="sxs-lookup"><span data-stu-id="4b848-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4b848-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b848-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}/channels/{channel-id}
```
## <a name="request-headers"></a><span data-ttu-id="4b848-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b848-121">Request headers</span></span>
| <span data-ttu-id="4b848-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b848-122">Header</span></span>       | <span data-ttu-id="4b848-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4b848-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4b848-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b848-124">Authorization</span></span>  | <span data-ttu-id="4b848-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b848-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4b848-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b848-127">Content-Type</span></span>  | <span data-ttu-id="4b848-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b848-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4b848-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b848-130">Request body</span></span>

<span data-ttu-id="4b848-131">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="4b848-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="4b848-132">**Observação:** Não é possível atualizar `membershipType` o valor de um canal existente.</span><span class="sxs-lookup"><span data-stu-id="4b848-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="4b848-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b848-133">Response</span></span>

<span data-ttu-id="4b848-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4b848-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4b848-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b848-135">Example</span></span>

### <a name="example-1-update-channel"></a><span data-ttu-id="4b848-136">Exemplo 1: canal de atualização</span><span class="sxs-lookup"><span data-stu-id="4b848-136">Example 1: Update channel</span></span>

#### <a name="request"></a><span data-ttu-id="4b848-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b848-137">Request</span></span>

<span data-ttu-id="4b848-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b848-138">Here is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```


#### <a name="response"></a><span data-ttu-id="4b848-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b848-139">Response</span></span>

<span data-ttu-id="4b848-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b848-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-channel-with-moderation-settings"></a><span data-ttu-id="4b848-141">Exemplo 2: Atualizar canal com configurações de moderação</span><span class="sxs-lookup"><span data-stu-id="4b848-141">Example 2: Update channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="4b848-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b848-142">Request</span></span>

<span data-ttu-id="4b848-143">O exemplo a seguir mostra uma solicitação para atualizar as [configurações de moderação](../resources/channelmoderationsettings.md) de um canal.</span><span class="sxs-lookup"><span data-stu-id="4b848-143">The following example shows a request to update the [moderation settings](../resources/channelmoderationsettings.md) of a channel.</span></span> <span data-ttu-id="4b848-144">Essa operação só pode ser executada por um proprietário da equipe.</span><span class="sxs-lookup"><span data-stu-id="4b848-144">This operation can only be performed by a team owner.</span></span>



# <a name="http"></a>[<span data-ttu-id="4b848-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b848-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel_with_moderationSettings"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
Content-type: application/json

{
    "displayName": "UpdateChannelModeration",
    "description": "Update channel moderation.",
    "moderationSettings": {
        "userNewMessageRestriction": "moderators",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```
# <a name="c"></a>[<span data-ttu-id="4b848-146">C#</span><span class="sxs-lookup"><span data-stu-id="4b848-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-channel-with-moderationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b848-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b848-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-channel-with-moderationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b848-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b848-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-with-moderationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b848-149">Java</span><span class="sxs-lookup"><span data-stu-id="4b848-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-channel-with-moderationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="4b848-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b848-150">Response</span></span>

<span data-ttu-id="4b848-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b848-151">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


