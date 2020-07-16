---
title: Canal de patch
description: Atualiza as propriedades do canal especificado.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7b3b9321fc4ce95fdbb06eeb83491344c7c40bd3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897803"
---
# <a name="patch-channel"></a><span data-ttu-id="757e6-103">Canal de patch</span><span class="sxs-lookup"><span data-stu-id="757e6-103">Patch channel</span></span>

<span data-ttu-id="757e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="757e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="757e6-105">Atualiza as propriedades do [canal](../resources/channel.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="757e6-105">Update the properties of the specified [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="757e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="757e6-106">Permissions</span></span>

<span data-ttu-id="757e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="757e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="757e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="757e6-109">Permission type</span></span>      | <span data-ttu-id="757e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="757e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="757e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="757e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="757e6-112">ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="757e6-112">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="757e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="757e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="757e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="757e6-114">Not supported.</span></span>    |
|<span data-ttu-id="757e6-115">Application</span><span class="sxs-lookup"><span data-stu-id="757e6-115">Application</span></span> | <span data-ttu-id="757e6-116">ChannelSettings. ReadWrite. All, Group. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="757e6-116">ChannelSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="757e6-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="757e6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="757e6-118">Os administradores globais e os administradores do serviço do Microsoft Teams podem acessar equipes das quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="757e6-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="757e6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="757e6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}/channels/{id}
```

## <a name="request-headers"></a><span data-ttu-id="757e6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="757e6-120">Request headers</span></span>

| <span data-ttu-id="757e6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="757e6-121">Header</span></span>       | <span data-ttu-id="757e6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="757e6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="757e6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="757e6-123">Authorization</span></span>  | <span data-ttu-id="757e6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="757e6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="757e6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="757e6-126">Content-Type</span></span>  | <span data-ttu-id="757e6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="757e6-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="757e6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="757e6-128">Request body</span></span>

<span data-ttu-id="757e6-129">No corpo da solicitação, fornça uma representação JSON do objeto [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="757e6-129">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="757e6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="757e6-130">Response</span></span>

<span data-ttu-id="757e6-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="757e6-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="757e6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="757e6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="757e6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="757e6-133">Request</span></span>

<span data-ttu-id="757e6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="757e6-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="757e6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="757e6-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "patch_channel"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}
```
# <a name="objective-c"></a>[<span data-ttu-id="757e6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="757e6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="757e6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="757e6-137">Response</span></span>

<span data-ttu-id="757e6-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="757e6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Patch channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
