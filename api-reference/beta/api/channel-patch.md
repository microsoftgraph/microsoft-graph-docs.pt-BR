---
title: Canal de patch
description: Atualiza as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fbfc08f634ff499ca73bd4102119cfd9d1795052
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895619"
---
# <a name="patch-channel"></a><span data-ttu-id="bf0a4-103">Canal de patch</span><span class="sxs-lookup"><span data-stu-id="bf0a4-103">Patch channel</span></span>

<span data-ttu-id="bf0a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf0a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf0a4-105">Atualiza as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf0a4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bf0a4-106">Permissions</span></span>

<span data-ttu-id="bf0a4-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bf0a4-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf0a4-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf0a4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf0a4-109">Permission type</span></span>      | <span data-ttu-id="bf0a4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bf0a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf0a4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf0a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf0a4-112">ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bf0a4-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="bf0a4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf0a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf0a4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-114">Not supported.</span></span>    |
|<span data-ttu-id="bf0a4-115">Application</span><span class="sxs-lookup"><span data-stu-id="bf0a4-115">Application</span></span> | <span data-ttu-id="bf0a4-116">ChannelSettings. Edit. Group \*, ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bf0a4-116">ChannelSettings.Edit.Group\*, ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="bf0a4-117">**Observação**: as permissões marcadas com \* usam o [consentimento específico do recurso]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bf0a4-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="bf0a4-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="bf0a4-119">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="bf0a4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf0a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bf0a4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf0a4-121">Request headers</span></span>
| <span data-ttu-id="bf0a4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf0a4-122">Header</span></span>       | <span data-ttu-id="bf0a4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bf0a4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf0a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf0a4-124">Authorization</span></span>  | <span data-ttu-id="bf0a4-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-125">Bearer {token}.</span></span> <span data-ttu-id="bf0a4-126">Required.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-126">Required.</span></span>  |
| <span data-ttu-id="bf0a4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf0a4-127">Content-Type</span></span>  | <span data-ttu-id="bf0a4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bf0a4-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf0a4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf0a4-129">Request body</span></span>

<span data-ttu-id="bf0a4-130">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="bf0a4-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

> <span data-ttu-id="bf0a4-131">Observação: não é possível atualizar o `membershipType` valor de um canal existente.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-131">Note: You cannot update the `membershipType` value for an existing channel.</span></span>

## <a name="response"></a><span data-ttu-id="bf0a4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf0a4-132">Response</span></span>

<span data-ttu-id="bf0a4-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bf0a4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf0a4-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf0a4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf0a4-135">Request</span></span>

<span data-ttu-id="bf0a4-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bf0a4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf0a4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="bf0a4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf0a4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bf0a4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf0a4-139">Response</span></span>

<span data-ttu-id="bf0a4-140">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-140">Here is an example of the response.</span></span> <span data-ttu-id="bf0a4-141">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bf0a4-142">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="bf0a4-142">All of the properties will be returned from an actual call.</span></span>
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
