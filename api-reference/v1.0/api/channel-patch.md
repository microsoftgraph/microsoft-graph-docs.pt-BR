---
title: Canal de patch
description: Atualiza as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3b46315ce93574a778e56fba9f924c2959413d64
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863919"
---
# <a name="patch-channel"></a><span data-ttu-id="e24ca-103">Canal de patch</span><span class="sxs-lookup"><span data-stu-id="e24ca-103">Patch channel</span></span>

<span data-ttu-id="e24ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e24ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e24ca-105">Atualiza as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="e24ca-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e24ca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e24ca-106">Permissions</span></span>

<span data-ttu-id="e24ca-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e24ca-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e24ca-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e24ca-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e24ca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e24ca-109">Permission type</span></span>      | <span data-ttu-id="e24ca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e24ca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e24ca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e24ca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e24ca-112">ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e24ca-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="e24ca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e24ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e24ca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e24ca-114">Not supported.</span></span>    |
|<span data-ttu-id="e24ca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e24ca-115">Application</span></span> | <span data-ttu-id="e24ca-116">ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e24ca-116">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e24ca-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="e24ca-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e24ca-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="e24ca-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e24ca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e24ca-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e24ca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e24ca-120">Request headers</span></span>

| <span data-ttu-id="e24ca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e24ca-121">Header</span></span>       | <span data-ttu-id="e24ca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e24ca-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e24ca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e24ca-123">Authorization</span></span>  | <span data-ttu-id="e24ca-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e24ca-124">Bearer {token}.</span></span> <span data-ttu-id="e24ca-125">Required.</span><span class="sxs-lookup"><span data-stu-id="e24ca-125">Required.</span></span>  |
| <span data-ttu-id="e24ca-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e24ca-126">Content-Type</span></span>  | <span data-ttu-id="e24ca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e24ca-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e24ca-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e24ca-128">Request body</span></span>

<span data-ttu-id="e24ca-129">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="e24ca-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e24ca-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e24ca-130">Response</span></span>

<span data-ttu-id="e24ca-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e24ca-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e24ca-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e24ca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e24ca-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e24ca-133">Request</span></span>

<span data-ttu-id="e24ca-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e24ca-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e24ca-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e24ca-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="e24ca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e24ca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e24ca-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e24ca-137">Response</span></span>

<span data-ttu-id="e24ca-138">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e24ca-138">Here is an example of the response.</span></span> <span data-ttu-id="e24ca-139">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e24ca-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e24ca-140">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e24ca-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 204 No Content
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
