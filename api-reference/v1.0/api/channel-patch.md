---
title: Canal patch
description: Atualize as propriedades do canal especificado.
author: anandjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c611ea955c82be94f5e0220fe0632d2c5791fc8
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51506864"
---
# <a name="patch-channel"></a><span data-ttu-id="35dff-103">Canal patch</span><span class="sxs-lookup"><span data-stu-id="35dff-103">Patch channel</span></span>

<span data-ttu-id="35dff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35dff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35dff-105">Atualize as propriedades do canal [especificado](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="35dff-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35dff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35dff-106">Permissions</span></span>

<span data-ttu-id="35dff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35dff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35dff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35dff-109">Permission type</span></span>      | <span data-ttu-id="35dff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35dff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35dff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35dff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35dff-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35dff-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="35dff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35dff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35dff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35dff-114">Not supported.</span></span>    |
|<span data-ttu-id="35dff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35dff-115">Application</span></span> | <span data-ttu-id="35dff-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35dff-116">ChannelSettings.ReadWrite.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="35dff-117">**Observação**: Permissões marcadas com \* usam [consentimento específico de recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="35dff-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="35dff-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="35dff-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="35dff-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="35dff-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="35dff-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35dff-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}/channels/{channel-id}
```

## <a name="request-headers"></a><span data-ttu-id="35dff-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35dff-121">Request headers</span></span>
| <span data-ttu-id="35dff-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35dff-122">Header</span></span>       | <span data-ttu-id="35dff-123">Valor</span><span class="sxs-lookup"><span data-stu-id="35dff-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35dff-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="35dff-124">Authorization</span></span>  | <span data-ttu-id="35dff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35dff-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="35dff-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35dff-127">Content-Type</span></span>  | <span data-ttu-id="35dff-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35dff-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35dff-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35dff-130">Request body</span></span>

<span data-ttu-id="35dff-131">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="35dff-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="35dff-132">**Observação:** Não é possível atualizar `membershipType` o valor de um canal existente.</span><span class="sxs-lookup"><span data-stu-id="35dff-132">**Note:** You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="35dff-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="35dff-133">Response</span></span>

<span data-ttu-id="35dff-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35dff-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="35dff-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35dff-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="35dff-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35dff-136">Request</span></span>

<span data-ttu-id="35dff-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35dff-137">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="35dff-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="35dff-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```
# <a name="objective-c"></a>[<span data-ttu-id="35dff-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35dff-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35dff-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="35dff-140">Response</span></span>

<span data-ttu-id="35dff-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35dff-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
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
